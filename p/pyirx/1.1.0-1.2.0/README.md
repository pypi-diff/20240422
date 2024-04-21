# Comparing `tmp/pyirx-1.1.0.tar.gz` & `tmp/pyirx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirx-1.1.0.tar", max compression
+gzip compressed data, was "pyirx-1.2.0.tar", max compression
```

## Comparing `pyirx-1.1.0.tar` & `pyirx-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     1498 2024-03-24 23:49:25.930678 pyirx-1.1.0/LICENSE
--rw-r--r--   0        0        0      524 2024-03-24 23:49:25.930678 pyirx-1.1.0/docs/index.md
--rw-r--r--   0        0        0     2125 2024-03-24 23:50:39.146569 pyirx-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      149 2024-03-24 23:50:39.146569 pyirx-1.1.0/src/irx/__init__.py
--rw-r--r--   0        0        0     1652 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/ast/__init__.py
--rw-r--r--   0        0        0     1016 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/ast/blocks.py
--rw-r--r--   0        0        0       32 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/builders/__init__.py
--rw-r--r--   0        0        0     4780 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/builders/base.py
--rw-r--r--   0        0        0    27537 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/builders/llvmliteir.py
--rw-r--r--   0        0        0      739 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/builders/symbol_table.py
--rw-r--r--   0        0        0        0 2024-03-24 23:49:25.934678 pyirx-1.1.0/src/irx/py.typed
--rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 pyirx-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-04-21 22:03:17.092317 pyirx-1.2.0/LICENSE
+-rw-r--r--   0        0        0      518 2024-04-21 22:03:17.092317 pyirx-1.2.0/docs/index.md
+-rw-r--r--   0        0        0     2126 2024-04-21 22:04:29.871634 pyirx-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-04-21 22:04:29.871634 pyirx-1.2.0/src/irx/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/base.py
+-rw-r--r--   0        0        0    27549 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/llvmliteir.py
+-rw-r--r--   0        0        0      739 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/symbol_table.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:03:17.096317 pyirx-1.2.0/src/irx/py.typed
+-rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 pyirx-1.2.0/PKG-INFO
```

### Comparing `pyirx-1.1.0/LICENSE` & `pyirx-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyirx-1.1.0/docs/index.md` & `pyirx-1.2.0/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 **ASTx** is a generic project that offers a way to compound in an expressive way
 an **AST**. It is not specific for the **ArxLang** project, although it is main
 focus is to provide all needed feature for it.
 
 **IRx** uses **llvmlite** in order to generate **LLVM-IR** source.
 
 - Software License: BSD 3 Clause
-- Documentation: https://irx.arxlang.github.io.
+- Documentation: https://irx.arxlang.org.
 
 ## Features
 
 - Generate **LLVM-IR** from **ASTx**.
```

### Comparing `pyirx-1.1.0/pyproject.toml` & `pyirx-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyirx"
-version = "1.1.0"  # semantic-release
+version = "1.2.0"  # semantic-release
 description = "IRx"
 readme = "docs/index.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 exclude = [
   ".git/*",
   ".env*",
