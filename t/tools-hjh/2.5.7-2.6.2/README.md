# Comparing `tmp/tools_hjh-2.5.7.tar.gz` & `tmp/tools_hjh-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.5.7.tar", last modified: Tue Sep 26 08:34:43 2023, max compression
+gzip compressed data, was "dist\tools_hjh-2.6.2.tar", last modified: Mon Apr 22 04:50:05 2024, max compression
```

## Comparing `tools_hjh-2.5.7.tar` & `tools_hjh-2.6.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-09-26 08:34:43.000000 tools_hjh-2.5.7/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.7/LICENSE
--rw-rw-rw-   0        0        0      207 2023-09-26 08:34:43.000000 tools_hjh-2.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-09-26 08:34:43.000000 tools_hjh-2.5.7/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-09-26 08:30:17.000000 tools_hjh-2.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-26 08:34:43.000000 tools_hjh-2.5.7/tools_hjh/
--rw-rw-rw-   0        0        0     3215 2023-09-01 15:08:18.000000 tools_hjh-2.5.7/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     7791 2023-09-22 16:34:26.000000 tools_hjh-2.5.7/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.7/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.7/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.7/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.7/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    41650 2023-09-22 11:28:07.000000 tools_hjh-2.5.7/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.7/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.7/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     6685 2023-09-21 04:49:29.000000 tools_hjh-2.5.7/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.7/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-26 08:34:43.000000 tools_hjh-2.5.7/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2023-09-26 08:34:42.000000 tools_hjh-2.5.7/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-09-26 08:34:42.000000 tools_hjh-2.5.7/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-09-26 08:34:42.000000 tools_hjh-2.5.7/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      453 2023-09-26 08:34:42.000000 tools_hjh-2.5.7/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-09-26 08:34:42.000000 tools_hjh-2.5.7/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.2/LICENSE
+-rw-rw-rw-   0        0        0      207 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-02-19 08:41:24.000000 tools_hjh-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:50:04.000000 tools_hjh-2.6.2/tools_hjh/
+-rw-rw-rw-   0        0        0     3720 2024-03-13 07:44:26.000000 tools_hjh-2.6.2/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.2/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     6029 2024-04-22 03:27:09.000000 tools_hjh-2.6.2/tools_hjh/Fanyi.py
+-rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.2/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.2/tools_hjh/HTTPRequest2.py
+-rw-rw-rw-   0        0        0     9183 2024-03-13 12:45:59.000000 tools_hjh-2.6.2/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.2/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.2/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    44796 2024-04-22 02:39:49.000000 tools_hjh-2.6.2/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.2/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     2092 2024-03-13 06:16:36.000000 tools_hjh-2.6.2/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     7061 2024-04-22 01:45:38.000000 tools_hjh-2.6.2/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      539 2024-01-30 07:55:42.000000 tools_hjh-2.6.2/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-04-22 04:50:02.000000 tools_hjh-2.6.2/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      498 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.5.7/tools_hjh/Chrome.py` & `tools_hjh-2.6.2/tools_hjh/Chrome.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # coding:utf-8
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 import time
 from tools_hjh.ThreadPool import ThreadPool
+import os
+from tools_hjh import Tools
 
 
 def main():
     tp = ThreadPool(2, save_result=True)
     chrome_path = r'U:\MyApps\CentBrowser\App\chrome.exe'
     chromedriver_path = r'U:\MyApps\CentBrowser\chromedriver.exe'
 
@@ -54,15 +56,16 @@
     
     def get_status(self):
         return self.status
 
 
 class ChromePool():
 
-    def __init__(self, maxSize, chrome_path, chromedriver_path, is_hidden=False, is_display_picture=True):
+    def __init__(self, maxSize, chrome_path, chromedriver_path, is_hidden=False, is_display_picture=True, cache=False):
+        self.cache = cache
         self.maxSize = maxSize
         self.pool = []
         for _ in range(0, maxSize):
             self.pool.append(Chrome(chrome_path, chromedriver_path, is_hidden, is_display_picture))
         self.openSize = 0
         
     def set_cookies(self, cookies, cookie_domian):
@@ -77,16 +80,25 @@
         
     def get(self, url):
         while self.openSize == self.maxSize:
             time.sleep(0.2)
         for chrome in self.pool:
             if chrome.get_status() == 0:
                 self.openSize = self.openSize + 1
