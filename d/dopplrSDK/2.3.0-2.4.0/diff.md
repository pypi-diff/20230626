# Comparing `tmp/dopplrSDK-2.3.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4236 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     6113 b- defN 23-Jun-16 05:45 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-16 12:24 dopplrSDK-2.3.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      537 b- defN 23-Jun-16 12:24 dopplrSDK-2.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 12:24 dopplrSDK-2.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-16 12:24 dopplrSDK-2.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-Jun-16 12:24 dopplrSDK-2.3.0.dist-info/RECORD
-6 files, 8306 bytes uncompressed, 3370 bytes compressed:  59.4%
+Zip file size: 4898 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    10779 b- defN 23-Jun-26 12:17 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      621 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/RECORD
+6 files, 13057 bytes uncompressed, 4032 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-2.3.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-2.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-2.3.0.dist-info/METADATA
+Filename: dopplrSDK-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-2.3.0.dist-info/WHEEL
+Filename: dopplrSDK-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-2.3.0.dist-info/top_level.txt
+Filename: dopplrSDK-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-2.3.0.dist-info/RECORD
+Filename: dopplrSDK-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -6,52 +6,84 @@
 import os
 import base64
 import hashlib
 from Crypto.Cipher import DES3
 from Crypto.Util.Padding import unpad
 from cryptography.fernet import Fernet
 from botocore.client import Config
+from azure.storage.blob import BlobServiceClient, BlobClient
 
-def decrypt_keys(de_key,s_key):
+def decrypt_keys(de_key):
     keys={}
-    key = s_key
+    key = "xLrwTFMdJroA8zG_5wnkQADuJvD5TTmfCKfe8RRz_xU="
     key = hashlib.md5(key.encode("utf-8")).digest()
     cipher_bytes = base64.b64decode(de_key)
     cipher = DES3.new(key, DES3.MODE_ECB)
     decrypted_bytes = cipher.decrypt(cipher_bytes)
     decrypted_text = unpad(decrypted_bytes, DES3.block_size).decode("utf-8")
     data=decrypted_text.split('|')
     
     for i in data:
         a=i.split(':')
         keys[a[0]]=a[1]
-    s3 = boto3.client('s3', aws_access_key_id=keys['Access'], aws_secret_access_key=keys['Secret'])
-    ContainerName = keys['Bucket']
-    file_key = 'Connections/Dopplr_Connection.ini'
-    db = {}
-    response = s3.get_object(Bucket=ContainerName, Key=file_key)
-    file_content = response['Body'].read()
-    key=s_key.encode('utf-8')
-    key=key
-    fernet = Fernet(key)
-    decrypted_data = fernet.decrypt(file_content)
-    decrypted_data = decrypted_data.decode('utf-8')
-    lines = decrypted_data.split('\n')
-    index=lines.index('[postgresql]\r')
-    data=lines[index+1:index+6]
+    if keys['Cloud'] == 'MinIO':
+        s3=boto3.client('s3',endpoint_url="http://20.219.94.221:9000",
+                      aws_access_key_id=keys['Access'],
+                      aws_secret_access_key=keys['Secret'],
+                      config=Config(signature_version='s3v4'),region_name="us-west-2"
+                      )
+    elif keys['Cloud'] == 'AWS':
+        s3 = boto3.client('s3', aws_access_key_id=keys['Access'], aws_secret_access_key=keys['Secret'])
+    elif keys['Cloud'] == 'AZURE':
+        connect_str = "DefaultEndpointsProtocol=https;AccountName={0};AccountKey={1};EndpointSuffix=core.windows.net".format(keys['Access'],keys['Secret'])            
+        s3 = BlobServiceClient.from_connection_string(connect_str)
+        
+    if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':       
+        ContainerName = keys['Bucket']
+        file_key = 'Connections/Dopplr_Connection.ini'
+        db = {}
+        response = s3.get_object(Bucket=ContainerName, Key=file_key)
+        file_content = response['Body'].read()
+        key = b"xLrwTFMdJroA8zG_5wnkQADuJvD5TTmfCKfe8RRz_xU="
+        fernet = Fernet(key)
+        decrypted_data = fernet.decrypt(file_content)
+        decrypted_data = decrypted_data.decode('utf-8')
+        lines = decrypted_data.split('\n')
+        index=lines.index('[postgresql]\r')
+        data=lines[index+1:index+6]
+
+        for i in data:
+            a=i.split('=')
+            db[a[0]]=a[1].replace('\r','')
+    else:
+        
+        ContainerName = keys['Bucket']
+        file_key = 'Connections/Dopplr_Connection.ini'
+        blob_client = s3.get_blob_client(container=ContainerName, blob=file_key)
+        az = blob_client.download_blob()
+        file_contents = az.readall()
+        key = b"xLrwTFMdJroA8zG_5wnkQADuJvD5TTmfCKfe8RRz_xU="
+        fernet = Fernet(key)
+        decrypted_data = fernet.decrypt(file_contents)
+        decrypted_data = decrypted_data.decode('utf-8')
+        lines = decrypted_data.split('\n')
+        index = lines.index('[postgresql]\r')
+        data = lines[index + 1: index + 6]
+        db = {}
+        for i in data:
+            a = i.split('=')
+            db[a[0]]=a[1].replace('\r', '')
+        
 
