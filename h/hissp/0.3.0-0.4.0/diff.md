# Comparing `tmp/hissp-0.3.0-py3-none-any.whl.zip` & `tmp/hissp-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 42664 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      807 b- defN 22-Feb-09 05:51 hissp/__init__.py
--rw-rw-rw-  2.0 fat     1881 b- defN 22-Feb-09 05:51 hissp/__main__.py
--rw-rw-rw-  2.0 fat    16661 b- defN 22-Feb-09 05:51 hissp/basic.lissp
--rw-rw-rw-  2.0 fat    43218 b- defN 22-Feb-09 05:52 hissp/basic.py
--rw-rw-rw-  2.0 fat    16919 b- defN 22-Feb-09 05:51 hissp/compiler.py
--rw-rw-rw-  2.0 fat     5698 b- defN 22-Feb-09 05:51 hissp/munger.py
--rw-rw-rw-  2.0 fat    16481 b- defN 22-Feb-09 05:51 hissp/reader.py
--rw-rw-rw-  2.0 fat     2703 b- defN 22-Feb-09 05:51 hissp/repl.py
--rw-rw-rw-  2.0 fat    11358 b- defN 22-Feb-09 05:52 hissp-0.3.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    18637 b- defN 22-Feb-09 05:52 hissp-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Feb-09 05:52 hissp-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       47 b- defN 22-Feb-09 05:52 hissp-0.3.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 22-Feb-09 05:52 hissp-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1058 b- defN 22-Feb-09 05:52 hissp-0.3.0.dist-info/RECORD
-14 files, 135566 bytes uncompressed, 40946 bytes compressed:  69.8%
+Zip file size: 94072 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-26 01:25 hissp/__init__.py
+-rw-rw-rw-  2.0 fat     1927 b- defN 23-Jun-26 01:25 hissp/__main__.py
+-rw-rw-rw-  2.0 fat    18896 b- defN 23-Jun-26 00:00 hissp/compiler.py
+-rw-rw-rw-  2.0 fat    96125 b- defN 23-Jun-21 04:58 hissp/macros.lissp
+-rw-rw-rw-  2.0 fat   257822 b- defN 23-Jun-26 03:32 hissp/macros.py
+-rw-rw-rw-  2.0 fat     5870 b- defN 23-Jun-15 04:56 hissp/munger.py
+-rw-rw-rw-  2.0 fat    20531 b- defN 23-Jun-26 00:59 hissp/reader.py
+-rw-rw-rw-  2.0 fat     3569 b- defN 23-Jun-17 17:00 hissp/repl.py
+-rw-rw-rw-  2.0 fat    11358 b- defN 23-Jun-26 03:32 hissp-0.4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    28422 b- defN 23-Jun-26 03:32 hissp-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 03:32 hissp-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       46 b- defN 23-Jun-26 03:32 hissp-0.4.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-26 03:32 hissp-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1062 b- defN 23-Jun-26 03:32 hissp-0.4.0.dist-info/RECORD
+14 files, 448246 bytes uncompressed, 92350 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
 Filename: hissp/__init__.py
 Comment: 
 
 Filename: hissp/__main__.py
 Comment: 
 
-Filename: hissp/basic.lissp
+Filename: hissp/compiler.py
 Comment: 
 
-Filename: hissp/basic.py
+Filename: hissp/macros.lissp
 Comment: 
 
-Filename: hissp/compiler.py
+Filename: hissp/macros.py
 Comment: 
 
 Filename: hissp/munger.py
 Comment: 
 
 Filename: hissp/reader.py
 Comment: 
 
 Filename: hissp/repl.py
 Comment: 
 
-Filename: hissp-0.3.0.dist-info/LICENSE.txt
+Filename: hissp-0.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hissp-0.3.0.dist-info/METADATA
+Filename: hissp-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: hissp-0.3.0.dist-info/WHEEL
+Filename: hissp-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: hissp-0.3.0.dist-info/entry_points.txt
+Filename: hissp-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: hissp-0.3.0.dist-info/top_level.txt
+Filename: hissp-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hissp-0.3.0.dist-info/RECORD
+Filename: hissp-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hissp/__init__.py

```diff
@@ -1,20 +1,58 @@
-# Copyright 2020 Matthew Egan Odendahl
+# Copyright 2020, 2022 Matthew Egan Odendahl
 # SPDX-License-Identifier: Apache-2.0
 
 # Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this module except in compliance with the License.
+# you may not use this package except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# :Abguvatarff nobir nofgenpgvba:  ohg vzcyrzragngvba vf / gur orfg anzr.:Grefrarff znl znxr bar gbb znal / trg hfrq~
+# gb gurz:  ryfr biresybj lbhe oenva.:Ab fhofgvghgr sbe haqrefgnaqvat:Pbqr;     gur yvnovyvgl:nf nffrg;~
+# gur   novyvgl.:Gur ovttrfg puhaxf / ner uneq gb fjnyybj:  nf fvzcyr nf cbffvoyr / ab zber.:Fbhepr jnf znqr / sbe gur~
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# uhzna:  bowrpg / gur znpuvar.:Ner lbh ynml rabhtu gb orne / gur fvaprerfg sbez / bs bgure jnlf bs orvat?:*univat*~
+# qrprag fgnaqneqf / vf zber vzcbegnag / guna rknpgyl jung gurl ner:Cresrpgvba / vf rkcrafvir:  zntvp / uvtuyl~
+# cevprq:  cnl sbe jura / vg'f Jbegu Vg:  n dhnegre vf nqivfrq:Ernqnovyvgl / vf znvayl / ynvq bhg ba gur cntr.:Tbysvat~
+# / znxrf tbbq cenpgvpr / orfg cenpgvpr vg orgenlf.:Pnfgyrf ohvyg / va gur nve / juvgure gurl qb orybat?:  Ryrtnapr /~
+# gura rkprcgvba:  Sbez / orsber qrgnvy:  jurapr haqre gurz,:Sbhaqngvbaf nccrne.:Znxr gur evtug jnl boivbhf,:zrqvgngr~
+# ba guvf.:  --Mn Mra bs Uvffc:~
+"""It's Python with a `Lissp`.
+
+See the GitHub project for complete documentation and tests.
+
+https://github.com/gilch/hissp
+
+``__init__.py`` imports several utilities for convenience, including
+
+* `hissp.compiler.readerless`,
+* `hissp.munger.demunge`,
+* `hissp.munger.munge`,
+* `hissp.reader.transpile`, and
+* `hissp.repl.interact`,
+
+as well as the `hissp.macros._macro_` namespace, making all the bundled
+macros available with the shorter ``hissp.._macro_`` qualifier.
+"""
+from hissp.compiler import Compiler, readerless
+from hissp.munger import demunge, munge
+from hissp.reader import transpile
+from hissp.repl import interact
+
+from contextlib import suppress
+
+# Hissp must be importable to compile macros.lissp in the first place.
+with suppress(ImportError):
+    # noinspection PyUnresolvedReferences
+    from hissp.macros import _macro_
+del suppress
 
-# TODO: fill in docstrings for all modules
-# TODO: Organize into private modules for utility and public modules for interface?
-#  Maybe split Lissp from Hissp?
 
-__version__ = "0.3.0"
+VERSION = "0.4.0"
```