-                text = chrome.get(url)
-                # chrome.get(url='data:,')
+                if self.cache:
+                    url_split = url.split('/')
+                    host = url_split[0] + '//' + url_split[2] + '/'
+                    path_ = 'tmp/' + url.replace(host, '').rstrip('/')
+                    if os.path.exists(path_):
+                        text = Tools.cat(path_)
+                    else:
+                        text = chrome.get(url)
+                        Tools.echo(text, path_)
+                else:
+                    text = chrome.get(url)
                 self.openSize = self.openSize - 1
                 return text
         time.sleep(0.2)
         return self.get(url)
     
     def close(self):
         while self.openSize > 0:
```

### Comparing `tools_hjh-2.5.7/tools_hjh/DBConn.py` & `tools_hjh-2.6.2/tools_hjh/DBConn.py`

 * *Files 16% similar despite different names*

```diff
@@ -105,53 +105,89 @@
             conn = self.dbpool.acquire()
         else:
             conn = self.dbpool.connection()
             
         cur = conn.cursor()
         
         for sql in sql_list:
+            # 执行SELECT语句
+            if sql.lower().strip().startswith("select") or (sql.lower().strip().startswith("with") and 'select' in sql.lower()):
+                sql = sql.strip()
+                if param is None:
+                    cur.execute(sql)
+                elif type(param) == tuple:
+                    cur.execute(sql, param)
+                rs = QueryResults(cur, conn)
+                
             # 执行非SELECT语句
-            if not sql.lower().strip().startswith("select"):
+            elif not sql.lower().strip().startswith("select"):
                 sql = sql.strip()
                 if type(param) == list:
                     cur.executemany(sql, param)
                 elif type(param) == tuple:
                     cur.execute(sql, param)
                 elif param is None:
                     cur.execute(sql)
                 if auto_commit: 
                     if sql.lower().strip().startswith("update") or sql.lower().strip().startswith("delete") or sql.lower().strip().startswith("insert"):
                         conn.commit()
                 rownum = cur.rowcount
                 cur.close()
                 conn.close()
                 rs = rownum
-           
-            # 执行SELECT语句
-            if sql.lower().strip().startswith("select"):
-                sql = sql.strip()
-                if param is None:
-                    cur.execute(sql)
-                elif type(param) == tuple:
-                    cur.execute(sql, param)
-                rs = QueryResults(cur, conn)
-            
         return rs
 
     def run(self, sql, param=None, wait=False, auto_commit=True):
         """ 执行点什么
         sql中的占位符可以统一使用“?”
         wait为True则会等待当前正在执行的sql，有bug，暂不处理，自用规避"""
         if wait == True:
             tpnum = self.runtp.run(self.__run, (sql, param, auto_commit))
             self.runtp.wait()
             rs = self.runtp.result_map.pop(tpnum)
             return rs
         else:
             return self.__run(sql, param, auto_commit)
+        
+    def insert(self, table_name, rows, pks=[]):
+        """ 往指定table_name中插入数据，rows是一个多个元组的列表，每个元组表示一组参数；或者是一个元组 """
+        if type(rows) == list and len(rows) > 0:
+            row = rows[0]
+        elif type(rows) == tuple:
+            row = rows
+        elif len(rows) == 0:
+            return 0
+        
+        sql2 = ''
+        pk_num = 0
+        if type(pks) == str:
+            pk_num = 1
+            sql2 = sql2 + pks + ' = ?'
+        elif type(pks) == list or type(pks) == tuple:
+            pk_num = len(pks)
+            for pk in pks:
+                sql2 = sql2 + pk + ' = ? and '
+            sql2 = sql2.rstrip('and ')
+            
+        param_num = '?'
+        for _ in range(len(row) - 1 - pk_num):
+            param_num = param_num + ', ?'
+            
+        if self.dbtype == 'oracle':
+            if len(pks) == 0:
+                sql = 'insert into ' + table_name + ' select ' + param_num + ' from dual'
+            else:
+                sql = 'insert into ' + table_name + ' select ' + param_num + ' from dual where not exists(select 1 from ' + table_name + ' where ' + sql2 + ')'
+        else:
+            if len(pks) == 0:
+                sql = 'insert into ' + table_name + ' select ' + param_num
+            else:
+                sql = 'insert into ' + table_name + ' select ' + param_num + ' where not exists(select 1 from ' + table_name + ' where ' + sql2 + ')'
+        
+        return self.run(sql, rows)
     
     def close(self):
         try:
             self.dbpool.close()
         except:
             pass
         finally:
```

### Comparing `tools_hjh-2.5.7/tools_hjh/HTTPRequest.py` & `tools_hjh-2.6.2/tools_hjh/HTTPRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,48 +61,43 @@
         if self.response is None:
             self.connect()
         
         filepath = filepath.replace('\\', '/')
         path = filepath.rsplit('/', 1)[0] + '/'
         mkdir(path)
         
-        # 判断文件是否已经存在，如果存在且大小一致，视为已下载，不重复下载
-        content_size = self.get_size()
-        if content_size > 0 and os.path.exists(filepath):
-            existsFileSize = os.path.getsize(filepath)
-            if existsFileSize == content_size:
-                return existsFileSize
-            elif existsFileSize != content_size and replace:
-                rm(filepath)
-            else:
-                return 0
-        elif content_size == 0:
+        if os.path.exists(filepath) and replace:
+            rm(filepath)
+        elif os.path.exists(filepath) and not replace:
             return 0
-        
+
         try:
             with open(filepath, 'wb') as f:
                 for ch in self.response.iter_content(1024):
                     if ch:
                         f.write(ch)
         except Exception as _:
             pass
         finally:
             try:
                 f.close()
             except:
                 pass
         
         download_size = os.path.getsize(filepath)
-        
-        if content_size != download_size:
-            rm(filepath)
-            pass
-        
+
         return download_size
     
+    def download_until_success(self, filepath, replace=False):
+        """ 下载请求的文件, 返回文件大小, 如果抛出异常就重试 """
+        try:
+            return self.download(filepath, replace)
+        except:
+            return self.download_until_success(filepath, replace)
+
     def close(self):
         self.response = None
         self.head = None
     
     def __del__(self):
         self.close()
```

### Comparing `tools_hjh-2.5.7/tools_hjh/Log.py` & `tools_hjh-2.6.2/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.7/tools_hjh/MemoryDB.py` & `tools_hjh-2.6.2/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.7/tools_hjh/OracleTools.py` & `tools_hjh-2.6.2/tools_hjh/OracleTools.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,18 @@
                         data_type || '(' || data_precision || ', ' || data_scale || ')'
                     when data_type = 'NUMBER' and data_precision > 0 and data_scale = 0 then 
                         data_type || '(' || data_precision || ')'
                     when data_type = 'NUMBER' and data_precision = 0 and data_scale = 0 then 
                         data_type
                     else data_type 
                 end column_type, nullable, data_default
-            from dba_tab_cols where owner = ? and table_name = ? and column_name not like '%$%' order by column_id
+            from dba_tab_cols where owner = '{username}' and table_name = '{table}' and column_name not like '%$%' order by column_id
         '''
-        cols_ = ora_conn.run(sql, (username, table)).get_rows(True)
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        cols_ = ora_conn.run(sql).get_rows(True)
         lenNum = 0
         for col_ in cols_:
             if lenNum < len(col_[0]):
                 lenNum = len(col_[0])
         for col_ in cols_:
             colstr = col_[0]
             typestr = col_[1]
@@ -59,74 +60,39 @@
                 nullable = ''
             if col_[3] != 'None':
                 data_default = ' default ' + col_[3].replace('''/* GOLDENGATE_DDL_REPLICATION */''', '').strip().strip('\n')
             else:
                 data_default = ''
             mess = mess + 'column: ' + colstr.lower() + nullable + data_default + '\n'
             
-        # 约束 类型 列和列排序
-        sql = '''
-            select constraint_name, constraint_type
-            , max(cols)
-            from (
-                select t.constraint_name, t.constraint_type
-                , to_char(
-                    wm_concat(t2.column_name)
-                    over(partition by t.constraint_name order by t2.position)
-                ) cols
-                from dba_constraints t, dba_cons_columns t2
-                where t.owner = ?
-                and t.table_name = ?
-                and t.owner = t2.owner
-                and t.constraint_name = t2.constraint_name
-                and t.table_name = t2.table_name
-                and t.constraint_type in('P','U')
-            ) group by constraint_name, constraint_type
-            order by 3
-        '''
-        rss = ora_conn.run(sql, (username, table)).get_rows(True)
-        for rs in rss:
-            name = rs[0]
-            c_type = rs[1]
-            cols = rs[2].lower()
-            if c_type == 'U':
-                constraint_type = ' unique'
-            elif c_type == 'P':
-                constraint_type = ' pk'
-            else:
-                constraint_type = ''
-            if simple_mode:
-                mess = mess + 'constraint: (' + cols + ')' + constraint_type + '\n'
-            else:
-                mess = mess + 'constraint: ' + name.lower() + ' (' + cols + ')' + constraint_type + '\n'
-                
         # 索引 类型 列和列排序
         sql = '''
             select t.index_name
             , t.index_type
             , t2.column_name
             , t3.column_expression
             , t2.descend
             , t2.column_position
             , t.uniqueness
             from dba_indexes t, dba_ind_columns t2, dba_ind_expressions t3