-    for i in data:
-        a=i.split('=')
-        db[a[0]]=a[1].replace('\r','')
     return keys,db,s3
 
-def putFileTomywrkspace(filePath,file_type,loginName,s_key):
+def putFileTomywrkspace(filePath,file_type,loginName,de_key):
     try:
-        keys,db,s3=decrypt_keys("zvkPurRjZz0ptGnEIxMq0tu3062oChYVkuUwkk7RG7pigQttPVQFkoHBQp+hb5dcYuGeb8asmxKv9XkaI9EnTTTT3YT4UvOF9cT46kotQRceh4oRzPwwKSWFUswJmtBBb2NNlUBFBae6qZqoozBn5g==",s_key)
-        
+        keys,db,client=decrypt_keys(de_key)
+
         query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
 
         ContainerName = keys['Bucket']
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
     
         cur=cnxn.cursor()
         cur.execute(query)
@@ -70,16 +102,15 @@
         results = cur.fetchone()
         if results[0]<1:
             insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name1[0]+"','"+file_type+"',null,'','Uploaded')"
             cur.execute(insert_query)
             cnxn.commit()
         else:
             pass
-            
-        
+                    
         cur1=cnxn.cursor()
         insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name1[0]+"'"
         
         cur1.execute(insert_query1)
         results = cur1.fetchone()
         SourceKey=results[0]
         SourceKey=str(SourceKey)
@@ -87,71 +118,126 @@
 
         ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/SOURCE/'+file_name)
         update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+"',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
         cur2=cnxn.cursor()
 
         cur2.execute(update_query)
         cnxn.commit()
-        s3.upload_file(filePath, ContainerName, ConnectionString)
-         # Generate a pre-signed URL
-        
-        s3.put_object_acl(ACL='public-read',
-                          Bucket=ContainerName,
-                          Key=ConnectionString)
-        
-        url = f"s3://{ContainerName}/{ConnectionString}"
-        print("uri : ",url)
-        cnxn.close()
-        #print("done")
+        if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
+            
+            client.upload_file(filePath, ContainerName, ConnectionString)
+             # Generate a pre-signed URL        
+            client.put_object_acl(ACL='public-read',
+                              Bucket=ContainerName,
+                              Key=ConnectionString)
+            
+            url = f"s3://{ContainerName}/{ConnectionString}"
+            print("uri : ",url)
+            cnxn.close()
+            #print("done")
+        else:
+            print(keys['Cloud'])
+            blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
+            with open(filePath, "rb") as data:
+                blob_client.upload_blob(data)
+            
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
         else:
             print("Error : ",error)
 
 
-def getWorkspaceFile(fileName,destination,loginName,s_key):
+def getWorkspaceFile(fileName,destination,loginName,de_key):
+    try:
 
-    keys,db,s3=decrypt_keys("zvkPurRjZz0ptGnEIxMq0tu3062oChYVkuUwkk7RG7pigQttPVQFkoHBQp+hb5dcYuGeb8asmxKv9XkaI9EnTTTT3YT4UvOF9cT46kotQRceh4oRzPwwKSWFUswJmtBBb2NNlUBFBae6qZqoozBn5g==",s_key)
+        def is_file_name_same(file_path, expected_file_name):
+            file_name = os.path.basename(file_path)
+            return file_name == expected_file_name
 