## hissp/__main__.py

```diff
@@ -3,17 +3,18 @@
 """
 Hissp's command-line interface.
 """
 
 import argparse
 import re
 import sys
+import traceback
 
 import hissp.repl
-from hissp import __version__ as ver
+from hissp import VERSION
 from hissp.reader import Lissp
 
 
 def main():
     """
     Entry point for the `lissp command`.
     """
@@ -27,41 +28,43 @@
     else:
         hissp.repl.main(__main__)
 
 
 def _cmd(args, ns):
     sys.argv = ["-c"]
     sys.argv.extend([args.file, *args.args])
-    args.i("(hissp.basic.._macro_.prelude)\n" + args.c, ns)
+    args.i("(hissp.._macro_.prelude)\n" + args.c, ns)
 
 
 def _with_args(args, ns):
     with argparse.FileType("r", encoding="utf8")(args.file) as file:
         sys.argv = [file.name, *args.args]
         code = file.read()
     args.i(re.sub("^#!.*\n", "\n", code), ns)
 
 
 def _interact(code, ns):
     repl = hissp.repl.LisspREPL(locals=ns)
     repl.lissp.compiler.evaluate = True
     try:
         repl.lissp.compile(code)
+    except:
+        traceback.print_exc()
     finally:
         repl.lissp.compiler.evaluate = False
         repl.interact()
 
 
 def _no_interact(code, ns):
     Lissp(ns=ns, evaluate=True).compile(code)
 
 
 def _arg_parser():
     root = argparse.ArgumentParser(
-        description=f"(Hissp {ver}) Starts a LisspREPL if there are no arguments."
+        description=f"(Hissp {VERSION}) Starts a LisspREPL if there are no arguments."
     )
     _ = root.add_argument
     _(
         "-i",
         action="store_const",
         const=_interact,
         default=_no_interact,
```

## hissp/compiler.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019, 2020, 2021, 2022 Matthew Egan Odendahl
+# Copyright 2019, 2020, 2021, 2022, 2023 Matthew Egan Odendahl
 # SPDX-License-Identifier: Apache-2.0
 
 """
 The Hissp data-structure language compiler and associated helper functions.
 """
 
 import ast
@@ -25,17 +25,17 @@
 # Module Macro container
 MACROS = "_macro_"
 # Macro from foreign module foo.bar.._macro_.baz
 MACRO = f"..{MACROS}."
 MAYBE = "..QzMaybe_."
 RE_MACRO = re.compile(rf"({re.escape(MACRO)}|{re.escape(MAYBE)})")
 
-NS = ContextVar("NS", default=())
+NS = ContextVar("NS", default=None)
 """
-Sometimes macros need the current namespace when expanding,
+Sometimes a macro needs the current namespace when expanding,
 instead of its defining namespace.
 Rather than pass in an implicit argument to all macros,
 it's available here.
 `readerless` uses this automatically.
 """
 
 Sentinel = NewType("Sentinel", object)
@@ -44,31 +44,43 @@
 
 class CompileError(SyntaxError):
     """Catch-all exception for compilation failures."""
 
 
 def _trace(method):
     @wraps(method)
-    def tracer(self, expr):
+    def tracer(self, expr) -> str:
         try:
             return method(self, expr)
         except Exception as e:
             self.error = e
             message = (
-                f"\nCompiler.{method.__name__}() {type(e).__name__}:\n {e}".replace(
-                    "\n", "\n# "
-                )
+                "\nCompiler.{}() {}:\n {}".format(
+                    method.__name__,
+                    type(e).__name__,
+                    format_exc() if method.__name__ == "macro" else e,
+                ).replace("\n", "\n# ")
+                + "\n"
             )
             return f"(>   >  > >>{pformat(expr)}<< <  <   <){message}"
 
     return tracer
 
 
 class PostCompileWarning(Warning):
-    """Form compiled to Python, but execution of it failed."""
+    """Form compiled to Python, but its execution failed.
+
+    Only possible when compiling in evaluate mode and not in __main__.
+    Would be a "Hissp Abort!" instead when in __main__, but other
+    modules can be allowed to continue compiling for debugging purposes.
+
+    Continuing execution after a failure can be dangerous if non-main
+    modules have side effects besides definitions. Warnings can be
+    upgraded to errors if this is a concern. See `warnings` for how.
+    """
 
 
 class Compiler:
     """
     The Hissp recursive-descent compiler.
 
     Translates the Hissp data-structure language into a functional
@@ -76,15 +88,15 @@
     """
 
     def __init__(self, qualname="__main__", ns=None, evaluate=True):
         self.qualname = qualname
         self.ns = self.new_ns(qualname) if ns is None else ns
         self.evaluate = evaluate
         self.error = False
-        self.abort = False
+        self.abort = None
 
     @staticmethod
     def new_ns(name, doc=None, package=None):
         """Creates and initializes a dict namespace like a module,
         with the given `__name__`, ``__doc__``, and `__package__`;
         ``__builtins__``; an empty ``__annotations__``; and whatever
         else Python currently adds to new module objects.
@@ -96,24 +108,24 @@
         return vars(mod)
 
     def compile(self, forms: Iterable) -> str:
         """
         Compile multiple forms, and execute them if evaluate mode enabled.
         """
         result: List[str] = []
-        for form in forms:
+        for i, form in enumerate(forms, 1):
             form = self.form(form)
             if self.error:
                 e = self.error
                 self.error = False
                 raise CompileError("\n" + form) from e
-            result.extend(self.eval(form))
+            result.extend(self.eval(form, i))
             if self.abort:
-                print("\n\n".join(result), file=sys.stderr)
-                self.abort = False  # To allow REPL debugging.
+                print("Hissp abort!", self.abort, sep="\n", file=sys.stderr)
+                self.abort = None  # To allow REPL debugging.
                 sys.exit(1)
         return "\n\n".join(result)
 
     @_trace
     def form(self, form) -> str:
         """
         Compile Hissp form to the equivalent Python code in a string.
@@ -132,52 +144,67 @@
         head, *tail = form
         if type(head) is str:
             return self.special(form)
         return self.call(form)
 
     @_trace
     def special(self, form: Tuple) -> str:
-        """Try to compile as special form, else `invocation`."""
+        """Try to compile as special form, else `invocation`.
+
+        The two special forms are ``quote`` and `lambda<function>`.
+
+        A quote form evaluates to its argument, treated as literal data,
+        not evaluated. Notice the difference in the `readerless`
+        compiled output.
+
+        >>> print(readerless(('print',42,)))  # function call
+        print(
+          (42))
+        >>> print(readerless(('quote',('print',42,),)))  # tuple
+        ('print',
+         (42),)
+
+        """
         if form[0] == "quote":
             return self.atom(*form[1:])
         if form[0] == "lambda":
             return self.function(form)
         return self.invocation(form)
 
     @_trace
     def function(self, form: Tuple) -> str:
         R"""
         Compile the anonymous function special form.
 
         (lambda (<parameters>)
           <body>)
 
-        The parameters tuple is divided into (<single> : <paired>)
+        The parameters tuple is divided into (<singles> : <pairs>)
 
         Parameter types are the same as Python's.
         For example,
 
         >>> readerless(
-        ... ('lambda', ('a',':/','b',
-        ...             ':', 'e',1, 'f',2,
-        ...             ':*','args', 'h',4, 'i',':?', 'j',1,
-        ...             ':**','kwargs',),
-        ...   42,),
+        ... ('lambda', ('a',':/','b'
+        ...            ,':', 'e',1, 'f',2
+        ...            ,':*','args', 'h',4, 'i',':?', 'j',1
+        ...            ,':**','kwargs',)
+        ...  ,42,)
         ... )
         '(lambda a,/,b,e=(1),f=(2),*args,h=(4),i,j=(1),**kwargs:(42))'
 
         The special control words ``:*`` and ``:**`` designate the
         remainder of the positional and keyword parameters, respectively.
         Note this body evaluates expressions in sequence, for side
         effects.
 
         >>> print(readerless(
-        ... ('lambda', (':',':*','args',':**','kwargs',),
-        ...   ('print','args',),
-        ...   ('print','kwargs',),),
+        ... ('lambda', (':',':*','args',':**','kwargs',)
+        ...  ,('print','args',)
+        ...  ,('print','kwargs',),)
         ... ))
         (lambda *args,**kwargs:(
           print(
             args),
           print(
             kwargs))[-1])
 
@@ -197,60 +224,63 @@
         >>> readerless(('lambda', ('a','b','c',),),)
         '(lambda a,b,c:())'
         >>> readerless(('lambda', (':',),),)
         '(lambda :())'
         >>> readerless(('lambda', (),),)
         '(lambda :())'
 
-        The ``:`` is required if there are any paired parameters, even
+        The ``:`` is required if there are any pair parameters, even
         if there are no single parameters:
 
         >>> readerless(('lambda', (':',':**','kwargs',),),)
         '(lambda **kwargs:())'
 
         """
         fn, parameters, *body = form
         assert fn == "lambda"
-        return f"(lambda {','.join(self.parameters(parameters))}:{self.body(body)})"
+        return f"(lambda {self.parameters(parameters)}:{self.body(body)})"
 
     @_trace
-    def parameters(self, parameters: Iterable) -> Iterable[str]:
+    def parameters(self, parameters: Iterable) -> str:
         """Process parameters to compile `function`."""
         parameters = iter(parameters)
-        yield from (
+        r = [
             {":/": "/", ":*": "*"}.get(a, a)
             for a in takewhile(lambda a: a != ":", parameters)
-        )
+        ]
         for k, v in _pairs(parameters):
             if k == ":*":
-                yield "*" if v == ":?" else f"*{v}"
+                r.append("*" if v == ":?" else f"*{v}")
             elif k == ":/":
-                yield "/"
+                r.append("/")
             elif k == ":**":
-                yield f"**{v}"
+                r.append(f"**{v}")
             elif v == ":?":
-                yield k
+                r.append(k)
             else:
-                yield f"{k}={self.form(v)}"
+                r.append(f"{k}={self.form(v)}")
+        return ",".join(r)
 
     @_trace
     def body(self, body: list) -> str:
         """Compile body of `function`."""
         if len(body) > 1:
             return f"({_join_args(*map(self.form, body))})[-1]"
         if not body:
             return "()"
         result = self.form(body[0])
         return ("\n" * ("\n" in result) + result).replace("\n", "\n  ")
 
     @_trace
     def invocation(self, form: Tuple) -> str:
         """Try to compile as `macro`, else normal `call`."""
-        if (result := self.macro(form)) is not _SENTINEL:
-            return f"# {form[0]}\n{result}"
+        if (res := self.macro(form)) is not _SENTINEL:
+            if res.startswith("#") and res.lstrip("#").startswith(f" {form[0]}\n"):
+                return f"#{res}"  # Abbreviate direct recursion.
+            return f"# {form[0]}\n{res}"
         form = form[0].replace(MAYBE, "..", 1), *form[1:]
         return self.call(form)
 
     @_trace
     def macro(self, form: Tuple) -> Union[str, Sentinel]:
         """Macroexpand and start over with `form`, if it's a macro."""
         head, *tail = form
@@ -299,16 +329,16 @@
         `macro` is a run-time call.
 
         Like Python, it has three parts:
         (<callable> <args> : <kwargs>).
         For example:
 
         >>> print(readerless(
-        ... ('print',1,2,3,
-        ...          ':','sep',('quote',":",), 'end',('quote',"\n\n",),)
+        ... ('print',1,2,3
+        ...         ,':','sep',('quote',":",), 'end',('quote',"\n\n",),)
         ... ))
         print(
           (1),
           (2),
           (3),
           sep=':',
           end='\n\n')
@@ -346,50 +376,54 @@
           *[4],
           **{'sep': ':', 'end': '\n\n'})
 
         Unlike other control words, these can be repeated,
         but (as in Python) a '*' is not allowed to follow '**'.
 
         Method calls are similar to function calls:
-        (.<method name> <object> <args> : <kwargs>)
-        Like Clojure, a method on the first object is assumed if the
-        function name starts with a dot:
+        (.<method name> <self> <args> : <kwargs>)
+        A method on the self argument is assumed if the function name
+        starts with a dot:
 
         >>> readerless(('.conjugate', 1j,),)
         '(1j).conjugate()'
         >>> eval(_)
         -1j
         >>> readerless(('.decode', b'\xfffoo', ':', 'errors',('quote','ignore',),),)
         "b'\\xfffoo'.decode(\n  errors='ignore')"
         >>> eval(_)
         'foo'
 
         """
         form = iter(form)
         head = next(form)
         args = chain(
-            map(self.form, takewhile(lambda a: a != ":", form)),
-            starmap(self._pair_arg, _pairs(form)),
+            (singles := [*map(self.form, takewhile(lambda a: a != ":", form))]),
+            starmap(self._pair_arg, pairs := [*_pairs(form)]),
         )
         if type(head) is str and head.startswith("."):
-            return "{}.{}({})".format(next(args), head[1:], _join_args(*args))
+            if singles or pairs[0][0] == ":?":
+                return "{}.{}({})".format(next(args), head[1:], _join_args(*args))
+            raise CompileError("self must be paired with :?")
         return "{}({})".format(self.form(head), _join_args(*args))
 
     def _pair_arg(self, k, v):
         k = PAIR_WORDS.get(k, k + "=")
         if ".." in k:
             k = k.split(".")[-1]
         return k + self.form(v).replace("\n", "\n" + " " * len(k))
 
     @_trace
     def str(self, code: str) -> str:
         """Compile code strings.