-            where t.table_owner = ?
-            and t.table_name = ?
+            where t.table_owner = '{username}'
+            and t.table_name = '{table}'
             and t.owner = t2.index_owner
             and t.table_owner = t2.table_owner
             and t.index_name = t2.index_name
             and t.table_name = t2.table_name
             and t2.index_owner = t3.index_owner(+)
             and t2.table_owner = t3.table_owner(+)
             and t2.index_name = t3.index_name(+)
             and t2.table_name = t3.table_name(+)
             and t2.column_position = t3.column_position(+)
             order by t.index_type, t2.column_position
         '''
-        qrs = ora_conn.run(sql, (username, table))
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        qrs = ora_conn.run(sql)
         rows = qrs.get_rows()
         col = qrs.get_cols(True)
         if len(rows) > 0:
             mdb = MemoryDB()
             mdb.set('t_idx', col, rows)
             # 降序索引也体现为函数索引，列名会用"col_name"，而字符串用'str'
             sql = '''
@@ -153,15 +119,52 @@
                     idx_type = ' unique'
                 else:
                     idx_type = ''
                 if simple_mode:
                     ss = 'index: (' + col.replace(' asc', '').replace(',', ', ') + ')' + idx_type
                 else:
                     ss = 'index: ' + name.lower() + ' (' + col.replace(' asc', '').replace(',', ', ') + ')' + idx_type
-                mess = mess + ss + '\n'
+                mess = mess + ss + '\n'    
+                
+        # 约束 类型 列和列排序
+        sql = '''
+            select constraint_name, constraint_type
+            , max(cols)
+            from (
+                select t.constraint_name, t.constraint_type
+                , to_char(
+                    wm_concat(t2.column_name)
+                    over(partition by t.constraint_name order by t2.position)
+                ) cols
+                from dba_constraints t, dba_cons_columns t2
+                where t.owner = '{username}'
+                and t.table_name = '{table}'
+                and t.owner = t2.owner
+                and t.constraint_name = t2.constraint_name
+                and t.table_name = t2.table_name
+                and t.constraint_type in('P','U')
+            ) group by constraint_name, constraint_type
+            order by 3
+        '''
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        rss = ora_conn.run(sql).get_rows(True)
+        for rs in rss:
+            name = rs[0]
+            c_type = rs[1]
+            cols = rs[2].lower()
+            if c_type == 'U':
+                constraint_type = ' unique'
+            elif c_type == 'P':
+                constraint_type = ' pk'
+            else:
+                constraint_type = ''
+            if simple_mode:
+                mess = mess + 'constraint: (' + cols + ')' + constraint_type + '\n'
+            else:
+                mess = mess + 'constraint: ' + name.lower() + ' (' + cols + ')' + constraint_type + '\n'
         
         return mess.strip('\n')
 
     @staticmethod
     def compare_table(src_conn, src_username, src_table_name, dst_conn, dst_username, dst_table_name):
         """ 比较两个表，根据desc方法得到的字符串去比较 """
         src_username = src_username.upper()
@@ -169,14 +172,75 @@
 
         src_desc = OracleTools.desc(src_conn, src_username, src_table_name)
         dst_desc = OracleTools.desc(dst_conn, dst_username, dst_table_name)
         mess = line_merge_align(str_1=src_username + '.' + src_table_name + '\n' + src_desc
                                        , str_2=dst_username + '.' + dst_table_name + '\n' + dst_desc
                                        , iscompare=True) + '\n\n'
         return mess, '\t*' not in mess
