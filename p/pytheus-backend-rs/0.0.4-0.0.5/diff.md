# Comparing `tmp/pytheus_backend_rs-0.0.4.tar.gz` & `tmp/pytheus_backend_rs-0.0.5.tar.gz`

## Comparing `pytheus_backend_rs-0.0.4.tar` & `pytheus_backend_rs-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.4/Cargo.toml
--rw-r--r--   0     1001      123     2792 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/.gitignore
--rw-r--r--   0     1001      123      620 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/pyproject.toml
--rw-r--r--   0     1001      123    10149 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/src/lib.rs
--rw-r--r--   0     1001      123    11135 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/Cargo.lock
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      319 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      123     2792 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/.gitignore
+-rw-r--r--   0     1001      123      620 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/pyproject.toml
+-rw-r--r--   0     1001      123    13267 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      123    12764 2023-06-25 23:52:04.000000 pytheus_backend_rs-0.0.5/Cargo.lock
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.5/PKG-INFO
```

### Comparing `pytheus_backend_rs-0.0.4/.github/workflows/CI.yml` & `pytheus_backend_rs-0.0.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.4/.gitignore` & `pytheus_backend_rs-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.4/pyproject.toml` & `pytheus_backend_rs-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.4/src/lib.rs` & `pytheus_backend_rs-0.0.5/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,119 @@
+use crossbeam::channel;
 use itertools::Itertools;
 use pyo3::exceptions::PyException;
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyType};
 use redis::Commands;
 use redis::{Connection, RedisResult};
 use std::collections::HashMap;
 use std::sync::{mpsc, Mutex, OnceLock};
 use std::thread;
 
 // This could be completely wrong, not sure if it would break the channel, let's try 🤞
 static REDIS_JOB_TX: OnceLock<Mutex<mpsc::Sender<RedisJob>>> = OnceLock::new();
+static REDIS_PIPELINE_JOB_TX: OnceLock<Mutex<channel::Sender<RedisPipelineJob>>> = OnceLock::new();
 const EXPIRE_KEY_SECONDS: usize = 3600;
 
-#[derive(Debug)]
 enum BackendAction {
     Inc,
     Dec,
     Set,
-    Get,
 }
 
 #[derive(Debug)]
-struct RedisJobResult {
-    value: f64,
+struct RedisPipelineJobResult {
+    values: Vec<f64>,
 }
 
-#[derive(Debug)]
 struct RedisJob {
     action: BackendAction,
     key_name: String,
     labels_hash: Option<String>,
     value: f64,
-    result_tx: Option<mpsc::Sender<RedisJobResult>>,
 }
 
+struct RedisPipelineJob {
+    pipeline: redis::Pipeline,
+    result_tx: mpsc::Sender<RedisPipelineJobResult>,
+}
+
+#[derive(Debug)]
 #[pyclass]
 struct RedisBackend {
     #[pyo3(get)]
     config: Py<PyDict>,
     #[pyo3(get)]
     metric: Py<PyAny>,
     #[pyo3(get)]
     histogram_bucket: Option<String>,
     redis_job_tx: mpsc::Sender<RedisJob>,
     key_name: String,
     labels_hash: Option<String>,
 }
 
+// Sample(suffix='_bucket', labels={'le': '0.005'}, value=0.0
+#[derive(Debug, FromPyObject)]
+struct Sample<'a> {
+    suffix: String,
+    labels: Option<HashMap<String, String>>,
+    value: PyRef<'a, RedisBackend>,
+}
+
+#[derive(Debug)]
+#[pyclass]
+struct OutSample {
+    #[pyo3(get)]
+    suffix: String,
+    #[pyo3(get)]
+    labels: Option<HashMap<String, String>>,
+    #[pyo3(get)]
+    value: f64,
+}
+
+impl OutSample {
+    fn new(suffix: String, labels: Option<HashMap<String, String>>, value: f64) -> Self {
+        Self {
+            suffix,
+            labels,
+            value,
+        }
+    }
+}
+
+#[derive(Debug)]
+struct SamplesResultDict {
+    collectors: Vec<Py<PyAny>>,
+    samples_vec: Vec<Vec<OutSample>>,
+}
+
+impl SamplesResultDict {
+    fn new() -> Self {
+        Self {
+            collectors: vec![],
+            samples_vec: vec![],
+        }
+    }
+}
+
+impl IntoPy<PyResult<PyObject>> for SamplesResultDict {
+    fn into_py(self, py: Python<'_>) -> PyResult<PyObject> {
+        let pydict = PyDict::new(py);
+        for (collector, samples) in self
+            .collectors
+            .into_iter()
+            .zip(self.samples_vec.into_iter())
+        {
+            pydict.set_item(collector, samples.into_py(py))?;
+        }
+        Ok(pydict.into())
+    }
+}
+
 fn create_redis_connection(host: &str, port: u16) -> RedisResult<Connection> {
     let url = format!("redis://{host}:{port}");
     let client = redis::Client::open(url)?;
     let con = client.get_connection()?;
     Ok(con)
 }
 