@@ -13,15 +13,15 @@
   {include = "irx", from="src"},
 ]
 include = ["src/irx/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 atpublic = ">=4.0"
-astx = ">=0.9"
+astx = "0.11.*"
 typing-extensions = { version = "^4", python = "<3.9" }
 llvmlite = ">=0.41.1"
 plum-dispatch = ">=2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.2"
 pytest-cov = ">=4.1.0"
@@ -32,15 +32,15 @@
 bandit = ">=1.7.5"
 vulture = ">=2.9.1"
 mccabe = ">=0.6.1"
 ipython = ">=7"
 ipykernel = ">=6.0.0"
 mkdocs = ">=1.4.3"
 mkdocs-exclude = ">=1.0.2"
-mkdocs-jupyter = ">=0.24.1"
+mkdocs-jupyter = ">=0.24.7"
 mkdocs-literate-nav = ">=0.6.0"
 mkdocs-macros-plugin = ">=0.7.0,<1"
 mkdocs-material = ">=9.1.15"
 mkdocstrings = ">=0.21.2"
 mkdocstrings-python = ">=1.1.2"
 makim = "1.14.0"
 pdbpp = ">=0.10.3"
```

### Comparing `pyirx-1.1.0/src/irx/builders/base.py` & `pyirx-1.2.0/src/irx/builders/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,110 +4,110 @@
 
 import os
 import sys
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict
 
-from plum import dispatch
+import astx
 
-from irx import ast
+from plum import dispatch
 
 
 class BuilderVisitor:
     """Builder translator visitor."""
 
-    def translate(self, expr: ast.AST) -> str:
+    def translate(self, expr: astx.AST) -> str:
         """
         Translate an ASTx expression to string.
 
         Example of how it could be implemented:
 
             self.visit(expr)
             return str(self.result)
         """
         raise Exception("Not implemented yet.")
 
     @dispatch.abstract
-    def visit(self, expr: ast.AST) -> None:
+    def visit(self, expr: astx.AST) -> None:
         """Translate an ASTx expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.FunctionCall) -> None:
+    def visit(self, expr: astx.FunctionCall) -> None:
         """Translate an ASTx FunctionCall expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Function) -> None:
+    def visit(self, expr: astx.Function) -> None:
         """Translate an ASTx Function expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.FunctionPrototype) -> None:
+    def visit(self, expr: astx.FunctionPrototype) -> None:
         """Translate an ASTx FunctionPrototype expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.FunctionReturn) -> None:
+    def visit(self, expr: astx.FunctionReturn) -> None:
         """Translate an ASTx FunctionReturn expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.InlineVariableDeclaration) -> None:
+    def visit(self, expr: astx.InlineVariableDeclaration) -> None:
         """Translate an ASTx InlineVariableDeclaration expression."""
         raise Exception("InlineVariableDeclaration not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.LiteralInt32) -> None:
+    def visit(self, expr: astx.LiteralInt32) -> None:
         """Translate an ASTx LiteralInt32 expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.ForCountLoop) -> None:
+    def visit(self, expr: astx.ForCountLoop) -> None:
         """Translate an ASTx ForCountLoop expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.ForRangeLoop) -> None:
+    def visit(self, expr: astx.ForRangeLoop) -> None:
         """Translate an ASTx ForRangeLoop expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.If) -> None:
+    def visit(self, expr: astx.If) -> None:
         """Translate an ASTx If expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.BinaryOp) -> None:
+    def visit(self, expr: astx.BinaryOp) -> None:
         """Translate an ASTx BinaryOp expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.UnaryOp) -> None:
+    def visit(self, expr: astx.UnaryOp) -> None:
         """Translate an ASTx UnaryOp expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Block) -> None:
+    def visit(self, expr: astx.Block) -> None:
         """Translate an ASTx Block expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Module) -> None:
+    def visit(self, expr: astx.Module) -> None:
         """Translate an ASTx Module expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Variable) -> None:
+    def visit(self, expr: astx.Variable) -> None:
         """Translate an ASTx Variable expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.VariableDeclaration) -> None:
+    def visit(self, expr: astx.VariableDeclaration) -> None:
         """Translate an ASTx VariableDeclaration expression."""
         raise Exception("Not implemented yet.")
 
 
 class Builder(ABC):
     """ASTx Builder."""
 
@@ -126,26 +126,26 @@
             _in=sys.stdin,
             _out=sys.stdout,
             _err=sys.stderr,
             _env=os.environ,
             # _new_session=True,
         )
 
-    def module(self) -> ast.Module:
+    def module(self) -> astx.Module:
         """Create a new ASTx Module."""
-        return ast.Module()
+        return astx.Module()
 
-    def translate(self, expr: ast.AST) -> str:
+    def translate(self, expr: astx.AST) -> str:
         """Transpile ASTx to LLVM-IR."""
         return self.translator.translate(expr)
 
     @abstractmethod
     def build(
         self,
-        expr: ast.AST,
+        expr: astx.AST,
         output_file: str,  # noqa: F841, RUF100
     ) -> None:
         """Transpile ASTx to LLVM-IR and build an executable file."""
         ...
 
     @abstractmethod
     def run(self) -> None:
```

### Comparing `pyirx-1.1.0/src/irx/builders/llvmliteir.py` & `pyirx-1.2.0/src/irx/builders/llvmliteir.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from __future__ import annotations
 
 import subprocess
 import tempfile
 
 from typing import Any, Optional, cast
 
+import astx
 import sh
 
 from llvmlite import binding as llvm
 from llvmlite import ir
 from plum import dispatch
 from public import public
 
-from irx import ast
 from irx.builders.base import Builder, BuilderVisitor
 
 
 def run_command(command: list[str]) -> None:
     """Run a command in the operating system."""
     try:
         subprocess.run(command, check=True)
@@ -80,33 +80,33 @@
 class LLVMLiteIRVisitor(BuilderVisitor):
     """LLVM-IR Translator."""
 
     # AllocaInst
     named_values: dict[str, Any] = {}  # noqa: RUF012
     _llvm: VariablesLLVM
 
-    function_protos: dict[str, ast.FunctionPrototype]
+    function_protos: dict[str, astx.FunctionPrototype]
     result_stack: list[ir.Value | ir.Function] = []  # noqa: RUF012
 
     def __init__(self) -> None:
         """Initialize LLVMTranslator object."""
         super().__init__()
-        self.function_protos: dict[str, ast.FunctionPrototype] = {}
+        self.function_protos: dict[str, astx.FunctionPrototype] = {}
         self.result_stack: list[ir.Value | ir.Function] = []
 
         self.initialize()
 
         self.target = llvm.Target.from_default_triple()
         self.target_machine = self.target.create_target_machine(
             codemodel="small"
         )
 
         self._add_builtins()
 
-    def translate(self, expr: ast.AST) -> str:
+    def translate(self, expr: astx.AST) -> str:
         """Translate an ASTx expression to string."""
         self.visit(expr)
         return str(self._llvm.module)
 
     def initialize(self) -> None:
         """Initialize self."""
         # self._llvm.context = ir.context.Context()
@@ -200,32 +200,32 @@
         alloca = self._llvm.ir_builder.alloca(
             self._llvm.get_data_type(type_name), None, var_name
         )
         self._llvm.ir_builder.position_at_end(self._llvm.ir_builder.block)
         return alloca
 
     @dispatch.abstract
-    def visit(self, expr: ast.AST) -> None:
+    def visit(self, expr: astx.AST) -> None:
         """Translate an ASTx expression."""
         raise Exception("Not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.BinaryOp) -> None:
+    def visit(self, expr: astx.BinaryOp) -> None:
         """Translate binary operation expression."""
         if expr.op_code == "=":
             # Special case '=' because we don't want to emit the lhs as an
             # expression.
             # Assignment requires the lhs to be an identifier.
             # This assumes we're building without RTTI because LLVM builds
             # that way by default.
             # If you build LLVM with RTTI, this can be changed to a
             # dynamic_cast for automatic error checking.
             var_lhs = expr.lhs
 
-            if not isinstance(var_lhs, ast.VariableExprAST):
+            if not isinstance(var_lhs, astx.VariableExprAST):
                 raise Exception("destination of '=' must be a variable")
 
             # Codegen the rhs.
             self.visit(expr.rhs)
             llvm_rhs = safe_pop(self.result_stack)
 
             if not llvm_rhs:
@@ -307,28 +307,28 @@
                 )
             self.result_stack.append(result)
             return
 
         raise Exception(f"Binary op {expr.op_code} not implemented yet.")
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, block: ast.Block) -> None:
+    def visit(self, block: astx.Block) -> None:
         """Translate ASTx Block to LLVM-IR."""
         result = []
         for node in block.nodes:
             self.visit(node)
             try:
                 result.append(self.result_stack.pop())
             except IndexError:
                 # some nodes doesn't add anything in the stack
                 pass
         self.result_stack.append(result)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.If) -> None:
+    def visit(self, expr: astx.If) -> None:
         """Translate IF statement."""
         self.visit(expr.cond)
         cond_v = self.result_stack.pop()
 
         if not cond_v:
             raise Exception("codegen: Invalid condition expression.")
 
@@ -389,15 +389,15 @@
 
         phi.add_incoming(then_v, then_bb)
         phi.add_incoming(else_v, else_bb)
 
         self.result_stack.append(phi)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.ForCountLoop) -> None:
+    def visit(self, expr: astx.ForCountLoop) -> None:
         """Translate ASTx For Range Loop to LLVM-IR."""
         saved_block = self._llvm.ir_builder.block
         var_addr = self.create_entry_block_alloca("for_count_loop", "int32")
         self._llvm.ir_builder.position_at_end(saved_block)
 
         # Emit the start code first, without 'variable' in scope.
         self.visit(expr.initializer)
@@ -489,15 +489,15 @@
             self.named_values.pop(expr.initializer.name, None)
 
         # for expr always returns 0.0.
         result = ir.Constant(self._llvm.INT32_TYPE, 0)
         self.result_stack.append(result)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.ForRangeLoop) -> None:
+    def visit(self, expr: astx.ForRangeLoop) -> None:
         """Translate ASTx For Range Loop to LLVM-IR."""
         saved_block = self._llvm.ir_builder.block
         var_addr = self.create_entry_block_alloca("for_count_loop", "int32")
         self._llvm.ir_builder.position_at_end(saved_block)
 
         # Emit the start code first, without 'variable' in scope.
         self.visit(expr.start)
@@ -589,27 +589,27 @@
             self.named_values.pop(expr.variable.name, None)
 
         # for expr always returns 0.0.
         result = ir.Constant(self._llvm.INT32_TYPE, 0)
         self.result_stack.append(result)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Module) -> None:
+    def visit(self, expr: astx.Module) -> None:
         """Translate ASTx Module to LLVM-IR."""
         for node in expr.nodes:
             self.visit(node)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.LiteralInt32) -> None:
+    def visit(self, expr: astx.LiteralInt32) -> None:
         """Translate ASTx LiteralInt32 to LLVM-IR."""
         result = ir.Constant(self._llvm.INT32_TYPE, expr.value)
         self.result_stack.append(result)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.FunctionCall) -> None:
+    def visit(self, expr: astx.FunctionCall) -> None:
         """Translate Function FunctionCall."""
         callee_f = self.get_function(expr.callee)
 
         if not callee_f:
             raise Exception("Unknown function referenced")
 
         if len(callee_f.args) != len(expr.args):
@@ -623,15 +623,15 @@
                 raise Exception("codegen: Invalid callee argument.")
             llvm_args.append(llvm_arg)
 
         result = self._llvm.ir_builder.call(callee_f, llvm_args, "calltmp")
         self.result_stack.append(result)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Function) -> None:
+    def visit(self, expr: astx.Function) -> None:
         """Translate ASTx Function to LLVM-IR."""
         proto = expr.prototype
         self.function_protos[proto.name] = proto
         fn = self.get_function(proto.name)
 
         if not fn:
             raise Exception("Invalid function.")
@@ -652,15 +652,15 @@
             # Add arguments to variable symbol table.
             self.named_values[llvm_arg.name] = alloca
 
         self.visit(expr.body)
         self.result_stack.append(fn)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.FunctionPrototype) -> None:
+    def visit(self, expr: astx.FunctionPrototype) -> None:
         """Translate ASTx Function Prototype to LLVM-IR."""
         args_type = [self._llvm.INT32_TYPE] * len(expr.args)
         # note: it should be dynamic
         return_type = self._llvm.get_data_type("int32")
         fn_type = ir.FunctionType(return_type, args_type, False)
 
         fn = ir.Function(self._llvm.module, fn_type, expr.name)