+    
+    @staticmethod
+    def sync_table_simple(src_conn, src_username, src_table_name, dst_conn, dst_username, dst_table_name):
+        """ 比较两个表，根据desc方法得到的字符串去比较 """
+        src_username = src_username.upper()
+        dst_username = dst_username.upper()
+
+        src_desc = OracleTools.desc(src_conn, src_username, src_table_name)
+        dst_desc = OracleTools.desc(dst_conn, dst_username, dst_table_name)
+        
+        # 依据源端为本，目标端为匹配构建map
+        
+        col_map = []
+        idx_map = []
+        con_map = []
+        
+        for line in src_desc.split('\n'):
+            if line.startswith('column: '):
+                a = line.split(' ')[1]
+                b = line.split(' ')[0].strip(':')
+                c = line.split(' ')[2]
+                col_map.append([a, b, c, ''])
+                
+            if line.startswith('index: '):
+                a = line.split(': ')[1]
+                b = line.split(': ')[0]
+                idx_map.append([a, b, ''])
+                
+            if line.startswith('constraint: '):
+                a = line.split(': ')[1]
+                b = line.split(': ')[0]
+                con_map.append([a, b, ''])
+        
+        for line in dst_desc.split('\n'):
+            if line.startswith('column: '):
+                for one in col_map:
+                    if line.split(' ')[1] == one[0]:
+                        one[3] = line.split(' ')[2]
+   
+            if line.startswith('index: '):
+                for one in idx_map:
+                    if line.split(': ')[1] == one[0]:
+                        one[2] = line.split(': ')[1]
+                        
+            if line.startswith('constraint: '):
+                for one in con_map:
+                    if line.split(': ')[1] == one[0]:
+                        one[2] = line.split(': ')[1]
+        
+        for col in col_map:
+            # 同列不同类型，直接alter，可能不成功，不管
+            if col[2] != col[3] and col[3] != '':
+                sql = 'alter table ' + src_username + '.' + src_table_name + ' modify (' + col[0] + ' ' + col[2] + ');'
+                print(sql)
+        # 缺列，直接alter table add column
+            if col[2] != col[3] and col[3] == '':
+                sql = 'alter table ' + src_username + '.' + src_table_name + ' add ' + col[0] + ' ' + col[2] + ';'
+                print(sql)
+        # 缺索引或者外键，直接create
+        
+        return 0
 
     @staticmethod
     def get_ddl(dba_conn, username, type_, obj_name):
         """得到某个对象的ddl语言"""
         username = username.upper()
         obj_name = obj_name.upper()
         type_ = type_.upper()
@@ -189,41 +253,42 @@
     def get_table_ddl(dba_conn, username, table):
         """得到某个表的全部ddl语言，包含表、索引和列注释的ddl"""
         ddl_sqls = ''
         sql = '''
             select * from (
                 select table_owner owner, table_name, index_name obj_name, 'INDEX' obj_type 
                 from dba_indexes
-                where index_type != 'LOB' and owner = ? and table_name = ?
+                where index_type != 'LOB' and owner = '{username}' and table_name = '{table}'
                 union all
                 select owner, table_name, table_name, 'TABLE' obj_type 
                 from dba_tables
-                where owner = ? and table_name = ?
+                where owner = '{username}' and table_name = '{table}'
             ) t order by decode(obj_type, 'TABLE', 0, 'INDEX', 1), obj_name
         '''
-        rows = dba_conn.run(sql, (username, table, username, table)).get_rows(True)
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        rows = dba_conn.run(sql).get_rows(True)
         for row in rows:
             type_ = row[3]
             name = row[2]
             ddl_sql = OracleTools.get_ddl(dba_conn, username, type_, name) + ';'
             ddl_sqls = ddl_sqls + '-- ' + type_ + ' ' + name + '\n'
             ddl_sql = ddl_sql.lstrip().replace('"', '')
             ddl_sqls = ddl_sqls + ddl_sql + '\n\n'
             
         # 建注释
         sql = '''
             select column_name, comments
             from dba_col_comments
-            where owner = ? 
-            and table_name = ? 
+            where owner = '{username}'
+            and table_name = '{table}'
             and comments is not null
         '''