@@ -117,34 +179,56 @@
             redis_job_tx: cloned_tx,
             key_name,
             labels_hash,
         })
     }
 
     #[classmethod]
-    fn _initialize(cls: &PyType, config: &PyDict) -> PyResult<()> {
-        println!("hello: {}", cls);
-
+    fn _initialize(_cls: &PyType, config: &PyDict) -> PyResult<()> {
         // using the PyAny::get_item so that it will raise a KeyError on missing key
         let host: &str = PyAny::get_item(config, intern!(config.py(), "host"))?.extract()?;
         let port: u16 = PyAny::get_item(config, intern!(config.py(), "port"))?.extract()?;
 
         let mut connection = match create_redis_connection(host, port) {
             Ok(connection) => connection,
             Err(e) => return Err(PyException::new_err(e.to_string())),
         };
 
         // producer / consumer
         let (tx, rx) = mpsc::channel();
         REDIS_JOB_TX.get_or_init(|| Mutex::new(tx));
 
+        let (pipeline_tx, pipeline_rx) = crossbeam::channel::unbounded();
+        REDIS_PIPELINE_JOB_TX.get_or_init(|| Mutex::new(pipeline_tx));
+
+        for i in 0..4 {
+            let cloned_pipeline_rx = pipeline_rx.clone();
+            let mut pipeline_connection = match create_redis_connection(host, port) {
+                Ok(connection) => connection,
+                Err(e) => return Err(PyException::new_err(e.to_string())),
+            };
+            thread::spawn(move || {
+                println!("Starting pipeline thread....{i}");
+                while let Ok(received) = cloned_pipeline_rx.recv() {
+                    let pipe = received.pipeline;
+                    let results: Vec<Option<f64>> = pipe.query(&mut pipeline_connection).unwrap();
+
+                    let values = results.into_iter().map(|val| val.unwrap_or(0f64)).collect();
+
+                    received
+                        .result_tx
+                        .send(RedisPipelineJobResult { values })
+                        .unwrap();
+                }
+            });
+        }
+
         thread::spawn(move || {
-            println!("In thread....");
+            println!("Starting BackendAction thread....");
             while let Ok(received) = rx.recv() {
-                println!("Got: {:?}", received);
                 match received.action {
                     BackendAction::Inc | BackendAction::Dec => {
                         match received.labels_hash {
                             Some(labels_hash) => connection
                                 .hincr(&received.key_name, &labels_hash, received.value)
                                 .unwrap(),
                             None => connection.incr(&received.key_name, received.value).unwrap(),
@@ -160,106 +244,134 @@
                                 .unwrap(),
                             None => connection.set(&received.key_name, received.value).unwrap(),
                         }
                         let _: () = connection
                             .expire(&received.key_name, EXPIRE_KEY_SECONDS)
                             .unwrap();
                     }
-                    BackendAction::Get => {
-                        let get_result: Result<f64, redis::RedisError> = match received.labels_hash
-                        {
-                            Some(labels_hash) => connection.hget(&received.key_name, &labels_hash),
-                            None => connection.get(&received.key_name),
-                        };
-                        let value: f64 = match get_result {
-                            Ok(value) => {
-                                // TODO: most likely will need to queue these operations
-                                // waiting on the expire call before returning the value is not
-                                // good
-                                let _: () = connection
-                                    .expire(&received.key_name, EXPIRE_KEY_SECONDS)
-                                    .unwrap();
-                                value
-                            }
-                            Err(e) => {
-                                if e.kind() == redis::ErrorKind::TypeError {
-                                    // This would happen when there is no key so `nil` is returned
-                                    // so we return the default 0.0 value
-                                    0.0
-                                } else {
-                                    // TODO: will need to handle the panic
-                                    panic!("{e:?}");
-                                }
-                            }
-                        };
-
-                        received
-                            .result_tx
-                            .unwrap()
-                            .send(RedisJobResult { value })
-                            .unwrap();
-                    }
                 }
             }
         });
 
         Ok(())
     }
 
+    #[classmethod]
+    fn _generate_samples(cls: &PyType, registry: &PyAny) -> PyResult<PyObject> {
+        let py = cls.py();
+        let collectors = registry.call_method0(intern!(py, "collect"))?;
+
+        let metric_collectors: PyResult<Vec<&PyAny>> = collectors
+            .iter()?
+            .map(|i| i.and_then(PyAny::extract))
+            .collect();
+
+        let mut samples_result_dict = SamplesResultDict::new();
+
+        let mut pipe = redis::pipe();
+
+        // TODO: need to support custom collectors
+        for metric_collector in metric_collectors? {
+            let mut samples_list: Vec<OutSample> = vec![];
+
+            let samples: PyResult<Vec<&PyAny>> = metric_collector
+                .call_method0(intern!(py, "collect"))?
+                .iter()?
+                .map(|i| i.and_then(PyAny::extract))
+                .collect();
+
+            for sample in samples? {
+                let sample: Sample = sample.extract()?;
+
+                // struct used for converting from python back into python are different
+                // probably because they share the same name with the existing `Sample` class
+                let out_sample = OutSample::new(sample.suffix, sample.labels, 0.0);
+                samples_list.push(out_sample);
+
+                // pipe the get command
+                let key_name = &sample.value.key_name;
+                let label_hash = &sample.value.labels_hash;
+
+                match label_hash {
+                    Some(label_hash) => pipe.hget(key_name, label_hash),
+                    None => pipe.get(key_name),
+                };
+                pipe.expire(key_name, EXPIRE_KEY_SECONDS).ignore();
+            }
+
+            samples_result_dict.collectors.push(metric_collector.into());
+            samples_result_dict.samples_vec.push(samples_list);
+        }
+
+        let send_tx = {
+            let redis_pipeline_job_tx_job_tx_mutex = REDIS_PIPELINE_JOB_TX.get().unwrap();
+            let redis_pipeline_job_tx = redis_pipeline_job_tx_job_tx_mutex.lock().unwrap();
+            redis_pipeline_job_tx.clone()
+        };
+
+        let (tx, rx) = mpsc::channel();
+
+        send_tx
+            .send(RedisPipelineJob {
+                result_tx: tx,
+                pipeline: pipe,
+            })
+            .unwrap();
+
+        let job_result = rx.recv().unwrap();
+
+        // map back the values from redis into the appropriate Sample
+        let mut samples_vec_united = vec![];
+        for samples_vec in &mut samples_result_dict.samples_vec {
+            samples_vec_united.extend(samples_vec);
+        }
+
+        for (sample, value) in samples_vec_united.iter_mut().zip(job_result.values) {
+            sample.value = value
+        }
+        samples_result_dict.into_py(py)
+    }
+
     fn inc(&self, value: f64) {
         self.redis_job_tx
             .send(RedisJob {
                 action: BackendAction::Inc,
                 key_name: self.key_name.clone(),
                 labels_hash: self.labels_hash.clone(), // I wonder if only the String inside should be cloned into a new Some
                 value,
-                result_tx: None,
             })
             .unwrap();
     }
 
     fn dec(&self, value: f64) {
         self.redis_job_tx
             .send(RedisJob {
                 action: BackendAction::Dec,
                 key_name: self.key_name.clone(),
                 labels_hash: self.labels_hash.clone(),
                 value: -value,
-                result_tx: None,
             })
             .unwrap();
     }
 
     fn set(&self, value: f64) {
         self.redis_job_tx
             .send(RedisJob {
                 action: BackendAction::Set,
                 key_name: self.key_name.clone(),
                 labels_hash: self.labels_hash.clone(),
                 value,
-                result_tx: None,
             })
             .unwrap();
     }
 
-    fn get(&self) -> f64 {
-        let (tx, rx) = mpsc::channel();
-        self.redis_job_tx
-            .send(RedisJob {
-                action: BackendAction::Get,
-                key_name: self.key_name.clone(),
-                labels_hash: self.labels_hash.clone(),
-                value: f64::NAN,
-                result_tx: Some(tx),
-            })
-            .unwrap();
-
-        // TODO: should free the GIL in here
-        let job_result = rx.recv().unwrap();
-        job_result.value
+    fn get(self_: PyRef<Self>) -> PyRef<'_, RedisBackend> {
+        // This returns itself so that we have a RedisBackend instance to retrieve key_name and
+        // labels_hash to query redis when collecting samples via a pipeline.
+        self_
     }
 }
 
 #[pyclass]
 struct SingleProcessBackend {
     #[pyo3(get)]
     config: Py<PyDict>,
@@ -304,9 +416,10 @@
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn pytheus_backend_rs(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<RedisBackend>()?;
     m.add_class::<SingleProcessBackend>()?;
+    m.add_class::<OutSample>()?;
     Ok(())
 }
```

### Comparing `pytheus_backend_rs-0.0.4/Cargo.lock` & `pytheus_backend_rs-0.0.5/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,81 @@
 checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
+name = "crossbeam"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2801af0d36612ae591caa9568261fddce32ce6e08a7275ea334a06a4ad021a2c"
+dependencies = [
+ "cfg-if",
+ "crossbeam-channel",
+ "crossbeam-deque",
+ "crossbeam-epoch",
+ "crossbeam-queue",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-channel"
+version = "0.5.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-deque"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+dependencies = [
+ "cfg-if",
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "crossbeam-utils",
+ "memoffset",
+ "scopeguard",
+]
+
+[[package]]
+name = "crossbeam-queue"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d1cfb3ea8a53f37c40dea2c7bedcbd88bdfae54f5e2175d6ecaff1c988353add"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "form_urlencoded"
@@ -215,16 +282,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytheus-backend-rs"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
+ "crossbeam",
  "itertools",
  "pyo3",
  "redis",
 ]
 
 [[package]]
 name = "quote"
```