@@ -668,30 +668,30 @@
         # Set names for all arguments.
         for idx, arg in enumerate(fn.args):
             fn.args[idx].name = expr.args[idx].name
 
         self.result_stack.append(fn)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.FunctionReturn) -> None:
+    def visit(self, expr: astx.FunctionReturn) -> None:
         """Translate ASTx FunctionReturn to LLVM-IR."""
         self.visit(expr.value)
 
         try:
             retval = self.result_stack.pop()
         except IndexError:
             retval = None
 
         if retval:
             self._llvm.ir_builder.ret(retval)
             return
         self._llvm.ir_builder.ret_void()
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.InlineVariableDeclaration) -> None:
+    def visit(self, expr: astx.InlineVariableDeclaration) -> None:
         """Translate an ASTx InlineVariableDeclaration expression."""
         if self.named_values.get(expr.name):
             raise Exception(f"Variable already declared: {expr.name}")
 
         # Emit the initializer
         if expr.value is not None:
             self.visit(expr.value)
@@ -704,26 +704,26 @@
         alloca = self.create_entry_block_alloca(expr.name, "int32")
         self._llvm.ir_builder.store(init_val, alloca)
         self.named_values[expr.name] = alloca
 
         self.result_stack.append(init_val)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.Variable) -> None:
+    def visit(self, expr: astx.Variable) -> None:
         """Translate ASTx Variable to LLVM-IR."""
         expr_var = self.named_values.get(expr.name)
 
         if not expr_var:
             raise Exception(f"Unknown variable name: {expr.name}")
 
         result = self._llvm.ir_builder.load(expr_var, expr.name)
         self.result_stack.append(result)
 
     @dispatch  # type: ignore[no-redef]
-    def visit(self, expr: ast.VariableDeclaration) -> None:
+    def visit(self, expr: astx.VariableDeclaration) -> None:
         """Translate ASTx Variable to LLVM-IR."""
         if self.named_values.get(expr.name):
             raise Exception(f"Variable already declared: {expr.name}")
 
         # Emit the initializer
         if expr.value is not None:
             self.visit(expr.value)
@@ -751,15 +751,15 @@
     """LLVM-IR transpiler and compiler."""
 
     def __init__(self) -> None:
         """Initialize LLVMIR."""
         super().__init__()
         self.translator: LLVMLiteIRVisitor = LLVMLiteIRVisitor()
 
-    def build(self, expr: ast.AST, output_file: str) -> None:
+    def build(self, expr: astx.AST, output_file: str) -> None:
         """Transpile the ASTx to LLVM-IR and build it to an executable file."""
         result = self.translate(expr)
 
         result_mod = llvm.parse_assembly(result)
         result_object = self.translator.target_machine.emit_object(result_mod)
 
         with tempfile.NamedTemporaryFile(suffix="", delete=False) as temp_file:
```

### Comparing `pyirx-1.1.0/src/irx/builders/symbol_table.py` & `pyirx-1.2.0/src/irx/builders/symbol_table.py`

 * *Files identical despite different names*

### Comparing `pyirx-1.1.0/PKG-INFO` & `pyirx-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyirx
-Version: 1.1.0
+Version: 1.2.0
 Summary: IRx
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: astx (>=0.9)
+Requires-Dist: astx (==0.11.*)
 Requires-Dist: atpublic (>=4.0)
 Requires-Dist: llvmlite (>=0.41.1)
 Requires-Dist: plum-dispatch (>=2.2.2)
 Requires-Dist: typing-extensions (>=4,<5) ; python_version < "3.9"
 Description-Content-Type: text/markdown
 
 # IRx
@@ -27,13 +27,13 @@
 **ASTx** is a generic project that offers a way to compound in an expressive way
 an **AST**. It is not specific for the **ArxLang** project, although it is main
 focus is to provide all needed feature for it.
 
 **IRx** uses **llvmlite** in order to generate **LLVM-IR** source.
 
 - Software License: BSD 3 Clause
-- Documentation: https://irx.arxlang.github.io.
+- Documentation: https://irx.arxlang.org.
 
 ## Features
 
 - Generate **LLVM-IR** from **ASTx**.
```