-        Expands qualified identifiers and module literals into imports.
+        Expands qualified identifiers and module handles into imports.
         Otherwise, injects as raw Python directly into the output.
         """
+        if "..." in code:
+            return code
         if not all(s.isidentifier() for s in code.split(".") if s):
             return code
         if ".." in code:
             return self.qualified_identifier(code)
         elif code.endswith("."):
             return self.module_identifier(code)
         return code
@@ -418,28 +452,34 @@
 
         Emits a literal if possible, otherwise falls back to `pickle`:
 
         >>> readerless(-4.2j)
         '((-0-4.2j))'
         >>> print(readerless(float('nan')))
         __import__('pickle').loads(  # nan
-            b'Fnan\n.'
+            b'Fnan\n'
+            b'.'
         )
         >>> readerless([{'foo':2},(),1j,2.0,{3}])
         "[{'foo': 2}, (), 1j, 2.0, {3}]"
         >>> spam = []
         >>> spam.append(spam)  # ref cycle can't be a literal
         >>> print(readerless(spam))
         __import__('pickle').loads(  # [[...]]
-            b'(lp0\ng0\na.'
+            b'(lp0\n'
+            b'g0\n'
+            b'a.'
         )
         >>> spam = [[]] * 3  # duplicated refs
         >>> print(readerless(spam))
         __import__('pickle').loads(  # [[], [], []]
-            b'(l(lp0\nag0\nag0\na.'
+            b'(l(lp0\n'
+            b'ag0\n'
+            b'ag0\n'
+            b'a.'
         )
 
         """
         if form is Ellipsis:
             return "..."
         case = type(form)
         if case is tuple and form:
@@ -475,27 +515,39 @@
             return ast.literal_eval(literal)
 
     @_trace
     def pickle(self, form) -> str:
         """Compile to `pickle.loads`. The final fallback for `atom`."""
         # 0 is the "human-readable" backwards-compatible text protocol.
         dumps = pickletools.optimize(pickle.dumps(form, 0, fix_imports=False))
+        dumps = "\n    ".join(f"{b!r}" for b in dumps.splitlines(keepends=True))
         r = repr(form).replace("\n", "\n  # ")
         nl = "\n" if "\n" in r else ""
-        return f"__import__('pickle').loads({nl}  # {r}\n    {dumps!r}\n)"
+        return f"__import__('pickle').loads({nl}  # {r}\n    {dumps}\n)"
 
-    def eval(self, form: str) -> Tuple[str, ...]:
+    @staticmethod
+    def linenos(form):
+        lines = form.split("\n")
+        digits = len(str(len(lines)))
+        return "\n".join(f"{i:0{digits}} {line}" for i, line in enumerate(lines, 1))
+
+    def eval(self, form: str, form_number: int) -> Tuple[str, ...]:
         """Execute compiled form, but only if evaluate mode is enabled."""
         try:
             if self.evaluate:
-                exec(compile(form, "<Hissp>", "exec"), self.ns)
+                filename = (
+                    f"<Compiled Hissp #{form_number} of {self.qualname}:\n"
+                    f"{self.linenos(form)}\n"
+                    f">"
+                )
+                exec(compile(form, filename, "exec"), self.ns)
         except Exception as e:
             exc = format_exc()
             if self.ns.get("__name__") == "__main__":
-                self.abort = True
+                self.abort = exc
             else:
                 warn(
                     f"\n {e} when evaluating form:\n{form}\n\n{exc}", PostCompileWarning
                 )
             return form, "# " + exc.replace("\n", "\n# ")
         return (form,)
 
@@ -518,9 +570,10 @@
 
 def readerless(form, ns=None):
     """Compile a Hissp form to Python without evaluating it.
     Uses the current `NS` for context, unless an alternative is provided.
     (Creates a temporary namespace if neither is available.)
     Returns the Python in a string.
     """
-    ns = ns or NS.get() or {"__name__": "__main__"}
+    if ns is None and (ns := NS.get()) is None:
+        ns = {"__name__": "__main__"}
     return Compiler(evaluate=False, ns=ns).compile([form])
```

## hissp/munger.py

```diff
@@ -57,14 +57,22 @@
 
     Inputs that begin with ``:`` are assumed to be control words
     and returned unmodified.
     Full stops are handled separately, as those are meaningful to Hissp.
     """
     if s.startswith(":"):
         return s  # control word
+    return force_munge(s)
+
+
+def force_munge(s: str) -> str:
+    """As `munge`, but skips the control word check.
+
+    Used for reader tags.
+    """
     # Always normalize identifiers:
     # >>> 𝐀 = 'MATHEMATICAL BOLD CAPITAL A'
     # >>> 'A' in globals()
     # True
     s = unicodedata.normalize("NFKC", s)
     if s.isidentifier():
         return s  # Nothing to munge.
@@ -102,30 +110,31 @@
         "*": "STAR",
         "+": "PLUS",
         # COMMA is fine.
         "-": "",  # Hyphen-minus
         # Full stop reserved for imports and attributes.
         "/": "SOL",
         # Digits only munge if first character.
+        # COLON is fine.
         ";": "SEMI",
         "<": "LT",  # Less Than or LefT.
         "=": "EQ",
         ">": "GT",  # Greater Than or riGhT.
         "?": "QUERY",
         "@": "AT",
         # Capital letters are always valid in Python identifiers.
         "[": "LSQB",
         "\\": "BSOL",
         "]": "RSQB",
-        "^": "CARET",
+        "^": "HAT",
         # Underscore is valid in Python identifiers.
         "`": "GRAVE",
         # Small letters are also always valid.
         "{": "LCUB",
-        "|": "BAR",
+        "|": "VERT",
         "}": "RCUB",
         # TILDE is fine.
     }.items()
 }
 """Shorter names for Quotez."""
 
 QZ_NAME = {ord(k): ord(v) for k, v in {" ": "x", "-": "h"}.items()}
```

## hissp/reader.py

```diff
@@ -1,81 +1,99 @@
-# Copyright 2019, 2020, 2021, 2022 Matthew Egan Odendahl
+# Copyright 2019, 2020, 2021, 2022, 2023 Matthew Egan Odendahl
 # SPDX-License-Identifier: Apache-2.0
 """
 The Lissp language reader and associated helper functions.
 