-    
-    query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
-    ContainerName = keys['Bucket']
-    cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
-
-    cur=cnxn.cursor()
-    cur.execute(query)
-    results = cur.fetchone()
+        keys,db,client=decrypt_keys(de_key)
         
+        query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
+        ContainerName = keys['Bucket']
+        cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
+        cur=cnxn.cursor()
+        cur.execute(query)
+        results = cur.fetchone()
+        UserKey=results[1]
+        OrgName=results[0]
+        folder_prefix = OrgName+'/'+loginName.upper()+'/'
+        # Check if the file exists
+        if os.path.exists(destination):
+            print('folder exists')
+        else:
+            os.mkdir(destination)
+        if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
+            response = client.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
+            destination=destination+'/'+fileName
+            for obj in response['Contents']:
+                key = obj['Key']               
+                is_same = is_file_name_same(key, fileName)
+                if(is_same):                
+                    client.download_file(ContainerName, key, destination)
+                    print("download")
+        else:
+            container_client = client.get_container_client(ContainerName)
 
+            destination=destination+'/'+fileName
+            blobs = container_client.list_blobs()
+            for blob in blobs:
+                #print(blob.name)
+                is_same = is_file_name_same(blob.name, fileName)
+                if(is_same):                  
+                    with open(destination, "wb") as my_blob:
+                        blob_client = container_client.get_blob_client(blob.name)
+                        blob_data = blob_client.download_blob()
+                        blob_data.readinto(my_blob)
+                        print("downloaded")
+                        
+    except Exception as error:
+        print("Error : ",error)
 
-    UserKey=results[1]
-    OrgName=results[0]
-    folder_prefix = OrgName+'/'+loginName.upper()+'/'
-        
+def getWorkspaceFolderFiles(folder,destination,loginName,de_key):
+    try:
+        keys,db,client=decrypt_keys(de_key)
 
-    # Check if the file exists
-    if os.path.exists(destination):
-        print('folder exists')
-    else:
-        os.mkdir(destination)
+        query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
+        cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
+        cur=cnxn.cursor()
+        cur.execute(query)
+        results = cur.fetchone()
+        UserKey=results[1]
+        OrgName=results[0]
+        folder_prefix = OrgName+'/'+loginName.upper()+'/'+folder
+        ContainerName = keys['Bucket']
+        if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
+            response = client.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
+            for obj in response['Contents']:
+                key = obj['Key']
+                if not key.endswith('/'):  # Exclude subdirectories
+                    file_name = os.path.join(destination, os.path.basename(key))
+                    client.download_file(ContainerName, key, file_name)  # Download the file
+            print("downloaded")
+        else:
+            
+            folder_prefix = OrgName+'/'+loginName.upper()+'/'+folder
+            container_client = client.get_container_client(ContainerName)
+            blobs = container_client.list_blobs(name_starts_with=folder_prefix)
+
+            for blob in blobs:
+                blob_client = container_client.get_blob_client(blob.name)
+                file_path = os.path.join(destination, os.path.basename(blob.name))
+                os.makedirs(os.path.dirname(file_path), exist_ok=True)
+                with open(file_path, "wb") as file:
+                    file.write(blob_client.download_blob().readall())
+            print("downloaded")
 
-    response = s3.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
-    # Iterate through the objects
-    destination=destination+'/'+fileName
-    for obj in response['Contents']:
-        key = obj['Key']
+        
+    except Exception as error:
+        print("Error : ",error)
 
-            
-        is_same = is_file_name_same(key, fileName)
 
-        if(is_same):                
-            s3.download_file(ContainerName, key, destination)
-            print("download")
-
-def is_file_name_same(file_path, expected_file_name):
-        file_name = os.path.basename(file_path)
-        return file_name == expected_file_name
```

## Comparing `dopplrSDK-2.3.0.dist-info/LICENSE.txt` & `dopplrSDK-2.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-2.3.0.dist-info/METADATA` & `dopplrSDK-2.4.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 2.3.0
+Version: 2.4.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: psycopg2-binary (==2.9.6)
 Requires-Dist: pandas (==2.0.2)
 Requires-Dist: boto3 (==1.26.153)
 Requires-Dist: pycryptodome (==3.18.0)
 Requires-Dist: cryptography (==41.0.6)
+Requires-Dist: azure-storage-blob (==12.15.0)
+Requires-Dist: botocore (==1.29.79)
 
 UNKNOWN
```