-        
+        sql = sql.replace('{username}', username).replace('{table}', table)
         ddl_sqls = ddl_sqls + '-- 注释' + '\n'
-        for r in dba_conn.run(sql, (username, table)).get_rows(True):
+        for r in dba_conn.run(sql).get_rows(True):
             ddl_sqls = ddl_sqls + "comment on column " + username + "." + table + "." + r[0] + " is '" + r[1] + "';\n"
             
         return ddl_sqls    
     
     @staticmethod
     def get_table_ddl_sample(ora_conn, username, table):
         """得到表结构，包括索引、约束和默认值情况"""
@@ -231,20 +296,21 @@
         table = table.strip()
         user_upper = username.upper()
         table_upper = table.upper()
         all_tablename_upper = user_upper + '.' + table_upper
         username = username.upper()
         table = table.upper()
         
-        exists_sql = '''
+        sql = '''
             select 1 from dba_tables 
-            where owner = ?
-            and table_name = ?
+            where owner = '{username}'
+            and table_name = '{table}'
         '''
-        rs = ora_conn.run(exists_sql, (username.upper(), table.upper())).get_rows()
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        rs = ora_conn.run(sql).get_rows()
         if len(rs) == 0:
             return '-- ' + all_tablename_upper + ' 不存在'
         
         mess = '-- drop table ' + all_tablename_upper + ' cascade constraints;\ncreate table ' + all_tablename_upper + '(test_col number);\n'
         
         # 列 类型 非空约束 默认值
         sql = '''
@@ -258,17 +324,18 @@
                         data_type || '(' || data_precision || ', ' || data_scale || ')'
                     when data_type = 'NUMBER' and data_precision > 0 and data_scale = 0 then 
                         data_type || '(' || data_precision || ')'
                     when data_type = 'NUMBER' and data_precision = 0 and data_scale = 0 then 
                         data_type
                     else data_type 
                 end column_type, nullable, data_default
-            from dba_tab_cols where owner = ? and table_name = ? and column_name not like '%$%' order by column_id
+            from dba_tab_cols where owner = '{username}' and table_name = '{table}' and column_name not like '%$%' order by column_id
         '''
-        cols_ = ora_conn.run(sql, (username, table)).get_rows(True)
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        cols_ = ora_conn.run(sql).get_rows(True)
         lenNum = 0
         for col_ in cols_:
             if lenNum < len(col_[0]):
                 lenNum = len(col_[0])
         for col_ in cols_:
             colstr = '"' + col_[0] + '"'
             typestr = col_[1]
@@ -279,69 +346,40 @@
                 nullable = ''
             if col_[3] != 'None':
                 data_default = ' default ' + col_[3].strip('\n')
             else:
                 data_default = ''
             mess = mess + 'alter table ' + all_tablename_upper + ' add ' + colstr.upper() + data_default + nullable + ';\n'
         mess = mess + 'alter table ' + all_tablename_upper + ' drop column test_col' + ';\n'
-        # 约束 类型 列和列排序
-        sql = '''
-            select constraint_name, constraint_type
-            , max(cols)
-            from (
-                select t.constraint_name, t.constraint_type
-                , to_char(
-                    wm_concat(t2.column_name)
-                    over(partition by t.constraint_name order by t2.position)
-                ) cols
-                from dba_constraints t, dba_cons_columns t2
-                where t.owner = ?
-                and t.table_name = ?
-                and t.owner = t2.owner
-                and t.constraint_name = t2.constraint_name
-                and t.table_name = t2.table_name
-                and t.constraint_type in('P','U')
-            ) group by constraint_name, constraint_type
-            order by constraint_name, constraint_type
-        '''
-        rss = ora_conn.run(sql, (username, table)).get_rows(True)
-        constraint_name = []
-        for rs in rss:
-            name = rs[0]
-            c_type = rs[1]
-            cols = rs[2]
-            if c_type == 'U':
-                mess = mess + 'alter table ' + all_tablename_upper + ' add unique (' + cols + ')' + ';\n'
-            elif c_type == 'P':
-                mess = mess + 'alter table ' + all_tablename_upper + ' add primary key (' + cols + ')' + ';\n'
-            constraint_name.append(name.lower())
+        
         # 索引 类型 列和列排序
         sql = '''
             select t.index_name
             , t.index_type
             , t2.column_name
             , t3.column_expression
             , t2.descend
             , t2.column_position
             , t.uniqueness
             from dba_indexes t, dba_ind_columns t2, dba_ind_expressions t3
