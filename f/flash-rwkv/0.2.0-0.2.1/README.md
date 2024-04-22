# Comparing `tmp/flash_rwkv-0.2.0-py3-none-any.whl.zip` & `tmp/flash_rwkv-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5450 bytes, number of entries: 9
--rw-r--r--  2.0 unx      136 b- defN 24-Apr-07 08:57 flash_rwkv/__init__.py
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-07 08:57 flash_rwkv/rwkv5/__init__.py
--rw-r--r--  2.0 unx     6969 b- defN 24-Apr-07 09:29 flash_rwkv/rwkv5/wkv5_kernel.cu
--rw-r--r--  2.0 unx     4814 b- defN 24-Apr-01 01:36 flash_rwkv/rwkv5/wkv5_op.cpp
--rw-r--r--  2.0 unx     7196 b- defN 24-Apr-07 09:24 flash_rwkv/rwkv5/wkv5_op.py
--rw-r--r--  2.0 unx      145 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      728 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/RECORD
-9 files, 20229 bytes uncompressed, 4192 bytes compressed:  79.3%
+Zip file size: 5416 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      136 b- defN 24-Apr-21 02:44 flash_rwkv/__init__.py
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-21 02:44 flash_rwkv/rwkv5/__init__.py
+-rw-r--r--  2.0 unx     6969 b- defN 24-Apr-21 02:44 flash_rwkv/rwkv5/wkv5_kernel.cu
+-rw-r--r--  2.0 unx     4814 b- defN 24-Apr-21 02:44 flash_rwkv/rwkv5/wkv5_op.cpp
+-rw-r--r--  2.0 unx     7211 b- defN 24-Apr-22 01:13 flash_rwkv/rwkv5/wkv5_op.py
+-rw-r--r--  2.0 unx       87 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      727 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/RECORD
+9 files, 20185 bytes uncompressed, 4158 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: flash_rwkv/rwkv5/wkv5_op.cpp
 Comment: 
 
 Filename: flash_rwkv/rwkv5/wkv5_op.py
 Comment: 
 
-Filename: flash_rwkv-0.2.0.dist-info/METADATA
+Filename: flash_rwkv-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: flash_rwkv-0.2.0.dist-info/WHEEL
+Filename: flash_rwkv-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: flash_rwkv-0.2.0.dist-info/top_level.txt
+Filename: flash_rwkv-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: flash_rwkv-0.2.0.dist-info/RECORD
+Filename: flash_rwkv-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flash_rwkv/rwkv5/wkv5_op.py

```diff
@@ -92,18 +92,18 @@
                     receptance,
                     key,
                     value,
                     ee_time_decay,
                     time_first,
                     out,
                 )
-            return out
+            return out, state
 
     @staticmethod
-    def backward(ctx, gout):
+    def backward(ctx, gout, gstate):
         with torch.no_grad():
             batch = ctx.batch
             seq_length = ctx.seq_length
             hidden_size = ctx.hidden_size
             num_heads = ctx.num_heads
             receptance, key, value, ee_time_decay, e_time_decay, time_first = ctx.saved_tensors
```

## Comparing `flash_rwkv-0.2.0.dist-info/RECORD` & `flash_rwkv-0.2.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 flash_rwkv/__init__.py,sha256=jwlgTqPy1E2gNv27TzWy-FImqcBtLC8ZXp3qDqM_cpc,136
 flash_rwkv/rwkv5/__init__.py,sha256=desTKc7PgHTUMXxF9hdpUSg0rPv2lb_mk_HYViwpg68,138
 flash_rwkv/rwkv5/wkv5_kernel.cu,sha256=q98KLcmJSvTftpx8UhkbqRevtt1u_YtfAOvAfB6ilSc,6969
 flash_rwkv/rwkv5/wkv5_op.cpp,sha256=Rw3p6FrvQmwYYCb5sC0wVO6ZmwVngBn1Cz28MFMUsHM,4814
-flash_rwkv/rwkv5/wkv5_op.py,sha256=sNmALw2_5c76OixkzCYmvuWSFn-14yt7pvRwrnmmOvM,7196
-flash_rwkv-0.2.0.dist-info/METADATA,sha256=rXmrmCwFSZgQWdSbZD1CsmyPbab0_1i3RnvoDS-8Vuw,145
-flash_rwkv-0.2.0.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-flash_rwkv-0.2.0.dist-info/top_level.txt,sha256=EjGwpbozwPncfQBngaW7eKhIATRaBOJdMXrMgOJ8bPc,11
-flash_rwkv-0.2.0.dist-info/RECORD,,
+flash_rwkv/rwkv5/wkv5_op.py,sha256=w30V064SgGRBynsKPeV7snDk_s8ZU2wLL7AMIismEO0,7211
+flash_rwkv-0.2.1.dist-info/METADATA,sha256=GRjlVJBr5vi4dsLRVV8ECQVJW4WKP2KBfGwxJSW_Kmo,87
+flash_rwkv-0.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+flash_rwkv-0.2.1.dist-info/top_level.txt,sha256=EjGwpbozwPncfQBngaW7eKhIATRaBOJdMXrMgOJ8bPc,11
+flash_rwkv-0.2.1.dist-info/RECORD,,
```