-Compiles Lissp files to Python files when run as the main module.
-
 The reader is organized as a lexer and parser.
 The parser is extensible with Lissp reader macros.
 The lexer is not extensible,
 and doesn't do much more than pull tokens from a relatively simple regex
 and track its position for error messages.
 """
 
 import ast
 import builtins
+import hashlib
 import re
+from base64 import b32encode
 from collections import namedtuple
-from contextlib import contextmanager, nullcontext
+from contextlib import contextmanager, nullcontext, suppress
 from functools import reduce
 from importlib import import_module, resources
 from itertools import chain, takewhile
 from keyword import iskeyword as _iskeyword
 from pathlib import Path, PurePath
 from pprint import pformat
 from threading import Lock
-from typing import Any, Iterable, Iterator, NewType, Optional, Tuple, Union
+from typing import Any, Iterable, Iterator, NewType, Optional, Tuple, Union, List
+
+import hissp.compiler as C
+from hissp.compiler import Compiler, readerless
+from hissp.munger import force_munge, force_qz_encode, munge
+
+GENSYM_BYTES = 5
+"""
+The number of bytes gensym `$# <parse_macro>` hashes have.
+
+The default 5 bytes (40 bits) should be more than sufficient space to
+eliminate collisions with typical usage, but for unusual applications,
+hash length can be increased, up to a maximum of 32 bytes.
+(16 would have more space than a `uuid.uuid4`.)
 
-from hissp.compiler import Compiler, MAYBE, readerless
-from hissp.munger import force_qz_encode, munge
+Each hash character encodes 5 bits (base32 encoding), so 40-bit hashes
+typically take 8 characters.
+"""
 
 ENTUPLE = ("lambda",(":",":*"," _")," _",)  # fmt: skip
 """
 Used by the template macro to make tuples.
 
 To avoid creating a dependency on Hissp, by default,
 templates spell out the entuple implementation every time,
 but you can override this by setting some other value here.
 """
 
 TOKENS = re.compile(
     r"""(?x)