-            where t.table_owner = ?
-            and t.table_name = ?
+            where t.table_owner = '{username}'
+            and t.table_name = '{table}'
             and t.owner = t2.index_owner
             and t.table_owner = t2.table_owner
             and t.index_name = t2.index_name
             and t.table_name = t2.table_name
             and t2.index_owner = t3.index_owner(+)
             and t2.table_owner = t3.table_owner(+)
             and t2.index_name = t3.index_name(+)
             and t2.table_name = t3.table_name(+)
             and t2.column_position = t3.column_position(+)
             order by t.index_type, t2.column_position
         '''
-        qrs = ora_conn.run(sql, (username, table))
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        qrs = ora_conn.run(sql)
         rows = qrs.get_rows()
         col = qrs.get_cols(True)
         if len(rows) > 0:
             mdb = MemoryDB()
             mdb.set('t_idx', col, rows)
             # 降序索引也体现为函数索引，列名会用"col_name"，而字符串用'str'
             sql = '''
@@ -357,35 +395,66 @@
                 , uniqueness, index_type
                 from t_idx 
             '''
             rss = mdb.db_conn.run(sql).get_rows(True)
             mdb.close()
             for rs in rss:
                 name = rs[0]
-                if name.lower() not in constraint_name:
-                    col = rs[1]
-                    if rs[3] == 'BITMAP':
-                        idx_type = 'bitmap'
-                    elif rs[2] == 'UNIQUE':
-                        idx_type = 'unique'
-                    else:
-                        idx_type = ''
-                    ss = 'create ' + idx_type + ' index ' + user_upper + '.' + name.upper() + ' on ' + all_tablename_upper + ' (' + col.replace(' asc', '').replace(',', ', ') + ');' 
-                    mess = mess + ss + '\n'
+                col = rs[1]
+                if rs[3] == 'BITMAP':
+                    idx_type = 'bitmap'
+                elif rs[2] == 'UNIQUE':
+                    idx_type = 'unique'
+                else:
+                    idx_type = ''
+                ss = 'create ' + idx_type + ' index ' + user_upper + '.' + name.upper() + ' on ' + all_tablename_upper + ' (' + col.replace(' asc', '').replace(',', ', ') + ');' 
+                mess = mess + ss + '\n'
+                
+        # 约束 类型 列和列排序
+        sql = '''
+            select constraint_name, constraint_type
+            , max(cols)
+            from (
+                select t.constraint_name, t.constraint_type
+                , to_char(
+                    wm_concat(t2.column_name)
+                    over(partition by t.constraint_name order by t2.position)
+                ) cols
+                from dba_constraints t, dba_cons_columns t2
+                where t.owner = '{username}'
+                and t.table_name = '{table}'
+                and t.owner = t2.owner
+                and t.constraint_name = t2.constraint_name
+                and t.table_name = t2.table_name
+                and t.constraint_type in('P','U')
+            ) group by constraint_name, constraint_type
+            order by constraint_name, constraint_type
+        '''
+        sql = sql.replace('{username}', username).replace('{table}', table)
+        rss = ora_conn.run(sql).get_rows(True)
+        for rs in rss:
+            name = rs[0]
+            c_type = rs[1]
+            cols = rs[2]
+            if c_type == 'U':
+                mess = mess + 'alter table ' + all_tablename_upper + ' add unique (' + cols + ')' + ';\n'
+            elif c_type == 'P':
+                mess = mess + 'alter table ' + all_tablename_upper + ' add primary key (' + cols + ')' + ';\n'
         
         # 建注释
         sql = '''
             select column_name, comments
             from dba_col_comments
