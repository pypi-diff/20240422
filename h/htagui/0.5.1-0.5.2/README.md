# Comparing `tmp/htagui-0.5.1.tar.gz` & `tmp/htagui-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.5.1.tar", max compression
+gzip compressed data, was "htagui-0.5.2.tar", max compression
```

## Comparing `htagui-0.5.1.tar` & `htagui-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2024-04-20 14:54:30.616303 htagui-0.5.1/LICENSE
--rw-r--r--   0        0        0     8232 2024-04-20 14:54:30.616303 htagui-0.5.1/README.md
--rw-r--r--   0        0        0      330 2024-04-20 14:54:30.864303 htagui-0.5.1/htagui/__init__.py
--rw-r--r--   0        0        0      846 2024-04-20 14:54:30.616303 htagui-0.5.1/htagui/all.py
--rw-r--r--   0        0        0      750 2024-04-20 14:54:30.616303 htagui-0.5.1/htagui/basics/__init__.py
--rw-r--r--   0        0        0    11089 2024-04-20 14:54:30.616303 htagui-0.5.1/htagui/basics/bases.py
--rw-r--r--   0        0        0      771 2024-04-20 14:54:30.616303 htagui-0.5.1/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   656140 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/bulma/bases.py
--rw-r--r--   0        0        0     3444 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/common.py
--rw-r--r--   0        0        0     3281 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/flex.py
--rw-r--r--   0        0        0      771 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/form.py
--rw-r--r--   0        0        0     3795 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/ifields.py
--rw-r--r--   0        0        0      746 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/md/__init__.py
--rw-r--r--   0        0        0    10527 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/md/bases.py
--rw-r--r--   0        0        0      774 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     8210 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     9619 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-04-20 14:54:30.620303 htagui-0.5.1/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-20 14:54:30.868303 htagui-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9465 1970-01-01 00:00:00.000000 htagui-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-22 07:02:21.192784 htagui-0.5.2/LICENSE
+-rw-r--r--   0        0        0     8232 2024-04-22 07:02:21.192784 htagui-0.5.2/README.md
+-rw-r--r--   0        0        0      330 2024-04-22 07:02:21.440784 htagui-0.5.2/htagui/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-22 07:02:21.192784 htagui-0.5.2/htagui/all.py
+-rw-r--r--   0        0        0      750 2024-04-22 07:02:21.192784 htagui-0.5.2/htagui/basics/__init__.py
+-rw-r--r--   0        0        0    11088 2024-04-22 07:02:21.192784 htagui-0.5.2/htagui/basics/bases.py
+-rw-r--r--   0        0        0      771 2024-04-22 07:02:21.192784 htagui-0.5.2/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   656139 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     3444 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/common.py
+-rw-r--r--   0        0        0     3282 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/flex.py
+-rw-r--r--   0        0        0      771 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/form.py
+-rw-r--r--   0        0        0     3795 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/ifields.py
+-rw-r--r--   0        0        0      746 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/md/__init__.py
+-rw-r--r--   0        0        0    10526 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/md/bases.py
+-rw-r--r--   0        0        0      774 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     8212 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     9619 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-04-22 07:02:21.196784 htagui-0.5.2/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-22 07:02:21.440784 htagui-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9465 1970-01-01 00:00:00.000000 htagui-0.5.2/PKG-INFO
```

### Comparing `htagui-0.5.1/LICENSE` & `htagui-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/README.md` & `htagui-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
 size is a float to force the percent of width on the dialog box. If None, it will use the default from the ui used.
 
 ### method dialog.confirm(obj, cbresponse=lambda bool:bool)
 
 (like js window.confirm(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able), and let the user click on Yes|No buttons, which will call the cbresponse callback with True or False ...
 
-### method dialog.prompt(value:str, title, cbresponse=lambda val:val)
+### method dialog.prompt(title, value:str, cbresponse=lambda val:val)
 
 (like js window.prompt(...)) Display a modal dialog letting the user edit the `value` in an Input box, with a `title` (title must be str'able). When the user click the OK button the value is sent in the callback cbresponse. (clicking the cancel button does nothing, except close the dialog)
 
 
 
 ### method dialog.notify(obj, time=2000)
```

### Comparing `htagui-0.5.1/htagui/all.py` & `htagui-0.5.2/htagui/all.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/basics/__init__.py` & `htagui-0.5.2/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/basics/bases.py` & `htagui-0.5.2/htagui/basics/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 class PopPage(Tag.div):
     def init(self,metatag,obj):
         self["style"].set("position","fixed")
         self["style"].set("top","0px")
         self["style"].set("bottom","0px")
         self["style"].set("right","0px")
         self["style"].set("left","0px")
-        self["style"].set("z-index","1000")
+        self["style"].set("z-index","500")
         self["style"].set("background","white")
         self <= obj
 
 
 class ModalAlert(ModalBlock):
     def __init__(self,metatag,obj,wsize:float=None):
         if wsize is None: wsize=0.6
```

### Comparing `htagui-0.5.1/htagui/bulma/__init__.py` & `htagui-0.5.2/htagui/bulma/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/bulma/bases.py` & `htagui-0.5.2/htagui/bulma/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -40801,209 +40801,209 @@
 0009f600: 2c22 3070 7822 290a 2020 2020 2020 2020  ,"0px").        
 0009f610: 7365 6c66 5b22 7374 796c 6522 5d2e 7365  self["style"].se
 0009f620: 7428 2272 6967 6874 222c 2230 7078 2229  t("right","0px")
 0009f630: 0a20 2020 2020 2020 2073 656c 665b 2273  .        self["s
 0009f640: 7479 6c65 225d 2e73 6574 2822 6c65 6674  tyle"].set("left
 0009f650: 222c 2230 7078 2229 0a20 2020 2020 2020  ","0px").       
 0009f660: 2073 656c 665b 2273 7479 6c65 225d 2e73   self["style"].s
-0009f670: 6574 2822 7a2d 696e 6465 7822 2c22 3130  et("z-index","10
-0009f680: 3030 2229 0a20 2020 2020 2020 2073 656c  00").        sel
-0009f690: 665b 2273 7479 6c65 225d 2e73 6574 2822  f["style"].set("
-0009f6a0: 6261 636b 6772 6f75 6e64 222c 2277 6869  background","whi
-0009f6b0: 7465 2229 0a20 2020 2020 2020 2073 656c  te").        sel
-0009f6c0: 6620 3c3d 206f 626a 0a0a 636c 6173 7320  f <= obj..class 
-0009f6d0: 4d6f 6461 6c41 6c65 7274 284d 6f64 616c  ModalAlert(Modal
-0009f6e0: 426c 6f63 6b29 3a0a 2020 2020 6465 6620  Block):.    def 
-0009f6f0: 5f5f 696e 6974 5f5f 2873 656c 662c 6d65  __init__(self,me
-0009f700: 7461 7461 672c 6f62 6a2c 7773 697a 653a  tatag,obj,wsize:
-0009f710: 666c 6f61 743d 4e6f 6e65 293a 0a20 2020  float=None):.   
-0009f720: 2020 2020 2069 6620 7773 697a 6520 6973       if wsize is
-0009f730: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0009f740: 2020 2020 2020 2070 7769 6474 683d 6622         pwidth=f"
-0009f750: 7b69 6e74 2877 7369 7a65 2a31 3030 297d  {int(wsize*100)}
-0009f760: 2522 2020 2020 2020 2020 0a20 2020 2020  %"        .     
-0009f770: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0009f780: 2020 2020 2070 7769 6474 683d 4e6f 6e65       pwidth=None
-0009f790: 0a20 2020 2020 2020 206f 626a 203d 2054  .        obj = T
-0009f7a0: 6167 2e64 6976 286f 626a 2c5f 636c 6173  ag.div(obj,_clas
-0009f7b0: 733d 2262 6f78 2229 0a20 2020 2020 2020  s="box").       
-0009f7c0: 206f 626a 3d54 6167 2e64 6976 286f 626a   obj=Tag.div(obj
-0009f7d0: 2c5f 636c 6173 733d 226d 6f64 616c 2d63  ,_class="modal-c
-0009f7e0: 6f6e 7465 6e74 2229 0a20 2020 2020 2020  ontent").       
-0009f7f0: 204d 6f64 616c 426c 6f63 6b2e 5f5f 696e   ModalBlock.__in
-0009f800: 6974 5f5f 2873 656c 662c 6d65 7461 7461  it__(self,metata
-0009f810: 672c 6f62 6a29 0a20 2020 2020 2020 2073  g,obj).        s
-0009f820: 656c 662e 6368 696c 6473 5b30 5d5b 226f  elf.childs[0]["o
-0009f830: 6e63 6c69 636b 225d 3d6d 6574 6174 6167  nclick"]=metatag
-0009f840: 2e73 7465 7065 7665 6e74 2829 0a20 2020  .stepevent().   
-0009f850: 2020 2020 2069 6620 7077 6964 7468 3a0a       if pwidth:.
-0009f860: 2020 2020 2020 2020 2020 2020 6f62 6a5b              obj[
-0009f870: 2273 7479 6c65 225d 3d66 2277 6964 7468  "style"]=f"width
-0009f880: 3a7b 7077 6964 7468 7d3b 220a 2020 2020  :{pwidth};".    
-0009f890: 2020 2020 7365 6c66 202b 3d20 5461 672e      self += Tag.
-0009f8a0: 6275 7474 6f6e 285f 636c 6173 733d 226d  button(_class="m
-0009f8b0: 6f64 616c 2d63 6c6f 7365 2069 732d 6c61  odal-close is-la
-0009f8c0: 7267 6522 2c5f 6172 6961 5f6c 6162 656c  rge",_aria_label
-0009f8d0: 3d22 636c 6f73 6522 2c5f 6f6e 636c 6963  ="close",_onclic
-0009f8e0: 6b3d 6d65 7461 7461 672e 7374 6570 6576  k=metatag.stepev
-0009f8f0: 656e 7428 2929 0a0a 0a63 6c61 7373 204d  ent())...class M
-0009f900: 6f64 616c 436f 6e66 6972 6d28 4d6f 6461  odalConfirm(Moda
-0009f910: 6c41 6c65 7274 293a 0a20 2020 2064 6566  lAlert):.    def
-0009f920: 205f 5f69 6e69 745f 5f28 7365 6c66 2c6d   __init__(self,m
-0009f930: 6574 6174 6167 2c6f 626a 2c63 6229 3a0a  etatag,obj,cb):.
-0009f940: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
-0009f950: 2865 7629 3a0a 2020 2020 2020 2020 2020  (ev):.          
-0009f960: 2020 6d65 7461 7461 672e 7374 6570 2829    metatag.step()
-0009f970: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0009f980: 7572 6e20 6362 2820 6576 2e74 6172 6765  urn cb( ev.targe
-0009f990: 742e 7661 6c20 290a 2020 2020 2020 2020  t.val ).        
-0009f9a0: 200a 2020 2020 2020 2020 626f 783d 5b20   .        box=[ 
-0009f9b0: 0a20 2020 2020 2020 2020 2020 2054 6167  .            Tag
-0009f9c0: 2e64 6976 286f 626a 292c 0a20 2020 2020  .div(obj),.     
-0009f9d0: 2020 2020 2020 2042 7574 746f 6e28 2259         Button("Y
-0009f9e0: 6573 222c 7661 6c3d 5472 7565 2c5f 6f6e  es",val=True,_on
-0009f9f0: 636c 6963 6b3d 6361 6c6c 292c 0a20 2020  click=call),.   
-0009fa00: 2020 2020 2020 2020 2042 7574 746f 6e28           Button(
-0009fa10: 224e 6f22 2c76 616c 3d46 616c 7365 2c5f  "No",val=False,_
-0009fa20: 6f6e 636c 6963 6b3d 6361 6c6c 292c 0a20  onclick=call),. 
-0009fa30: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0009fa40: 204d 6f64 616c 416c 6572 742e 5f5f 696e   ModalAlert.__in
-0009fa50: 6974 5f5f 2873 656c 662c 6d65 7461 7461  it__(self,metata
-0009fa60: 672c 626f 7829 0a0a 636c 6173 7320 4d6f  g,box)..class Mo
-0009fa70: 6461 6c50 726f 6d70 7428 4d6f 6461 6c41  dalPrompt(ModalA
-0009fa80: 6c65 7274 293a 0a20 2020 2064 6566 205f  lert):.    def _
-0009fa90: 5f69 6e69 745f 5f28 7365 6c66 2c6d 6574  _init__(self,met
-0009faa0: 6174 6167 2c20 7661 6c75 652c 7469 746c  atag, value,titl
-0009fab0: 652c 6362 293a 0a20 2020 2020 2020 2064  e,cb):.        d
-0009fac0: 6566 2063 616c 6c28 6469 636f 293a 0a20  ef call(dico):. 
-0009fad0: 2020 2020 2020 2020 2020 206d 6574 6174             metat
-0009fae0: 6167 2e73 7465 7028 290a 2020 2020 2020  ag.step().      
-0009faf0: 2020 2020 2020 7265 7475 726e 2063 6228        return cb(
-0009fb00: 2064 6963 6f5b 2270 726f 6d70 7476 616c   dico["promptval
-0009fb10: 7565 225d 2029 0a20 2020 2020 2020 2077  ue"] ).        w
-0009fb20: 6974 6820 466f 726d 286f 6e73 7562 6d69  ith Form(onsubmi
-0009fb30: 743d 6361 6c6c 2920 6173 2066 3a0a 2020  t=call) as f:.  
-0009fb40: 2020 2020 2020 2020 2020 662b 3d54 6167            f+=Tag
-0009fb50: 2e64 6976 2820 7469 746c 6520 290a 2020  .div( title ).  
-0009fb60: 2020 2020 2020 2020 2020 662b 3d54 6167            f+=Tag
-0009fb70: 2e64 6976 2820 496e 7075 7428 5f76 616c  .div( Input(_val
-0009fb80: 7565 3d76 616c 7565 2c5f 6e61 6d65 3d22  ue=value,_name="
-0009fb90: 7072 6f6d 7074 7661 6c75 6522 2c6a 733d  promptvalue",js=
-0009fba0: 2273 656c 662e 666f 6375 7328 293b 7365  "self.focus();se
-0009fbb0: 6c66 2e73 656c 6563 7428 2922 2c20 5f61  lf.select()", _a
-0009fbc0: 7574 6f66 6f63 7573 3d54 7275 6529 202c  utofocus=True) ,
-0009fbd0: 5f73 7479 6c65 3d22 7061 6464 696e 673a  _style="padding:
-0009fbe0: 3470 7820 3022 290a 2020 2020 2020 2020  4px 0").        
-0009fbf0: 2020 2020 662b 3d42 7574 746f 6e28 224f      f+=Button("O
-0009fc00: 6b22 2029 0a20 2020 2020 2020 2020 2020  k" ).           
-0009fc10: 2066 2b3d 4275 7474 6f6e 2822 4361 6e63   f+=Button("Canc
-0009fc20: 656c 222c 5f74 7970 653d 2262 7574 746f  el",_type="butto
-0009fc30: 6e22 2c5f 6f6e 636c 6963 6b3d 6d65 7461  n",_onclick=meta
-0009fc40: 7461 672e 7374 6570 6576 656e 7428 2929  tag.stepevent())
-0009fc50: 0a20 2020 2020 2020 204d 6f64 616c 416c  .        ModalAl
-0009fc60: 6572 742e 5f5f 696e 6974 5f5f 2873 656c  ert.__init__(sel
-0009fc70: 662c 6d65 7461 7461 672c 6629 0a20 2020  f,metatag,f).   
-0009fc80: 2020 2020 200a 636c 6173 7320 4472 6177       .class Draw
-0009fc90: 6572 2854 6167 2e64 6976 293a 0a20 2020  er(Tag.div):.   
-0009fca0: 2064 6566 2069 6e69 7428 7365 6c66 2c6d   def init(self,m
-0009fcb0: 6574 6174 6167 2c6f 626a 2c6d 6f64 653a  etatag,obj,mode:
-0009fcc0: 7374 7229 3a0a 2020 2020 2020 2020 7369  str):.        si
-0009fcd0: 7a65 3d35 300a 2020 2020 2020 2020 6966  ze=50.        if
-0009fce0: 206d 6f64 653d 3d22 6c65 6674 223a 0a20   mode=="left":. 
-0009fcf0: 2020 2020 2020 2020 2020 2074 2c72 2c62             t,r,b
-0009fd00: 2c6c 3d20 2822 3070 7822 2c66 227b 7369  ,l= ("0px",f"{si
-0009fd10: 7a65 7d25 222c 2230 7078 222c 2230 7078  ze}%","0px","0px
-0009fd20: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-0009fd30: 6d6f 6465 3d3d 2272 6967 6874 223a 0a20  mode=="right":. 
-0009fd40: 2020 2020 2020 2020 2020 2074 2c72 2c62             t,r,b
-0009fd50: 2c6c 3d20 2822 3070 7822 2c22 3070 7822  ,l= ("0px","0px"
-0009fd60: 2c22 3070 7822 2c66 227b 7369 7a65 7d25  ,"0px",f"{size}%
-0009fd70: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-0009fd80: 6d6f 6465 3d3d 2262 6f74 746f 6d22 3a0a  mode=="bottom":.
-0009fd90: 2020 2020 2020 2020 2020 2020 742c 722c              t,r,
-0009fda0: 622c 6c3d 2866 227b 7369 7a65 7d25 222c  b,l=(f"{size}%",
-0009fdb0: 2230 7078 222c 2230 7078 222c 2230 7078  "0px","0px","0px
-0009fdc0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-0009fdd0: 6d6f 6465 3d3d 2274 6f70 223a 0a20 2020  mode=="top":.   
-0009fde0: 2020 2020 2020 2020 2074 2c72 2c62 2c6c           t,r,b,l
-0009fdf0: 3d20 2822 3070 7822 2c22 3070 7822 2c66  = ("0px","0px",f
-0009fe00: 227b 7369 7a65 7d25 222c 2230 7078 2229  "{size}%","0px")
-0009fe10: 0a0a 2020 2020 2020 2020 7365 6c66 203c  ..        self <
-0009fe20: 3d20 566f 696c 6528 5f6f 6e6d 6f75 7365  = Voile(_onmouse
-0009fe30: 646f 776e 3d6d 6574 6174 6167 2e73 7465  down=metatag.ste
-0009fe40: 7065 7665 6e74 2829 290a 2020 2020 2020  pevent()).      
-0009fe50: 2020 7365 6c66 203c 3d20 5461 672e 6469    self <= Tag.di
-0009fe60: 7628 206f 626a 202c 5f73 7479 6c65 3d66  v( obj ,_style=f
-0009fe70: 2270 6f73 6974 696f 6e3a 6669 7865 643b  "position:fixed;
-0009fe80: 746f 703a 7b74 7d3b 626f 7474 6f6d 3a7b  top:{t};bottom:{
-0009fe90: 627d 3b6c 6566 743a 7b6c 7d3b 7269 6768  b};left:{l};righ
-0009fea0: 743a 7b72 7d3b 6261 636b 6772 6f75 6e64  t:{r};background
-0009feb0: 3a77 6869 7465 3b62 6f72 6465 722d 7261  :white;border-ra
-0009fec0: 6469 7573 3a30 7078 3b62 6f78 2d73 6861  dius:0px;box-sha
-0009fed0: 646f 773a 2072 6762 6128 302c 2030 2c20  dow: rgba(0, 0, 
-0009fee0: 302c 2030 2e33 3529 2030 7078 2035 7078  0, 0.35) 0px 5px
-0009fef0: 2031 3570 783b 3b7a 2d69 6e64 6578 3a31   15px;;z-index:1
-0009ff00: 3030 313b 7061 6464 696e 673a 3130 7078  001;padding:10px
-0009ff10: 2229 0a0a 636c 6173 7320 506f 7028 5461  ")..class Pop(Ta
-0009ff20: 672e 6469 7629 3a0a 2020 2020 6465 6620  g.div):.    def 
-0009ff30: 696e 6974 2873 656c 662c 6d65 7461 7461  init(self,metata
-0009ff40: 672c 6f62 6a2c 7879 3a74 7570 6c65 293a  g,obj,xy:tuple):
-0009ff50: 0a20 2020 2020 2020 2078 2c79 3d78 790a  .        x,y=xy.
-0009ff60: 2020 2020 2020 2020 7365 6c66 203c 3d20          self <= 
-0009ff70: 566f 696c 6528 5f6f 6e6d 6f75 7365 646f  Voile(_onmousedo
-0009ff80: 776e 3d6d 6574 6174 6167 2e73 7465 7065  wn=metatag.stepe
-0009ff90: 7665 6e74 2829 290a 2020 2020 2020 2020  vent()).        
-0009ffa0: 7365 6c66 203c 3d20 5461 672e 6469 7628  self <= Tag.div(
-0009ffb0: 206f 626a 202c 5f73 7479 6c65 3d66 2270   obj ,_style=f"p
-0009ffc0: 6f73 6974 696f 6e3a 6669 7865 643b 746f  osition:fixed;to
-0009ffd0: 703a 7b79 7d70 783b 6c65 6674 3a7b 787d  p:{y}px;left:{x}
-0009ffe0: 7078 3b7a 2d69 6e64 6578 3a31 3030 313b  px;z-index:1001;
-0009fff0: 6261 636b 6772 6f75 6e64 3a77 6869 7465  background:white
-000a0000: 2229 0a0a 636c 6173 7320 546f 6173 7428  ")..class Toast(
-000a0010: 5461 672e 6469 7629 3a0a 2020 2020 6465  Tag.div):.    de
-000a0020: 6620 696e 6974 2873 656c 662c 6d61 696e  f init(self,main
-000a0030: 5f6e 6f6e 5f75 7365 642c 6f62 6a2c 7469  _non_used,obj,ti
-000a0040: 6d65 6f75 743d 3130 3030 293a 0a20 2020  meout=1000):.   
-000a0050: 2020 2020 2073 656c 6620 3c3d 2054 6167       self <= Tag
-000a0060: 2e64 6976 286f 626a 2c5f 7374 796c 653d  .div(obj,_style=
-000a0070: 2270 6f73 6974 696f 6e3a 6669 7865 643b  "position:fixed;
-000a0080: 7269 6768 743a 3130 7078 3b62 6f74 746f  right:10px;botto
-000a0090: 6d3a 3130 7078 3b7a 2d69 6e64 6578 3a31  m:10px;z-index:1
-000a00a0: 3030 313b 222c 205f 636c 6173 733d 226e  001;", _class="n
-000a00b0: 6f74 6966 6963 6174 696f 6e20 6973 2d6c  otification is-l
-000a00c0: 696e 6b20 6973 2d6c 6967 6874 2229 0a20  ink is-light"). 
-000a00d0: 2020 2020 2020 2073 656c 662e 6a73 3d22         self.js="
-000a00e0: 7365 7454 696d 656f 7574 2820 6675 6e63  setTimeout( func
-000a00f0: 7469 6f6e 2829 207b 7365 6c66 2e72 656d  tion() {self.rem
-000a0100: 6f76 6528 297d 202c 2025 7329 2220 2520  ove()} , %s)" % 
-000a0110: 7469 6d65 6f75 740a 0a23 2323 2323 2323  timeout..#######
+0009f670: 6574 2822 7a2d 696e 6465 7822 2c22 3530  et("z-index","50
+0009f680: 3022 290a 2020 2020 2020 2020 7365 6c66  0").        self
+0009f690: 5b22 7374 796c 6522 5d2e 7365 7428 2262  ["style"].set("b
+0009f6a0: 6163 6b67 726f 756e 6422 2c22 7768 6974  ackground","whit
+0009f6b0: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+0009f6c0: 203c 3d20 6f62 6a0a 0a63 6c61 7373 204d   <= obj..class M
+0009f6d0: 6f64 616c 416c 6572 7428 4d6f 6461 6c42  odalAlert(ModalB
+0009f6e0: 6c6f 636b 293a 0a20 2020 2064 6566 205f  lock):.    def _
+0009f6f0: 5f69 6e69 745f 5f28 7365 6c66 2c6d 6574  _init__(self,met
+0009f700: 6174 6167 2c6f 626a 2c77 7369 7a65 3a66  atag,obj,wsize:f
+0009f710: 6c6f 6174 3d4e 6f6e 6529 3a0a 2020 2020  loat=None):.    
+0009f720: 2020 2020 6966 2077 7369 7a65 2069 7320      if wsize is 
+0009f730: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0009f740: 2020 2020 2020 7077 6964 7468 3d66 227b        pwidth=f"{
+0009f750: 696e 7428 7773 697a 652a 3130 3029 7d25  int(wsize*100)}%
+0009f760: 2220 2020 2020 2020 200a 2020 2020 2020  "        .      
+0009f770: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0009f780: 2020 2020 7077 6964 7468 3d4e 6f6e 650a      pwidth=None.
+0009f790: 2020 2020 2020 2020 6f62 6a20 3d20 5461          obj = Ta
+0009f7a0: 672e 6469 7628 6f62 6a2c 5f63 6c61 7373  g.div(obj,_class
+0009f7b0: 3d22 626f 7822 290a 2020 2020 2020 2020  ="box").        
+0009f7c0: 6f62 6a3d 5461 672e 6469 7628 6f62 6a2c  obj=Tag.div(obj,
+0009f7d0: 5f63 6c61 7373 3d22 6d6f 6461 6c2d 636f  _class="modal-co
+0009f7e0: 6e74 656e 7422 290a 2020 2020 2020 2020  ntent").        
+0009f7f0: 4d6f 6461 6c42 6c6f 636b 2e5f 5f69 6e69  ModalBlock.__ini
+0009f800: 745f 5f28 7365 6c66 2c6d 6574 6174 6167  t__(self,metatag
+0009f810: 2c6f 626a 290a 2020 2020 2020 2020 7365  ,obj).        se
+0009f820: 6c66 2e63 6869 6c64 735b 305d 5b22 6f6e  lf.childs[0]["on
+0009f830: 636c 6963 6b22 5d3d 6d65 7461 7461 672e  click"]=metatag.
+0009f840: 7374 6570 6576 656e 7428 290a 2020 2020  stepevent().    
+0009f850: 2020 2020 6966 2070 7769 6474 683a 0a20      if pwidth:. 
+0009f860: 2020 2020 2020 2020 2020 206f 626a 5b22             obj["
+0009f870: 7374 796c 6522 5d3d 6622 7769 6474 683a  style"]=f"width:
+0009f880: 7b70 7769 6474 687d 3b22 0a20 2020 2020  {pwidth};".     
+0009f890: 2020 2073 656c 6620 2b3d 2054 6167 2e62     self += Tag.b
+0009f8a0: 7574 746f 6e28 5f63 6c61 7373 3d22 6d6f  utton(_class="mo
+0009f8b0: 6461 6c2d 636c 6f73 6520 6973 2d6c 6172  dal-close is-lar
+0009f8c0: 6765 222c 5f61 7269 615f 6c61 6265 6c3d  ge",_aria_label=
+0009f8d0: 2263 6c6f 7365 222c 5f6f 6e63 6c69 636b  "close",_onclick
+0009f8e0: 3d6d 6574 6174 6167 2e73 7465 7065 7665  =metatag.stepeve
+0009f8f0: 6e74 2829 290a 0a0a 636c 6173 7320 4d6f  nt())...class Mo
+0009f900: 6461 6c43 6f6e 6669 726d 284d 6f64 616c  dalConfirm(Modal
+0009f910: 416c 6572 7429 3a0a 2020 2020 6465 6620  Alert):.    def 
+0009f920: 5f5f 696e 6974 5f5f 2873 656c 662c 6d65  __init__(self,me
+0009f930: 7461 7461 672c 6f62 6a2c 6362 293a 0a20  tatag,obj,cb):. 
+0009f940: 2020 2020 2020 2064 6566 2063 616c 6c28         def call(
+0009f950: 6576 293a 0a20 2020 2020 2020 2020 2020  ev):.           
+0009f960: 206d 6574 6174 6167 2e73 7465 7028 290a   metatag.step().
+0009f970: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0009f980: 726e 2063 6228 2065 762e 7461 7267 6574  rn cb( ev.target
+0009f990: 2e76 616c 2029 0a20 2020 2020 2020 2020  .val ).         
+0009f9a0: 0a20 2020 2020 2020 2062 6f78 3d5b 200a  .        box=[ .
+0009f9b0: 2020 2020 2020 2020 2020 2020 5461 672e              Tag.
+0009f9c0: 6469 7628 6f62 6a29 2c0a 2020 2020 2020  div(obj),.      
+0009f9d0: 2020 2020 2020 4275 7474 6f6e 2822 5965        Button("Ye
+0009f9e0: 7322 2c76 616c 3d54 7275 652c 5f6f 6e63  s",val=True,_onc
+0009f9f0: 6c69 636b 3d63 616c 6c29 2c0a 2020 2020  lick=call),.    
+0009fa00: 2020 2020 2020 2020 4275 7474 6f6e 2822          Button("
+0009fa10: 4e6f 222c 7661 6c3d 4661 6c73 652c 5f6f  No",val=False,_o
+0009fa20: 6e63 6c69 636b 3d63 616c 6c29 2c0a 2020  nclick=call),.  
+0009fa30: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0009fa40: 4d6f 6461 6c41 6c65 7274 2e5f 5f69 6e69  ModalAlert.__ini
+0009fa50: 745f 5f28 7365 6c66 2c6d 6574 6174 6167  t__(self,metatag
+0009fa60: 2c62 6f78 290a 0a63 6c61 7373 204d 6f64  ,box)..class Mod
+0009fa70: 616c 5072 6f6d 7074 284d 6f64 616c 416c  alPrompt(ModalAl
+0009fa80: 6572 7429 3a0a 2020 2020 6465 6620 5f5f  ert):.    def __
+0009fa90: 696e 6974 5f5f 2873 656c 662c 6d65 7461  init__(self,meta
+0009faa0: 7461 672c 2076 616c 7565 2c74 6974 6c65  tag, value,title
+0009fab0: 2c63 6229 3a0a 2020 2020 2020 2020 6465  ,cb):.        de
+0009fac0: 6620 6361 6c6c 2864 6963 6f29 3a0a 2020  f call(dico):.  
+0009fad0: 2020 2020 2020 2020 2020 6d65 7461 7461            metata
+0009fae0: 672e 7374 6570 2829 0a20 2020 2020 2020  g.step().       
+0009faf0: 2020 2020 2072 6574 7572 6e20 6362 2820       return cb( 
+0009fb00: 6469 636f 5b22 7072 6f6d 7074 7661 6c75  dico["promptvalu
+0009fb10: 6522 5d20 290a 2020 2020 2020 2020 7769  e"] ).        wi
+0009fb20: 7468 2046 6f72 6d28 6f6e 7375 626d 6974  th Form(onsubmit
+0009fb30: 3d63 616c 6c29 2061 7320 663a 0a20 2020  =call) as f:.   
+0009fb40: 2020 2020 2020 2020 2066 2b3d 5461 672e           f+=Tag.
+0009fb50: 6469 7628 2074 6974 6c65 2029 0a20 2020  div( title ).   
+0009fb60: 2020 2020 2020 2020 2066 2b3d 5461 672e           f+=Tag.
+0009fb70: 6469 7628 2049 6e70 7574 285f 7661 6c75  div( Input(_valu
+0009fb80: 653d 7661 6c75 652c 5f6e 616d 653d 2270  e=value,_name="p
+0009fb90: 726f 6d70 7476 616c 7565 222c 6a73 3d22  romptvalue",js="
+0009fba0: 7365 6c66 2e66 6f63 7573 2829 3b73 656c  self.focus();sel
+0009fbb0: 662e 7365 6c65 6374 2829 222c 205f 6175  f.select()", _au
+0009fbc0: 746f 666f 6375 733d 5472 7565 2920 2c5f  tofocus=True) ,_
+0009fbd0: 7374 796c 653d 2270 6164 6469 6e67 3a34  style="padding:4
+0009fbe0: 7078 2030 2229 0a20 2020 2020 2020 2020  px 0").         
+0009fbf0: 2020 2066 2b3d 4275 7474 6f6e 2822 4f6b     f+=Button("Ok
+0009fc00: 2220 290a 2020 2020 2020 2020 2020 2020  " ).            
+0009fc10: 662b 3d42 7574 746f 6e28 2243 616e 6365  f+=Button("Cance
+0009fc20: 6c22 2c5f 7479 7065 3d22 6275 7474 6f6e  l",_type="button
+0009fc30: 222c 5f6f 6e63 6c69 636b 3d6d 6574 6174  ",_onclick=metat
+0009fc40: 6167 2e73 7465 7065 7665 6e74 2829 290a  ag.stepevent()).
+0009fc50: 2020 2020 2020 2020 4d6f 6461 6c41 6c65          ModalAle
+0009fc60: 7274 2e5f 5f69 6e69 745f 5f28 7365 6c66  rt.__init__(self
+0009fc70: 2c6d 6574 6174 6167 2c66 290a 2020 2020  ,metatag,f).    
+0009fc80: 2020 2020 0a63 6c61 7373 2044 7261 7765      .class Drawe
+0009fc90: 7228 5461 672e 6469 7629 3a0a 2020 2020  r(Tag.div):.    
+0009fca0: 6465 6620 696e 6974 2873 656c 662c 6d65  def init(self,me
+0009fcb0: 7461 7461 672c 6f62 6a2c 6d6f 6465 3a73  tatag,obj,mode:s
+0009fcc0: 7472 293a 0a20 2020 2020 2020 2073 697a  tr):.        siz
+0009fcd0: 653d 3530 0a20 2020 2020 2020 2069 6620  e=50.        if 
+0009fce0: 6d6f 6465 3d3d 226c 6566 7422 3a0a 2020  mode=="left":.  
+0009fcf0: 2020 2020 2020 2020 2020 742c 722c 622c            t,r,b,
+0009fd00: 6c3d 2028 2230 7078 222c 6622 7b73 697a  l= ("0px",f"{siz
+0009fd10: 657d 2522 2c22 3070 7822 2c22 3070 7822  e}%","0px","0px"
+0009fd20: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
+0009fd30: 6f64 653d 3d22 7269 6768 7422 3a0a 2020  ode=="right":.  
+0009fd40: 2020 2020 2020 2020 2020 742c 722c 622c            t,r,b,
+0009fd50: 6c3d 2028 2230 7078 222c 2230 7078 222c  l= ("0px","0px",
+0009fd60: 2230 7078 222c 6622 7b73 697a 657d 2522  "0px",f"{size}%"
+0009fd70: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
+0009fd80: 6f64 653d 3d22 626f 7474 6f6d 223a 0a20  ode=="bottom":. 
+0009fd90: 2020 2020 2020 2020 2020 2074 2c72 2c62             t,r,b
+0009fda0: 2c6c 3d28 6622 7b73 697a 657d 2522 2c22  ,l=(f"{size}%","
+0009fdb0: 3070 7822 2c22 3070 7822 2c22 3070 7822  0px","0px","0px"
+0009fdc0: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
+0009fdd0: 6f64 653d 3d22 746f 7022 3a0a 2020 2020  ode=="top":.    
+0009fde0: 2020 2020 2020 2020 742c 722c 622c 6c3d          t,r,b,l=
+0009fdf0: 2028 2230 7078 222c 2230 7078 222c 6622   ("0px","0px",f"
+0009fe00: 7b73 697a 657d 2522 2c22 3070 7822 290a  {size}%","0px").
+0009fe10: 0a20 2020 2020 2020 2073 656c 6620 3c3d  .        self <=
+0009fe20: 2056 6f69 6c65 285f 6f6e 6d6f 7573 6564   Voile(_onmoused
+0009fe30: 6f77 6e3d 6d65 7461 7461 672e 7374 6570  own=metatag.step
+0009fe40: 6576 656e 7428 2929 0a20 2020 2020 2020  event()).       
+0009fe50: 2073 656c 6620 3c3d 2054 6167 2e64 6976   self <= Tag.div
+0009fe60: 2820 6f62 6a20 2c5f 7374 796c 653d 6622  ( obj ,_style=f"
+0009fe70: 706f 7369 7469 6f6e 3a66 6978 6564 3b74  position:fixed;t
+0009fe80: 6f70 3a7b 747d 3b62 6f74 746f 6d3a 7b62  op:{t};bottom:{b
+0009fe90: 7d3b 6c65 6674 3a7b 6c7d 3b72 6967 6874  };left:{l};right
+0009fea0: 3a7b 727d 3b62 6163 6b67 726f 756e 643a  :{r};background:
+0009feb0: 7768 6974 653b 626f 7264 6572 2d72 6164  white;border-rad
+0009fec0: 6975 733a 3070 783b 626f 782d 7368 6164  ius:0px;box-shad
+0009fed0: 6f77 3a20 7267 6261 2830 2c20 302c 2030  ow: rgba(0, 0, 0
+0009fee0: 2c20 302e 3335 2920 3070 7820 3570 7820  , 0.35) 0px 5px 
+0009fef0: 3135 7078 3b3b 7a2d 696e 6465 783a 3130  15px;;z-index:10
+0009ff00: 3031 3b70 6164 6469 6e67 3a31 3070 7822  01;padding:10px"
+0009ff10: 290a 0a63 6c61 7373 2050 6f70 2854 6167  )..class Pop(Tag
+0009ff20: 2e64 6976 293a 0a20 2020 2064 6566 2069  .div):.    def i
+0009ff30: 6e69 7428 7365 6c66 2c6d 6574 6174 6167  nit(self,metatag
+0009ff40: 2c6f 626a 2c78 793a 7475 706c 6529 3a0a  ,obj,xy:tuple):.
+0009ff50: 2020 2020 2020 2020 782c 793d 7879 0a20          x,y=xy. 
+0009ff60: 2020 2020 2020 2073 656c 6620 3c3d 2056         self <= V
+0009ff70: 6f69 6c65 285f 6f6e 6d6f 7573 6564 6f77  oile(_onmousedow
+0009ff80: 6e3d 6d65 7461 7461 672e 7374 6570 6576  n=metatag.stepev
+0009ff90: 656e 7428 2929 0a20 2020 2020 2020 2073  ent()).        s
+0009ffa0: 656c 6620 3c3d 2054 6167 2e64 6976 2820  elf <= Tag.div( 
+0009ffb0: 6f62 6a20 2c5f 7374 796c 653d 6622 706f  obj ,_style=f"po
+0009ffc0: 7369 7469 6f6e 3a66 6978 6564 3b74 6f70  sition:fixed;top
+0009ffd0: 3a7b 797d 7078 3b6c 6566 743a 7b78 7d70  :{y}px;left:{x}p
+0009ffe0: 783b 7a2d 696e 6465 783a 3130 3031 3b62  x;z-index:1001;b
+0009fff0: 6163 6b67 726f 756e 643a 7768 6974 6522  ackground:white"
+000a0000: 290a 0a63 6c61 7373 2054 6f61 7374 2854  )..class Toast(T
+000a0010: 6167 2e64 6976 293a 0a20 2020 2064 6566  ag.div):.    def
+000a0020: 2069 6e69 7428 7365 6c66 2c6d 6169 6e5f   init(self,main_
+000a0030: 6e6f 6e5f 7573 6564 2c6f 626a 2c74 696d  non_used,obj,tim
+000a0040: 656f 7574 3d31 3030 3029 3a0a 2020 2020  eout=1000):.    
+000a0050: 2020 2020 7365 6c66 203c 3d20 5461 672e      self <= Tag.
+000a0060: 6469 7628 6f62 6a2c 5f73 7479 6c65 3d22  div(obj,_style="
+000a0070: 706f 7369 7469 6f6e 3a66 6978 6564 3b72  position:fixed;r
+000a0080: 6967 6874 3a31 3070 783b 626f 7474 6f6d  ight:10px;bottom
+000a0090: 3a31 3070 783b 7a2d 696e 6465 783a 3130  :10px;z-index:10
+000a00a0: 3031 3b22 2c20 5f63 6c61 7373 3d22 6e6f  01;", _class="no
+000a00b0: 7469 6669 6361 7469 6f6e 2069 732d 6c69  tification is-li
+000a00c0: 6e6b 2069 732d 6c69 6768 7422 290a 2020  nk is-light").  
+000a00d0: 2020 2020 2020 7365 6c66 2e6a 733d 2273        self.js="s
+000a00e0: 6574 5469 6d65 6f75 7428 2066 756e 6374  etTimeout( funct
+000a00f0: 696f 6e28 2920 7b73 656c 662e 7265 6d6f  ion() {self.remo
+000a0100: 7665 2829 7d20 2c20 2573 2922 2025 2074  ve()} , %s)" % t
+000a0110: 696d 656f 7574 0a0a 2323 2323 2323 2323  imeout..########
 000a0120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000a0130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000a0140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000a0150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a0160: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-000a0170: 0a63 6c61 7373 2054 6162 7328 5461 672e  .class Tabs(Tag.
-000a0180: 6469 7629 3a0a 2020 2020 6465 6620 696e  div):.    def in
-000a0190: 6974 2873 656c 662c 6d65 7461 7461 672c  it(self,metatag,
-000a01a0: 7365 6c65 6374 6564 3d30 293a 0a20 2020  selected=0):.   
-000a01b0: 2020 2020 2075 6c20 3d20 5461 672e 756c       ul = Tag.ul
-000a01c0: 2829 0a20 2020 2020 2020 2066 6f72 2069  ().        for i
-000a01d0: 6478 2c69 2069 6e20 656e 756d 6572 6174  dx,i in enumerat
-000a01e0: 6528 6d65 7461 7461 672e 5f74 6162 7329  e(metatag._tabs)
-000a01f0: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
-000a0200: 6d65 203d 2068 6173 6174 7472 2869 2c22  me = hasattr(i,"
-000a0210: 6e61 6d65 2229 2061 6e64 2069 2e6e 616d  name") and i.nam
-000a0220: 6520 6f72 2022 3f28 6e61 6d65 293f 220a  e or "?(name)?".
-000a0230: 2020 2020 2020 2020 2020 2020 756c 2b3d              ul+=
-000a0240: 5461 672e 6c69 2820 5461 672e 6128 6e61  Tag.li( Tag.a(na
-000a0250: 6d65 292c 205f 6f6e 636c 6963 6b20 3d20  me), _onclick = 
-000a0260: 6d65 7461 7461 672e 7374 6570 6576 656e  metatag.stepeven
-000a0270: 7428 7365 6c65 6374 3d69 6478 292c 205f  t(select=idx), _
-000a0280: 636c 6173 733d 2269 732d 6163 7469 7665  class="is-active
-000a0290: 2220 6966 2069 6478 3d3d 7365 6c65 6374  " if idx==select
-000a02a0: 6564 2065 6c73 6520 2222 290a 2020 2020  ed else "").    
-000a02b0: 2020 2020 7365 6c66 3c3d 5461 672e 6469      self<=Tag.di
-000a02c0: 7628 756c 2c5f 636c 6173 733d 2274 6162  v(ul,_class="tab
-000a02d0: 7322 290a 2020 2020 2020 2020 6966 206d  s").        if m
-000a02e0: 6574 6174 6167 2e5f 7461 6273 3a20 7365  etatag._tabs: se
-000a02f0: 6c66 3c3d 6d65 7461 7461 672e 5f74 6162  lf<=metatag._tab
-000a0300: 735b 7365 6c65 6374 6564 5d0a            s[selected].
+000a0160: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
+000a0170: 636c 6173 7320 5461 6273 2854 6167 2e64  class Tabs(Tag.d
+000a0180: 6976 293a 0a20 2020 2064 6566 2069 6e69  iv):.    def ini
+000a0190: 7428 7365 6c66 2c6d 6574 6174 6167 2c73  t(self,metatag,s
+000a01a0: 656c 6563 7465 643d 3029 3a0a 2020 2020  elected=0):.    
+000a01b0: 2020 2020 756c 203d 2054 6167 2e75 6c28      ul = Tag.ul(
+000a01c0: 290a 2020 2020 2020 2020 666f 7220 6964  ).        for id
+000a01d0: 782c 6920 696e 2065 6e75 6d65 7261 7465  x,i in enumerate
+000a01e0: 286d 6574 6174 6167 2e5f 7461 6273 293a  (metatag._tabs):
+000a01f0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+000a0200: 6520 3d20 6861 7361 7474 7228 692c 226e  e = hasattr(i,"n
+000a0210: 616d 6522 2920 616e 6420 692e 6e61 6d65  ame") and i.name
+000a0220: 206f 7220 223f 286e 616d 6529 3f22 0a20   or "?(name)?". 
+000a0230: 2020 2020 2020 2020 2020 2075 6c2b 3d54             ul+=T
+000a0240: 6167 2e6c 6928 2054 6167 2e61 286e 616d  ag.li( Tag.a(nam
+000a0250: 6529 2c20 5f6f 6e63 6c69 636b 203d 206d  e), _onclick = m
+000a0260: 6574 6174 6167 2e73 7465 7065 7665 6e74  etatag.stepevent
+000a0270: 2873 656c 6563 743d 6964 7829 2c20 5f63  (select=idx), _c
+000a0280: 6c61 7373 3d22 6973 2d61 6374 6976 6522  lass="is-active"
+000a0290: 2069 6620 6964 783d 3d73 656c 6563 7465   if idx==selecte
+000a02a0: 6420 656c 7365 2022 2229 0a20 2020 2020  d else "").     
+000a02b0: 2020 2073 656c 663c 3d54 6167 2e64 6976     self<=Tag.div
+000a02c0: 2875 6c2c 5f63 6c61 7373 3d22 7461 6273  (ul,_class="tabs
+000a02d0: 2229 0a20 2020 2020 2020 2069 6620 6d65  ").        if me
+000a02e0: 7461 7461 672e 5f74 6162 733a 2073 656c  tatag._tabs: sel
+000a02f0: 663c 3d6d 6574 6174 6167 2e5f 7461 6273  f<=metatag._tabs
+000a0300: 5b73 656c 6563 7465 645d 0a              [selected].
```

### Comparing `htagui-0.5.1/htagui/common.py` & `htagui-0.5.2/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/dialog.py` & `htagui-0.5.2/htagui/dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def alert(self,obj,size:float=None):
         """if no size is provided : use the default width size of the dialog (depending of ui used)"""
         self.step( alert = obj, size=size )
 
     def confirm(self,obj,cbresponse=lambda bool:bool):
         self.step( confirm = obj, cb=cbresponse )
         
-    def prompt(self,value:str,title,cbresponse=lambda val:val):
+    def prompt(self,title, value:str,cbresponse=lambda val:val):
         self.step( prompt = value, title=title, cb=cbresponse )
 
     #DEPRECATED
     def box(self,obj,size:float=0.5):
         self.step( alert = obj, size=size )
```

### Comparing `htagui-0.5.1/htagui/flex.py` & `htagui-0.5.2/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/form.py` & `htagui-0.5.2/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/ifields.py` & `htagui-0.5.2/htagui/ifields.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/md/__init__.py` & `htagui-0.5.2/htagui/md/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/md/bases.py` & `htagui-0.5.2/htagui/md/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 class PopPage(Tag.div):
     def init(self,metatag,obj):
         self["style"].set("position","fixed")
         self["style"].set("top","0px")
         self["style"].set("bottom","0px")
         self["style"].set("right","0px")
         self["style"].set("left","0px")
-        self["style"].set("z-index","1000")
+        self["style"].set("z-index","500")
         self["style"].set("background","white")
         self <= obj
 
 
 class ModalBlock(Tag.div):
     def init(self,metatag,obj):
         modal=Tag.div( obj, _style="position:fixed;left:0px;right:0px;top:0px;bottom:0px;z-index:1001;    display:flex;align-items:center;justify-content:center;")
```

### Comparing `htagui-0.5.1/htagui/shoelace/__init__.py` & `htagui-0.5.2/htagui/shoelace/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/shoelace/bases.py` & `htagui-0.5.2/htagui/shoelace/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 class PopPage(Tag.div):
     def init(self,metatag,obj):
         self["style"].set("position","fixed")
         self["style"].set("top","0px")
         self["style"].set("bottom","0px")
         self["style"].set("right","0px")
         self["style"].set("left","0px")
-        self["style"].set("z-index","1")
+        self["style"].set("z-index","500")
         self["style"].set("background","white")
         self <= obj
 
 class ModalAlert(Tag.sl_dialog):
     def init(self,metatag,obj,closable=True,wsize:float=None):
         if wsize is not None:
             pwidth=f"{int(wsize*100)}%"
```

### Comparing `htagui-0.5.1/htagui/splitters.py` & `htagui-0.5.2/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/htagui/tabs.py` & `htagui-0.5.2/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.1/pyproject.toml` & `htagui-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.5.1" # auto-updated
+version = "0.5.2" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.5.1/PKG-INFO` & `htagui-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.5.1
+Version: 0.5.2
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -235,15 +235,15 @@
 
 size is a float to force the percent of width on the dialog box. If None, it will use the default from the ui used.
 
 ### method dialog.confirm(obj, cbresponse=lambda bool:bool)
 
 (like js window.confirm(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able), and let the user click on Yes|No buttons, which will call the cbresponse callback with True or False ...
 
-### method dialog.prompt(value:str, title, cbresponse=lambda val:val)
+### method dialog.prompt(title, value:str, cbresponse=lambda val:val)
 
 (like js window.prompt(...)) Display a modal dialog letting the user edit the `value` in an Input box, with a `title` (title must be str'able). When the user click the OK button the value is sent in the callback cbresponse. (clicking the cancel button does nothing, except close the dialog)
 
 
 
 ### method dialog.notify(obj, time=2000)
```