-     (?P<comment>;.*)
-    |(?P<whitespace>[\n ]+)
+     (?P<whitespace>[\n ]+)
+    |(?P<comment>(?:[ ]*;.*[\n])+)
     |(?P<badspace>\s)  # Other whitespace not allowed.
     |(?P<open>\()
     |(?P<close>\))
     |(?P<macro>
        ,@
       |['`,!]
-       # Any atom that ends in (an unescaped) ``#``
-      |(?:[^\\ \n"();#]|\\.)+[#]
+      |[.][#]
+      # Any atom that ends in ``#``, but not ``.#`` or ``\#``.
+      |(?:[^\\ \n"();#]|\\.)*(?:[^.\\ \n"();#]|\\.)[#]
      )
     |(?P<string>
       [#]?  # raw?
       "  # Open quote.
         (?:[^"\\]  # Any non-magic character.
            |\\(?:.|\n)  # Backslash only if paired, including with newline.
         )*  # Zero or more times.
       "  # Close quote.
      )
-    |(?P<continue>[#]?")  # String not closed.
+    |(?P<continue>
+       [#]?"  # String not closed.
+      |;.*  # Comment may need another line.
+     )
     |(?P<atom>(?:[^\\ \n"();]|\\.)+)  # Let Python deal with it.
     |(?P<error>.)
     """
 )
 
 Token = NewType("Token", Tuple[str, str, int])
 
 DROP = object()
 """
 The sentinel value returned by the discard macro ``_#``, which the
 reader skips over when parsing. Reader macros can have read-time side
-effects with no Hissp output by returning this.
+effects with no Hissp output by returning this. (Not recommended.)
 """
 
 
 class SoftSyntaxError(SyntaxError):
     """A syntax error that could be corrected with more lines of input.
 
     When the REPL encounters this when attempting to evaluate a form,
@@ -120,28 +138,56 @@
         good = self.code[0:pos].split("\n")
         lineno = len(good)
         offset = len(good[-1])
         return self.file, lineno, offset, self.code.split("\n")[lineno - 1]
 
 
 _Unquote = namedtuple("_Unquote", ["target", "value"])
-Comment = namedtuple("Comment", ["content"])
+
+
+class Comment:
+    """Parsed object for a comment token (line comment block).
+
+    The reader normally discards these, but reader macros can use them.
+    """
+
+    def __init__(self, token):
+        self.token = token
+
+    def contents(self):
+        """Gets the comment text inside the comment token.
+
+        Strips any leading indent, the ``;`` character(s), and up to one
+        following space for each line in the comment block.
+        """
+        return re.sub(r"(?m)\n$|^ *;+ ?", "", self.token)
+
+    def __repr__(self):
+        return f"Comment({self.token!r})"
 
 
 class Extra(tuple):
-    """Designates Extra read-time arguments for reader macros."""
+    """Designates Extra read-time arguments for reader macros.
+
+    Normally made with the ``!`` macro, but can be constructed directly.
+    """
 
     def __repr__(self):
         return f"Extra({list(self)!r})"
 
 
-def gensym_counter(_count=[0], _lock=Lock()):
+def gensym_counter(_count=[0], _lock=Lock()) -> int:
     """
     Call to increment the gensym counter, and return the new count.
     Used by the gensym reader macro ``$#`` to ensure symbols are unique.
+
+    Uses a `threading.Lock` to ensure a number is not allocated more
+    than once in a session, however builds may not be reproducible if
+    templates are allocated numbers in a nondeterministic order,
+    therefore reading gensyms with multiple threads is not recommended.
     """
     with _lock:
         _count[0] += 1
         return _count[0]
 
 
 class Lissp:
@@ -162,15 +208,16 @@
         self.qualname = qualname
         self.compiler = Compiler(self.qualname, ns, evaluate)
         self.filename = filename
         self.reinit()
 
     def reinit(self):
         """Reset position, nesting depth, and gensym stack."""
-        self.gensym_stack = []
+        self.counters: List[int] = []
+        self.context = []
         self.depth = []
         self._p = 0
 
     @property
     def ns(self):
         """The wrapped `Compiler`'s ``ns``."""
         return self.compiler.ns
@@ -182,14 +229,17 @@
     def compile(self, code: str) -> str:
         """Read Lissp code and pass it on to the Hissp compiler."""
         hissp = self.reads(code)
         return self.compiler.compile(hissp)
 
     def reads(self, code: str) -> Iterable:
         """Read Hissp forms from code string."""
+        self.blake = hashlib.blake2s(digest_size=GENSYM_BYTES)
+        self.blake.update(code.encode())
+        self.blake.update(self.ns.get("__name__", "__main__").encode())
         res: Iterable[object] = self.parse(Lexer(code, self.filename))
         self.reinit()
         return res
 
     def parse(self, tokens: Lexer) -> Iterator:
         """Build Hissp forms from a `Lexer`."""
         self.tokens = tokens
@@ -198,15 +248,15 @@
     def _filter_drop(self):
         return (x for x in self._parse() if x is not DROP)
 
     def _parse(self) -> Iterator:
         for k, v, self._p in self.tokens:
             # fmt: off
             if k == "whitespace": continue
-            elif k == "comment":  yield Comment(v[1:])
+            elif k == "comment":  yield Comment(v)
             elif k == "badspace": raise self._badspace(v)
             elif k == "open":     yield from self._open()
             elif k == "close":    return self._close()
             elif k == "macro":    yield from self._macro(v)
             elif k == "string":   yield self._string(v)
             elif k == "continue": raise self._continue()
             elif k == "atom":     yield self.atom(v)
@@ -244,31 +294,32 @@
             ",@": self.unquote_context,
         }.get(v, nullcontext)():
             yield self.parse_macro(v, *self._extras(p, v))
 
     @contextmanager
     def gensym_context(self):
         """Start a new gensym context for the current template."""
-        self.gensym_stack.append(gensym_counter())
+        self.counters.append(gensym_counter())
+        self.context.append("`")
         try:
             yield
         finally:
-            self.gensym_stack.pop()
+            self.counters.pop()
+            self.context.pop()
 
     @contextmanager
     def unquote_context(self):
         """Start a new unquote context for the current template."""
-        try:
-            gensym_number = self.gensym_stack.pop()
-        except IndexError:
+        self.context.append(",")
+        if self.context.count(",") > self.context.count("`"):
             raise SyntaxError("Unquote outside of template.", self.position()) from None
         try:
             yield
         finally:
-            self.gensym_stack.append(gensym_number)
+            self.context.pop()
 
     def _extras(self, p, v):
         extras = []
         depth = len(self.depth)
         nondrop = self._filter_drop()
         try:
             while isinstance(form := next(nondrop), Extra):
@@ -276,15 +327,46 @@
         except StopIteration:
             e = SoftSyntaxError if len(self.depth) == depth else SyntaxError
             raise e(f"Reader macro {v!r} missing argument.", self.position(p)) from None
         return form, extras
 
     def parse_macro(self, tag: str, form, extras):
         # fmt: off
-        """Apply a reader macro to a form."""
+        R"""Apply a reader macro to a form.
+
+        The built-in reader macros are handled here. They are
+
+        .. list-table::
+
+           * - ``'``
+             - `quote<special>`
+           * - ``!``
+             - `Extra`
+           * - :literal:`\`` (backtick)
+             - template quote (starts a `template`)
+           * - ``_#``
+             - `discard<DROP>`
+           * - ``.#``
+             - inject (evaluate at read time and use resulting object)
+
+        Plus the three built-in template helper macros, which are only
+        valid inside a template.
+
+        .. list-table::
+
+           * - ``,``
+             - unquote
+           * - ``,@``
+             - splice unquote
+           * - ``$#``
+             - `gensym`
+
+        The built-in macros are reserved by the reader and cannot be
+        reassigned.
+        """
         def case(s):
             if (b := tag == s) and extras:
                 raise SyntaxError(f"Extra for {s!r} reader macro.")
             return b
         if case("'"):  return "quote", form
         if tag == "!": return Extra([*extras, form])
         if case("`"):  return self.template(form)
@@ -295,15 +377,15 @@
         if case(".#"): return eval(readerless(form, self.ns), self.ns)
         return self._custom_macro(form, tag, extras)
         # fmt: on
 
     def template(self, form):
         """Process form as template."""
         case = type(form)
-        if is_string(form):
+        if is_lissp_string(form):
             return "quote", form
         if case is tuple and form:
             return (ENTUPLE, ":", *chain(*self._template(form)),)  # fmt: skip
         if case is str and not form.startswith(":"):
             return "quote", self.qualify(form)
         if case is _Unquote and form.target == ":?":
             return form.value
@@ -323,60 +405,74 @@
                 yield ":?", form
             invocation = False
 
     def qualify(self, symbol: str, invocation=False) -> str:
         """Qualify symbol based on current context."""
         if not is_qualifiable(symbol):
             return symbol
-        if invocation and "_macro_" in self.ns and self._macro_has(symbol):
-            return f"{self.qualname}.._macro_.{symbol}"  # Known macro.
+        if invocation and C.MACROS in self.ns and hasattr(self.ns[C.MACROS], symbol):
+            return f"{self.qualname}..{C.MACROS}.{symbol}"  # Known macro.
         if symbol in dir(builtins) and symbol.split(".", 1)[0] not in self.ns:
             return f"builtins..{symbol}"  # Known builtin, not shadowed (yet).
         if invocation and "." not in symbol:  # Could still be a recursive macro.
-            return f"{self.qualname}{MAYBE}{symbol}"
+            return f"{self.qualname}{C.MAYBE}{symbol}"
         return f"{self.qualname}..{symbol}"
 
-    def _macro_has(self, symbol):
-        # The _macro_ interface is not required to implement
-        # __contains__ or __dir__ and exotic _macro_ objects might
-        # override __getattribute__. The only way to tell if _macro_ has
-        # a name is getattr().
-        try:
-            getattr(self.ns["_macro_"], symbol)
-        except AttributeError:
-            return False
-        return True
-
     def gensym(self, form: str):
-        """Generate a symbol unique to the current template."""
-        try:
-            return f"_{munge(form)}_QzNo{self.gensym_stack[-1]}_"
-        except IndexError:
+        """Generate a symbol unique to the current template.
+        Re-munges any $'s as a gensym hash, or adds it as a prefix if
+        there aren't any. Gensym hashes are deterministic for
+        reproducible builds. Inputs are the code string being read,
+        the current `__name__` (defaults to "__main__" if not found)
+        and a `count<gensym_counter>` of templates read so far.
+        """
+        blk = self.blake.copy()
+        blk.update((c := self._get_counter()).to_bytes(1 + c.bit_length() // 8, "big"))
+        prefix = f"_Qz{b32encode(blk.digest()).rstrip(b'=').decode()}z_"
+        marker = munge("$")
+        if marker not in form:
+            return f"{prefix}{(form)}"
+        # TODO: escape $'s somehow? $$? \$?
+        return form.replace(marker, prefix)
+
+    def _get_counter(self) -> int:
+        index = self.context.count("`") - self.context.count(",")
+        if not self.context or index < 0:
             raise SyntaxError("Gensym outside of template.", self.position()) from None
+        if self.context[-1] == "`":
+            return self.counters[-1]
+        return self.counters[index]
 
     def _custom_macro(self, form, tag, extras):
         assert tag.endswith("#")
-        tag = munge(self.escape(tag[:-1]))
-        if ".." in tag:
-            module, function = tag.split("..", 1)
-            m = reduce(getattr, function.split("."), import_module(module))
-        else:
-            try:
-                m = getattr(self.ns["_macro_"], tag + munge("#"))
-            except (AttributeError, KeyError):
-                raise SyntaxError(f"Unknown reader macro {tag!r}.", self.position())
+        tag = force_munge(self.escape(tag[:-1]))
+        tag = re.sub(r"(^\.)", lambda m: force_qz_encode(m[1]), tag)
+        m = (self._fully_qualified if ".." in tag else self._local)(tag)
         with self.compiler.macro_context():
-            args, kwargs = _parse_extras(extras)
+            args, kwargs = parse_extras(extras)
             return m(form, *args, **kwargs)
 
+    def _fully_qualified(self, tag):
+        module, function = tag.split("..", 1)
+        if re.match(rf"{C.MACROS}\.[^.]+$", function):
+            function += munge("#")
+        return reduce(getattr, function.split("."), import_module(module))
+
+    def _local(self, tag):
+        try:
+            return getattr(self.ns[C.MACROS], tag + munge("#"))
+        except (AttributeError, KeyError):
+            raise SyntaxError(f"Unknown reader macro {tag!r}.", self.position())
+
     @staticmethod
     def escape(atom):
         """Process the backslashes in a token."""
-        atom = atom.replace(r"\.", force_qz_encode("."))
-        return re.sub(r"\\(.)", lambda m: m[1], atom)
+        return re.sub(
+            r"\\(.)", lambda m: force_qz_encode(m[1]) if m[1] in ".:" else m[1], atom
+        )
 
     @staticmethod
     def _string(v):
         if v[0] == "#":  # Let Python process escapes.
             v = v.replace("\\\n", "").replace("\n", R"\n")
             val = ast.literal_eval(v[1:])
         else:  # raw
@@ -391,15 +487,15 @@
         """Preprocesses atoms. Handles escapes and munging."""
         is_symbol = "\\" == v[0]
         v = Lissp.escape(v)
         if is_symbol:
             return munge(v)
         try:
             val = ast.literal_eval(v)
-            if isinstance(val, bytes):  # bytes have their own literals.
+            if isinstance(val, (bytes, dict, list, set, tuple)):
                 return munge(v)
             return val
         except (ValueError, SyntaxError):
             return munge(v)
 
     def _error(self, k):
         assert k == "error", f"unknown token: {k!r}"
@@ -408,34 +504,54 @@
     def _check_depth(self):
         if self.depth:
             raise SoftSyntaxError(
                 "This form is missing a `)`.", self.position(self.depth.pop())
             )
 
 
-def is_string(form):
+def is_hissp_string(form) -> bool:
+    """Determines if form would directly represent a string in Hissp.
+
+    Allows "readerless mode"-style strings: ('quote','foo',)
+    and any string literal in a Hissp-level str: '"foo"'
+    (including the "('foo')" form produced by the Lissp reader).
+
+    Macros often produce strings in one of these forms, via ``'`` or
+    `repr` on a string object.
+    """
+    return (
+        type(form) is tuple
+        and len(form) == 2
+        and form[0] == "quote"
+        and type(form[1]) is str
+    ) or bool(is_string_literal(form))
+
+
+def is_lissp_string(form) -> bool:
     """
     Determines if form could have been read from a Lissp string literal.
 
     It's not enough to check if the form has a string type.
     Several token types such as control words, symbols, and Python
     injections, read in as strings. Macros may need to distinguish these
     cases.
     """
-    try:
-        return (
-            type(form) is str
-            and form.startswith("(")
-            and type(ast.literal_eval(form)) is str
-        )
-    except:
-        return False
+    return type(form) is str and form.startswith("(") and bool(is_string_literal(form))
+
+
+def is_string_literal(form) -> Optional[bool]:
+    """Determines if `ast.literal_eval` on form produces a string.
+
+    False if it produces something else or None if it raises Exception.
+    """
+    with suppress(Exception):
+        return type(ast.literal_eval(form)) is str
 
 
-def _parse_extras(extras):
+def parse_extras(extras):
     it = iter(extras)
     args = [*takewhile(lambda x: x != ":", it)]
     kwargs = {}
     for k in it:
         # fmt: off
         v = next(it)
         if k == ":?":    args.append(v)
@@ -445,22 +561,22 @@
         # fmt: on
     return args, kwargs
 
 
 def is_qualifiable(symbol):
     """Determines if symbol can be qualified with a module.
 
-    Can't be ``quote``, ``__import__``, any Python reserved word, an
-    auto-gensym, already qualified, method syntax, or a module literal;
-    and must be a valid identifier or attribute identifier.
+    Can't be ``quote``, ``__import__``, any Python reserved word, a
+    prefix auto-gensym, already qualified, method syntax, or a module
+    handle; and must be a valid identifier or attribute identifier.
     """
     return (
         symbol not in {"quote", "__import__"}
         and not _iskeyword(symbol)
-        and not re.match(r".*_QzNo\d+_$", symbol)
+        and not re.match(r"_Qz[A-Z2-7]+z_", symbol)
         and all(map(str.isidentifier, symbol.split(".")))
     )
 
 
 def transpile(package: Optional[str], *modules: str):
     """Transpiles the named Python modules from Lissp.
 
@@ -482,14 +598,14 @@
 
 def transpile_file(path: Union[Path, str], package: Optional[str] = None):
     """Transpiles a single .lissp file to .py in the same location.
 
     Code in .lissp files is executed upon compilation. This is necessary
     because macro definitions can alter the compilation of subsequent
     top-level forms. A packaged Lissp file must know its package at
-    compile time to resolve imports correctly.
+    compile time to handle templates and macros correctly.
     """
     path = Path(path).resolve(strict=True)
     qualname = f"{package or ''}{'.' if package else ''}{PurePath(path.name).stem}"
     L = Lissp(qualname=qualname, evaluate=True, filename=str(path))
     python = L.compile(re.sub(r"^#!.*\n", "", path.read_text("utf8")))
     path.with_suffix(".py").write_text(python, "utf8")
```

## hissp/repl.py

```diff
@@ -5,38 +5,38 @@
 """
 
 import sys
 from code import InteractiveConsole
 from contextlib import suppress
 from types import ModuleType, SimpleNamespace
 
-import hissp.basic
 from hissp.compiler import CompileError
 from hissp.reader import Lissp, SoftSyntaxError
 
 
 ps1 = "#> "
-"""String specifying the primary prompt of the REPL."""
+"""String specifying the primary prompt of the `LisspREPL`."""
 
 
 ps2 = "#.."
-"""String specifying the secondary (continuation) prompt of the REPL."""
+"""String specifying the secondary (continuation) prompt of the `LisspREPL`."""
 
 
 class LisspREPL(InteractiveConsole):
     """Lissp's Read-Evaluate-Print Loop, layered on Python's.
 
     You can initialize the REPL with a locals dict,
     which is useful for debugging other modules.
     Call interact() to start.
     """
 
+    # locals shadows the builtin, but that's the name in the superclass.
     def __init__(self, locals=None, filename="<console>"):
         super().__init__(locals, filename)
-        self.lissp = Lissp(ns=locals)
+        self.lissp = Lissp(locals.get("__name__", "__main__"), locals)
         self.locals = self.lissp.ns
 
     def runsource(self, source, filename="<input>", symbol="single"):
         """:meta private:"""
         try:
             self.lissp.filename = filename
             source = self.lissp.compile(source)
@@ -50,41 +50,61 @@
             self.showsyntaxerror()
             return False
         except BaseException:
             print(f"{sys.ps1}# Compilation failed!", file=sys.stderr)
             self.showtraceback()
             return False
         print(sys.ps1, source.replace("\n", f"\n{sys.ps2}"), sep="", file=sys.stderr)
-        return super().runsource(source, filename, symbol)
+        fn = f"<Compiled Hissp of {filename}:\n{self.lissp.compiler.linenos(source)}\n>"
+        return super().runsource(source, fn, symbol)
 
     def raw_input(self, prompt=""):
         """:meta private:"""
         prompt = {sys.ps2: ps2, sys.ps1: ps1}.get(prompt, prompt)
         return super().raw_input(prompt)
 
     def interact(self, banner=None, exitmsg=None):
         """Imports readline if available, then super().interact()."""
         with suppress(ImportError):
             # noinspection PyUnresolvedReferences
             import readline
         return super().interact(banner, exitmsg)
 
 
+def interact(locals=None):
+    """Convenience function to start a `LisspREPL`.
+
+    Uses the calling frame's globals and locals as ``locals`` if not
+    provided.
+
+    Unlike `hissp.repl.main`, no ``_macros_`` are added to the locals to
+    avoid clobbering an existing namespace.
+    """
+    if locals is None:
+        import inspect
+
+        frame = inspect.currentframe().f_back
+        locals = {**frame.f_globals, **frame.f_locals}
+    LisspREPL(locals=locals).interact()
+
+
 def force_main():
     """:meta private:"""
+    # Creates a new ``__main__`` to take the place of the current
+    # ``__main__`` module.
     __main__ = ModuleType("__main__")
     sys.modules["__main__"] = __main__
     sys.path.insert(0, "")
     return __main__
 
 
-def main(__main__=None):
-    """REPL command-line entry point."""
-    if not __main__:
-        __main__ = force_main()
-    repl = LisspREPL(locals=__main__.__dict__)
-    repl.locals["_macro_"] = SimpleNamespace(**vars(hissp.basic._macro_))
-    repl.interact()
+def main(__main__):
+    """REPL command-line entry point.
 
+    `hissp.macros._macro_` is copied into the module namespace,
+    making the bundled macros immediately available unqualified.
+    """
+    repl = LisspREPL(locals=__main__.__dict__)
+    import hissp.macros  # Here so repl can import before compilation.
 
-if __name__ == "__main__":
-    main()
+    repl.locals["_macro_"] = SimpleNamespace(**vars(hissp.macros._macro_))
+    repl.interact()
```

## Comparing `hissp-0.3.0.dist-info/LICENSE.txt` & `hissp-0.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hissp-0.3.0.dist-info/RECORD` & `hissp-0.4.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-hissp/__init__.py,sha256=scUeCd1GoUYXMI7b5RAfAHJVERSF4e3rEYRVyMA4eJo,807
-hissp/__main__.py,sha256=RBgXQ5fC46o0kAkdfDOfNG-uJA45hNA7bEEG5oGlDIs,1881
-hissp/basic.lissp,sha256=QzcqUI3htnrZmMs6j9N6MW9b_wwS57EsXOXKI3UC-CE,16661
-hissp/basic.py,sha256=xO6NU-2e5TUmi3hSyPfyUbht8NOHGIBxIZliwiSwrWg,43218
-hissp/compiler.py,sha256=d38CkPKYHWg5rBWkLgTf5F0wFluADbFc_GjVMuBpi9g,16919
-hissp/munger.py,sha256=OwkS0U4wOKGBXjup-Z8dE0XH1O-nau2SdC41BmaxYxA,5698
-hissp/reader.py,sha256=crTpboWVAF5KdCvrAcKDthuu4r6uI80k_eKIY47RZ24,16481
-hissp/repl.py,sha256=gpS8soKKcJ3aWdXjiEI0733rGlejO84VtmVDqRbBkfM,2703
-hissp-0.3.0.dist-info/LICENSE.txt,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hissp-0.3.0.dist-info/METADATA,sha256=CgXIXqCBSID7M0eOCI_MI3uwyDByr_BMAI3EtuD6hjo,18637
-hissp-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-hissp-0.3.0.dist-info/entry_points.txt,sha256=NNdJ8cOarw_M804B7AfAYslz5He6EEf6s0tHvojAe94,47
-hissp-0.3.0.dist-info/top_level.txt,sha256=AudQVCWV320G1jGMPjyRmMhcop5FEBodfNyc65R_bh0,6
-hissp-0.3.0.dist-info/RECORD,,
+hissp/__init__.py,sha256=hvA92IW9F7ta6fKGI1TSEbC-a4b2WtgZfcfaexBNuFo,2520
+hissp/__main__.py,sha256=m6mQINawIm2qGRtF-fVpRTluAyOpsFmugXndzZf3dSg,1927
+hissp/compiler.py,sha256=Nr5NLESeubpbsowiyuj1m8hbd1y4PmRsZvET4GgMXnQ,18896
+hissp/macros.lissp,sha256=qjqZr1m89I3L7jZsd02wWkcLUezrTq3e53xkA0e_pWw,96125
+hissp/macros.py,sha256=THPI9O8qHLttnS4L4UBK5l2vPhpym-ilL8J45rYMidA,257822
+hissp/munger.py,sha256=2tV5DqtzK3smibU04YOLo4r_04ZhfmUgC0FaIgFtYes,5870
+hissp/reader.py,sha256=9zf13jW7v5ryR_g4QzFcoiJUt0j1sW7BtG_Xz1mxo1o,20531
+hissp/repl.py,sha256=y3RPdCTbeqnGKIeLzMAs1HyjMmpumh0wNKDz2NTHpEA,3569
+hissp-0.4.0.dist-info/LICENSE.txt,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hissp-0.4.0.dist-info/METADATA,sha256=A_1-dMq4V2VNiVw_Rwy7uQJg64t-1jaKYZbzI4kVc0o,28422
+hissp-0.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hissp-0.4.0.dist-info/entry_points.txt,sha256=vUC6DOnH6JWU26asY7EA9Wb03-UuP1bz48pni8uK-Mc,46
+hissp-0.4.0.dist-info/top_level.txt,sha256=AudQVCWV320G1jGMPjyRmMhcop5FEBodfNyc65R_bh0,6
+hissp-0.4.0.dist-info/RECORD,,
```