-            where owner = ? 
-            and table_name = ? 
+            where owner = '{username}'
+            and table_name = '{table}'
             and comments is not null
         '''
+        sql = sql.replace('{username}', username).replace('{table}', table)
         mess = mess + '-- 注释' + '\n'
-        for r in ora_conn.run(sql, (username, table)).get_rows(True):
+        for r in ora_conn.run(sql).get_rows(True):
             mess = mess + "comment on column " + all_tablename_upper + "." + r[0].upper() + " is '" + r[1] + "';\n"
             
         return Tools.merge_spaces(mess).strip('\n') 
     
     @staticmethod
     def get_table_size(dba_conn, username, table):
         """得到一个表相关对象的容量分布情况"""
@@ -604,15 +673,15 @@
         # 进程状态 
         # 查询时间 ogg所在主机HOST ggsci所在路径 进程类型 进程状态 进程名称 lag_at_chkpt time_since_chkpt
         ogg_status = QueryResults2()
         ogg_status.get_rows().clear()
         ogg_status.set_cols(('query_time', 'host', 'ggsci_path', 'type', 'status', 'name', 'lag_at_chkpt', 'time_since_chkpt'))
         
         # 解析进程状态 
-        cmd = 'locate *ggsci'
+        cmd = 'find / -name *ggsci'
         paths = host_conn.exec_command(cmd)
         for path in paths.split('\n'):
             if username == 'oracle':
                 cmd = 'source ~/.bash_profile;echo "info all" | ' + path
             else:
                 cmd = '''su - oracle -c 'source ~/.bash_profile;echo "info all" | ''' + path + '\''
             mess = host_conn.exec_command(cmd)
```

### Comparing `tools_hjh-2.5.7/tools_hjh/SSHConn.py` & `tools_hjh-2.6.2/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.7/tools_hjh/ThreadPool.py` & `tools_hjh-2.6.2/tools_hjh/ThreadPool.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         if self.pool_status[0] < self.size:
             thread_id = uuid1()
             t = myThread(func, args=args, kwargs=kwargs, thread_id=thread_id, pool_status=self.pool_status, result_map=self.result_map, save_result=self.save_result)
             t.start()
             return thread_id
         else:
             while self.pool_status[0] >= self.size:
-                time.sleep(0.2)
+                time.sleep(0.5)
             return self.run(func, args, kwargs)
 
     def get_results(self):
         return self.result_map
     
     def get_result(self, num):
         return self.result_map[num]
     
     def clear_result(self):
         self.result_map = {}
 
     def wait(self):
         """ 主线程等待，直到线程池不存在活动线程 """
         while self.pool_status[0] > 0:
-            time.sleep(0.2)
+            time.sleep(0.5)
 
 
 class myThread (threading.Thread):
 
     def __init__(self, func, args, kwargs, thread_id, pool_status, result_map, save_result):
         threading.Thread.__init__(self)
         self.func = func
```

### Comparing `tools_hjh-2.5.7/tools_hjh/Tools.py` & `tools_hjh-2.6.2/tools_hjh/Tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         else:
             sql_line = line
         sql = sql + ' ' + sql_line
     sql = merge_spaces(sql.replace('\n', ' '))
     return sql
 
 
-def echo(text, path, mode='a'): 
+def echo(text, path, mode='a', encoding='utf-8'): 
     """ 把text输出到指定路径文件，不存在会创建（包括文件夹），mode默认是a，表示追加写，设为w表示覆写 """
     try:
         mkdir(os.path.dirname(path))
     except:
         pass
     path = path.replace('\u202a', '')
-    file = open(path, mode, encoding='utf-8', errors='ignore')
+    file = open(path, mode, encoding=encoding, errors='ignore')
     file.write(str(text) + '\n')
     file.close()
 
     
 def mkdir(path):
     """ 不存在则创建文件夹，逐层创建 """
     if not os.path.exists(path):
@@ -210,9 +210,27 @@
         strs = line.split(' ')
         if strs[0] != '::1' and strs[0] != '':
             for idx in range(1, len(strs)):
                 kv[strs[idx]] = strs[0]
     return kv
 
 
+def lstrip(ss, del_ss):
+    if ss.find(del_ss) == 0:
+        return ss[len(del_ss):len(ss)]
+    else:
+        return ss
+
+    
+def rstrip(ss, del_ss):
+    if ss.rfind(del_ss) == len(ss) - len(del_ss):
+        return ss[0:ss.rfind(del_ss)]
+    else:
+        return ss
+
+
+def strip(ss, del_ss):
+    return rstrip(lstrip(ss, del_ss), del_ss)
+
+
 if __name__ == '__main__':
     main()
```

