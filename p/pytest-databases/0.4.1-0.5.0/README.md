# Comparing `tmp/pytest_databases-0.4.1.tar.gz` & `tmp/pytest_databases-0.5.0.tar.gz`

## Comparing `pytest_databases-0.4.1.tar` & `pytest_databases-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/CODEOWNERS
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/Makefile
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/sonar-project.properties
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.vscode/launch.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.vscode/settings.json
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/alloydb_omni.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/bigquery.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.bigquery.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.cockroachdb.yml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.dragonfly.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.elasticsearch.yml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.keydb.yml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mariadb.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mssql.yml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mysql.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.oracle.yml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.postgres.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.redis.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.spanner.yml
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/elastic_search.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_alloydb_omni.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_bigquery.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_elasticsearch.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/LICENSE
--rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/README.md
--rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/CODEOWNERS
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/Makefile
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/sonar-project.properties
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.vscode/launch.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/requirements/requirements.txt
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/alloydb_omni.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/bigquery.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.bigquery.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.cockroachdb.yml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.dragonfly.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.keydb.yml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mariadb.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mssql.yml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.oracle.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.postgres.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.redis.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.spanner.yml
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/elastic_search.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_alloydb_omni.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_bigquery.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_elasticsearch.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/LICENSE
+-rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/README.md
+-rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/PKG-INFO
```

### Comparing `pytest_databases-0.4.1/.pre-commit-config.yaml` & `pytest_databases-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/.sourcery.yaml` & `pytest_databases-0.5.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/CONTRIBUTING.rst` & `pytest_databases-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/Makefile` & `pytest_databases-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/.vscode/settings.json` & `pytest_databases-0.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/requirements/requirements-dev.txt` & `pytest_databases-0.5.0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/requirements/requirements-docs.txt` & `pytest_databases-0.5.0/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/scripts/__init__.py` & `pytest_databases-0.5.0/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/scripts/build_docs.py` & `pytest_databases-0.5.0/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/__init__.py` & `pytest_databases-0.5.0/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/__metadata__.py` & `pytest_databases-0.5.0/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/helpers.py` & `pytest_databases-0.5.0/src/pytest_databases/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -126,29 +126,7 @@
 
     def stop(self, name: str) -> None:
         self.run_command("down", "--volumes", "-t", "10", name)
 
     def down(self) -> None:
         if not SKIP_DOCKER_COMPOSE:
             self.run_command("down", "-t", "10")
-
-
-@pytest.fixture(scope="session")
-def compose_project_name() -> str:
-    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
-
-
-@pytest.fixture(scope="session")
-def docker_services(compose_project_name: str, worker_id: str = "main") -> Generator[DockerServiceRegistry, None, None]:
-    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
-        pytest.skip("Docker not available on this platform")
-
-    registry = DockerServiceRegistry(worker_id, compose_project_name=compose_project_name)
-    try:
-        yield registry
-    finally:
-        registry.down()
-
-
-@pytest.fixture(scope="session")
-def docker_ip(docker_services: DockerServiceRegistry) -> str:
-    return docker_services.docker_ip
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/alloydb_omni.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/keydb.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,92 +20,89 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
-import asyncpg
 import pytest
+from redis.asyncio import Redis as AsyncRedis
+from redis.exceptions import ConnectionError as RedisConnectionError
+
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
 
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
 
 
-async def alloydb_omni_responsive(host: str, port: int, user: str, password: str, database: str) -> bool:
-    try:
-        conn = await asyncpg.connect(
-            host=host,
-            port=port,
-            user=user,
-            database=database,
-            password=password,
-        )
-    except Exception:  # noqa: BLE001
-        return False
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-keydb-{simple_string_hash(__file__)}"
 
+
+async def keydb_responsive(host: str, port: int) -> bool:
+    client: AsyncRedis = AsyncRedis(host=host, port=port)
     try:
-        db_open = await conn.fetchrow("SELECT 1")
-        return bool(db_open is not None and db_open[0] == 1)
+        return await client.ping()
+    except (ConnectionError, RedisConnectionError):
+        return False
     finally:
-        await conn.close()
+        await client.aclose()  # type: ignore[attr-defined]
+
 
+@pytest.fixture(autouse=False, scope="session")
+def keydb_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
 
-@pytest.fixture()
-def postgres_user() -> str:
-    return "postgres"
 
+@pytest.fixture(scope="session")
+def keydb_docker_services(
+    keydb_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
 
-@pytest.fixture()
-def postgres_password() -> str:
-    return "super-secret"
+    registry = DockerServiceRegistry(worker_id, compose_project_name=keydb_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
 
 
-@pytest.fixture()
-def postgres_database() -> str:
-    return "postgres"
+@pytest.fixture(scope="session")
+def keydb_port() -> int:
+    return 6396
 
 
-@pytest.fixture()
-def alloydb_omni_port() -> int:
-    return 5420
+@pytest.fixture(scope="session")
+def keydb_docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.keydb.yml")]
 
 
-@pytest.fixture()
-def default_alloydb_omni_service_name() -> str:
-    return "alloydb"
+@pytest.fixture(scope="session")
+def default_keydb_service_name() -> str:
+    return "keydb"
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
-    return [Path(Path(__file__).parent / "docker-compose.alloydb-omni.yml")]
+def keydb_docker_ip(keydb_docker_services: DockerServiceRegistry) -> str:
+    return keydb_docker_services.docker_ip
 
 
-# alias to the latest
-@pytest.fixture(autouse=False)
-async def alloydb_omni_service(
-    docker_services: DockerServiceRegistry,
-    default_alloydb_omni_service_name: str,
-    docker_compose_files: list[Path],
-    alloydb_omni_port: int,
-    postgres_database: str,
-    postgres_user: str,
-    postgres_password: str,
-) -> None:
-    os.environ["POSTGRES_PASSWORD"] = postgres_password
-    os.environ["POSTGRES_USER"] = postgres_user
-    os.environ["POSTGRES_DATABASE"] = postgres_database
-    os.environ[f"{default_alloydb_omni_service_name.upper()}_PORT"] = str(alloydb_omni_port)
-    await docker_services.start(
-        name=default_alloydb_omni_service_name,
-        docker_compose_files=docker_compose_files,
-        timeout=45,
-        pause=1,
-        check=alloydb_omni_responsive,
-        port=alloydb_omni_port,
-        database=postgres_database,
-        user=postgres_user,
-        password=postgres_password,
+@pytest.fixture(autouse=False, scope="session")
+async def keydb_service(
+    keydb_docker_services: DockerServiceRegistry,
+    default_keydb_service_name: str,
+    keydb_docker_compose_files: list[Path],
+    keydb_port: int,
+) -> AsyncGenerator[None, None]:
+    os.environ["KEYDB_PORT"] = str(keydb_port)
+    await keydb_docker_services.start(
+        name=default_keydb_service_name,
+        docker_compose_files=keydb_docker_compose_files,
+        check=keydb_responsive,
+        port=keydb_port,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/bigquery.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/bigquery.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,24 +20,31 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import pytest
 from google.api_core.client_options import ClientOptions
 from google.auth.credentials import AnonymousCredentials, Credentials
 from google.cloud import bigquery
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-bigquery-{simple_string_hash(__file__)}"
 
 
 async def bigquery_responsive(
     host: str,
     bigquery_endpoint: str,
     bigquery_dataset: str,
     bigquery_client_options: ClientOptions,
@@ -53,81 +60,106 @@
 
         resp = list(job.result())
         return resp[0].one == 1
     except Exception:  # noqa: BLE001
         return False
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
+def bigquery_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def bigquery_docker_services(
+    bigquery_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=bigquery_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def bigquery_port() -> int:
     return 9051
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def bigquery_grpc_port() -> int:
     return 9061
 
 
-@pytest.fixture
-def bigquery_endpoint(docker_ip: str, bigquery_port: int) -> str:
-    return f"http://{docker_ip}:{bigquery_port}"
-
-
-@pytest.fixture
+@pytest.fixture(scope="session")
 def bigquery_dataset() -> str:
     return "test-dataset"
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def bigquery_project() -> str:
     return "emulator-test-project"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def bigquery_client_options(bigquery_endpoint: str) -> ClientOptions:
     return ClientOptions(api_endpoint=bigquery_endpoint)
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def bigquery_credentials() -> Credentials:
     return AnonymousCredentials()
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def bigquery_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.bigquery.yml")]
 
 
 @pytest.fixture(scope="session")
 def default_bigquery_service_name() -> str:
     return "bigquery"
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def bigquery_docker_ip(bigquery_docker_services: DockerServiceRegistry) -> str:
+    return bigquery_docker_services.docker_ip
+
+
+@pytest.fixture(scope="session")
+def bigquery_endpoint(bigquery_docker_ip: str, bigquery_port: int) -> str:
+    return f"http://{bigquery_docker_ip}:{bigquery_port}"
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def bigquery_service(
-    docker_services: DockerServiceRegistry,
+    bigquery_docker_services: DockerServiceRegistry,
     default_bigquery_service_name: str,
-    docker_compose_files: list[Path],
+    bigquery_docker_compose_files: list[Path],
     bigquery_port: int,
     bigquery_grpc_port: int,
     bigquery_endpoint: str,
     bigquery_dataset: str,
     bigquery_project: str,
     bigquery_credentials: Credentials,
     bigquery_client_options: ClientOptions,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["BIGQUERY_ENDPOINT"] = bigquery_endpoint
     os.environ["BIGQUERY_DATASET"] = bigquery_dataset
     os.environ["BIGQUERY_PORT"] = str(bigquery_port)
     os.environ["BIGQUERY_GRPC_PORT"] = str(bigquery_grpc_port)
     os.environ["GOOGLE_CLOUD_PROJECT"] = bigquery_project
-    await docker_services.start(
+    await bigquery_docker_services.start(
         name=default_bigquery_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=bigquery_docker_compose_files,
         timeout=60,
         check=bigquery_responsive,
         bigquery_endpoint=bigquery_endpoint,
         bigquery_dataset=bigquery_dataset,
         bigquery_project=bigquery_project,
         bigquery_credentials=bigquery_credentials,
         bigquery_client_options=bigquery_client_options,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.alloydb-omni.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.bigquery.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.bigquery.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.dragonfly.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.dragonfly.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.elasticsearch.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mysql.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mysql.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.oracle.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.oracle.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.postgres.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.postgres.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.spanner.yml` & `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.spanner.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.5.0/tests/docker/test_keydb.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,58 +19,33 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
-import os
-from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
-from redis.asyncio import Redis as AsyncRedis
-from redis.exceptions import ConnectionError as RedisConnectionError
+
+from pytest_databases.docker.keydb import keydb_responsive
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
 
-
-async def keydb_responsive(host: str, port: int) -> bool:
-    client: AsyncRedis = AsyncRedis(host=host, port=port)
-    try:
-        return await client.ping()
-    except (ConnectionError, RedisConnectionError):
-        return False
-    finally:
-        await client.aclose()  # type: ignore[attr-defined]
-
-
-@pytest.fixture()
-def keydb_port() -> int:
-    return 6396
-
-
-@pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
-    return [Path(Path(__file__).parent / "docker-compose.keydb.yml")]
+pytestmark = pytest.mark.anyio
+pytest_plugins = [
+    "pytest_databases.docker.keydb",
+]
 
 
-@pytest.fixture(scope="session")
-def default_keydb_service_name() -> str:
-    return "keydb"
+def test_keydb_default_config(keydb_port: int) -> None:
+    assert keydb_port == 6396
 
 
-@pytest.fixture(autouse=False)
-async def keydb_service(
-    docker_services: DockerServiceRegistry,
-    default_keydb_service_name: str,
-    docker_compose_files: list[Path],
+async def test_keydb_service(
+    keydb_docker_ip: str,
+    keydb_service: DockerServiceRegistry,
     keydb_port: int,
 ) -> None:
-    os.environ["KEYDB_PORT"] = str(keydb_port)
-    await docker_services.start(
-        name=default_keydb_service_name,
-        docker_compose_files=docker_compose_files,
-        check=keydb_responsive,
-        port=keydb_port,
-    )
+    ping = await keydb_responsive(keydb_docker_ip, keydb_port)
+    assert ping
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/alloydb_omni.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,136 +19,125 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
-import contextlib
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
-import asyncmy
+import asyncpg
 import pytest
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-alloydb-{simple_string_hash(__file__)}"
 
 
-async def mariadb_responsive(host: str, port: int, user: str, password: str, database: str) -> bool:
+async def alloydb_omni_responsive(host: str, port: int, user: str, password: str, database: str) -> bool:
     try:
-        conn = await asyncmy.connect(
+        conn = await asyncpg.connect(
             host=host,
             port=port,
             user=user,
             database=database,
             password=password,
         )
     except Exception:  # noqa: BLE001
         return False
 
     try:
-        async with conn.cursor() as cursor:
-            await cursor.execute("select 1 as is_available")
-            resp = await cursor.fetchone()
-        return resp[0] == 1
+        db_open = await conn.fetchrow("SELECT 1")
+        return bool(db_open is not None and db_open[0] == 1)
     finally:
-        with contextlib.suppress(Exception):
-            await conn.close()
+        await conn.close()
 
 
-@pytest.fixture()
-def mariadb_user() -> str:
-    return "app"
+@pytest.fixture(scope="session")
+def alloydb_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
 
 
-@pytest.fixture()
-def mariadb_password() -> str:
-    return "super-secret"
+@pytest.fixture(autouse=False, scope="session")
+def alloydb_docker_services(
+    alloydb_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
 
+    registry = DockerServiceRegistry(worker_id, compose_project_name=alloydb_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
 
-@pytest.fixture()
-def mariadb_root_password() -> str:
-    return "super-secret"
 
+@pytest.fixture(scope="session")
+def postgres_user() -> str:
+    return "postgres"
 
-@pytest.fixture()
-def mariadb_database() -> str:
-    return "db"
 
+@pytest.fixture(scope="session")
+def postgres_password() -> str:
+    return "super-secret"
 
-@pytest.fixture()
-def mariadb113_port() -> int:
-    return 3359
 
+@pytest.fixture(scope="session")
+def postgres_database() -> str:
+    return "postgres"
 
-@pytest.fixture()
-def default_mariadb_service_name() -> str:
-    return "mariadb113"
 
+@pytest.fixture(scope="session")
+def alloydb_omni_port() -> int:
+    return 5420
 
-@pytest.fixture()
-def mariadb_port(mariadb113_port: int) -> int:
-    return mariadb113_port
+
+@pytest.fixture(scope="session")
+def default_alloydb_omni_service_name() -> str:
+    return "alloydb"
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
-    return [Path(Path(__file__).parent / "docker-compose.mariadb.yml")]
+def alloydb_docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.alloydb-omni.yml")]
 
 
-@pytest.fixture()
-async def mariadb113_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
-    mariadb113_port: int,
-    mariadb_database: str,
-    mariadb_user: str,
-    mariadb_password: str,
-    mariadb_root_password: str,
-) -> None:
-    os.environ["MARIADB_ROOT_PASSWORD"] = mariadb_root_password
-    os.environ["MARIADB_PASSWORD"] = mariadb_password
-    os.environ["MARIADB_USER"] = mariadb_user
-    os.environ["MARIADB_DATABASE"] = mariadb_database
-    os.environ["MARIADB113_PORT"] = str(mariadb113_port)
-    await docker_services.start(
-        "mariadb113",
-        docker_compose_files=docker_compose_files,
-        timeout=45,
-        pause=1,
-        check=mariadb_responsive,
-        port=mariadb113_port,
-        database=mariadb_database,
-        user=mariadb_user,
-        password=mariadb_password,
-    )
+@pytest.fixture(scope="session")
+def alloydb_docker_ip(alloydb_docker_services: DockerServiceRegistry) -> str:
+    return alloydb_docker_services.docker_ip
 
 
-@pytest.fixture()
-async def mariadb_service(
-    docker_services: DockerServiceRegistry,
-    default_mariadb_service_name: str,
-    docker_compose_files: list[Path],
-    mariadb_port: int,
-    mariadb_database: str,
-    mariadb_user: str,
-    mariadb_password: str,
-    mariadb_root_password: str,
-) -> None:
-    os.environ["MARIADB_ROOT_PASSWORD"] = mariadb_root_password
-    os.environ["MARIADB_PASSWORD"] = mariadb_password
-    os.environ["MARIADB_USER"] = mariadb_user
-    os.environ["MARIADB_DATABASE"] = mariadb_database
-    os.environ[f"{default_mariadb_service_name.upper()}_PORT"] = str(mariadb_port)
-    await docker_services.start(
-        name=default_mariadb_service_name,
-        docker_compose_files=docker_compose_files,
+# alias to the latest
+@pytest.fixture(autouse=False, scope="session")
+async def alloydb_omni_service(
+    alloydb_docker_services: DockerServiceRegistry,
+    default_alloydb_omni_service_name: str,
+    alloydb_docker_compose_files: list[Path],
+    alloydb_omni_port: int,
+    postgres_database: str,
+    postgres_user: str,
+    postgres_password: str,
+) -> AsyncGenerator[None, None]:
+    os.environ["POSTGRES_PASSWORD"] = postgres_password
+    os.environ["POSTGRES_USER"] = postgres_user
+    os.environ["POSTGRES_DATABASE"] = postgres_database
+    os.environ[f"{default_alloydb_omni_service_name.upper()}_PORT"] = str(alloydb_omni_port)
+    await alloydb_docker_services.start(
+        name=default_alloydb_omni_service_name,
+        docker_compose_files=alloydb_docker_compose_files,
         timeout=45,
         pause=1,
-        check=mariadb_responsive,
-        port=mariadb_port,
-        database=mariadb_database,
-        user=mariadb_user,
-        password=mariadb_password,
+        check=alloydb_omni_responsive,
+        port=alloydb_omni_port,
+        database=postgres_database,
+        user=postgres_user,
+        password=postgres_password,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/mssql.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,22 +21,29 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import asyncio
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import aioodbc
 import pytest
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-mssql-{simple_string_hash(__file__)}"
 
 
 async def mssql_responsive(host: str, connstring: str) -> bool:
     await asyncio.sleep(1)
     try:
         conn = await aioodbc.connect(
             dsn=connstring,
@@ -46,91 +53,117 @@
             await cursor.execute("select 1 as is_available")
             resp = await cursor.fetchone()
             return resp[0] == 1 if resp is not None else False
     except Exception:  # noqa: BLE001
         return False
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
+def mssql_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def mssql_docker_services(
+    mssql_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=mssql_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def mssql_user() -> str:
     return "sa"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mssql_password() -> str:
     return "Super-secret1"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mssql_database() -> str:
     return "master"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mssql2022_port() -> int:
     return 4133
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mssql_port(mssql2022_port: int) -> int:
     return mssql2022_port
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def mssql_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.mssql.yml")]
 
 
 @pytest.fixture(scope="session")
 def default_mssql_service_name() -> str:
     return "mssql2022"
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def mssql_docker_ip(mssql_docker_services: DockerServiceRegistry) -> str:
+    return mssql_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def mssql2022_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
-    docker_ip: str,
+    mssql_docker_services: DockerServiceRegistry,
+    mssql_docker_compose_files: list[Path],
+    mssql_docker_ip: str,
     mssql2022_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["MSSQL_PASSWORD"] = mssql_password
     os.environ["MSSQL_USER"] = mssql_user
     os.environ["MSSQL_DATABASE"] = mssql_database
     os.environ["MSSQL2022_PORT"] = str(mssql2022_port)
-    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={docker_ip},{mssql2022_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
-    await docker_services.start(
+    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={mssql_docker_ip},{mssql2022_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
+    await mssql_docker_services.start(
         "mssql2022",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=mssql_docker_compose_files,
         timeout=120,
         pause=1,
         check=mssql_responsive,
         connstring=connstring,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def mssql_service(
-    docker_services: DockerServiceRegistry,
+    mssql_docker_services: DockerServiceRegistry,
     default_mssql_service_name: str,
-    docker_compose_files: list[Path],
-    docker_ip: str,
+    mssql_docker_compose_files: list[Path],
+    mssql_docker_ip: str,
     mssql_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
-) -> None:
-    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={docker_ip},{mssql_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
+) -> AsyncGenerator[None, None]:
+    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={mssql_docker_ip},{mssql_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
     os.environ["MSSQL_PASSWORD"] = mssql_password
     os.environ["MSSQL_USER"] = mssql_user
     os.environ["MSSQL_DATABASE"] = mssql_database
     os.environ[f"{default_mssql_service_name.upper()}_PORT"] = str(mssql_port)
-    await docker_services.start(
+    await mssql_docker_services.start(
         name=default_mssql_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=mssql_docker_compose_files,
         timeout=120,
         pause=1,
         check=mssql_responsive,
         connstring=connstring,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/mysql.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,22 +21,29 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import contextlib
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import asyncmy
 import pytest
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-mysql-{simple_string_hash(__file__)}"
 
 
 async def mysql_responsive(host: str, port: int, user: str, password: str, database: str) -> bool:
     try:
         conn = await asyncmy.connect(
             host=host,
             port=port,
@@ -53,168 +60,196 @@
             resp = await cursor.fetchone()
         return resp[0] == 1
     finally:
         with contextlib.suppress(Exception):
             await conn.close()
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
+def mysql_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def mysql_docker_services(
+    mysql_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=mysql_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def mysql_user() -> str:
     return "app"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql_password() -> str:
     return "super-secret"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql_root_password() -> str:
     return "super-secret"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql_database() -> str:
     return "db"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql56_port() -> int:
     return 3362
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql57_port() -> int:
     return 3361
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def default_mysql_service_name() -> str:
     return "mysql8"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql8_port() -> int:
     return 3360
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def mysql_port(mysql8_port: int) -> int:
     return mysql8_port
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def mysql_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.mysql.yml")]
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def mysql_docker_ip(mysql_docker_services: DockerServiceRegistry) -> str:
+    return mysql_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def mysql8_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    mysql_docker_services: DockerServiceRegistry,
+    mysql_docker_compose_files: list[Path],
     mysql8_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ["MYSQL8_PORT"] = str(mysql8_port)
-    await docker_services.start(
+    await mysql_docker_services.start(
         "mysql8",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=mysql_docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql8_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def mysql57_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    mysql_docker_services: DockerServiceRegistry,
+    mysql_docker_compose_files: list[Path],
     mysql57_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ["MYSQL57_PORT"] = str(mysql57_port)
-    await docker_services.start(
+    await mysql_docker_services.start(
         "mysql57",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=mysql_docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql57_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def mysql56_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    mysql_docker_services: DockerServiceRegistry,
+    mysql_docker_compose_files: list[Path],
     mysql56_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ["MYSQL56_PORT"] = str(mysql56_port)
-    await docker_services.start(
+    await mysql_docker_services.start(
         "mysql56",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=mysql_docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql56_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def mysql_service(
-    docker_services: DockerServiceRegistry,
+    mysql_docker_services: DockerServiceRegistry,
     default_mysql_service_name: str,
-    docker_compose_files: list[Path],
+    mysql_docker_compose_files: list[Path],
     mysql_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ[f"{default_mysql_service_name.upper()}_PORT"] = str(mysql_port)
-    await docker_services.start(
+    await mysql_docker_services.start(
         name=default_mysql_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=mysql_docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/oracle.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,22 +20,29 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import oracledb
 import pytest
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-oracle-{simple_string_hash(__file__)}"
 
 
 def oracle_responsive(host: str, port: int, service_name: str, user: str, password: str) -> bool:
     try:
         conn = oracledb.connect(
             host=host,
             port=port,
@@ -47,146 +54,173 @@
             cursor.execute("SELECT 1 FROM dual")
             resp = cursor.fetchone()
         return resp[0] == 1 if resp is not None else False
     except Exception:  # noqa: BLE001
         return False
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
+def oracle_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def oracle_docker_services(
+    oracle_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=oracle_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def oracle_user() -> str:
     return "app"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle_password() -> str:
     return "super-secret"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle_system_password() -> str:
     return "super-secret"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle18c_service_name() -> str:
     return "xepdb1"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle23c_service_name() -> str:
     return "FREEPDB1"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle_service_name(oracle23c_service_name: str) -> str:
     return oracle23c_service_name
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle18c_port() -> int:
     return 1514
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle23c_port() -> int:
     return 1513
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def default_oracle_service_name() -> str:
     return "oracle23c"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def oracle_port(oracle23c_port: int) -> int:
     return oracle23c_port
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def oracle_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.oracle.yml")]
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def oracle_docker_ip(oracle_docker_services: DockerServiceRegistry) -> str:
+    return oracle_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def oracle23c_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    oracle_docker_services: DockerServiceRegistry,
+    oracle_docker_compose_files: list[Path],
     oracle23c_port: int,
     oracle23c_service_name: str,
     oracle_system_password: str,
     oracle_user: str,
     oracle_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["ORACLE_PASSWORD"] = oracle_password
     os.environ["ORACLE_SYSTEM_PASSWORD"] = oracle_system_password
     os.environ["ORACLE_USER"] = oracle_user
     os.environ["ORACLE23C_SERVICE_NAME"] = oracle23c_service_name
     os.environ["ORACLE23C_PORT"] = str(oracle23c_port)
-    await docker_services.start(
+    await oracle_docker_services.start(
         "oracle23c",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=oracle_docker_compose_files,
         timeout=90,
         pause=1,
         check=oracle_responsive,
         port=oracle23c_port,
         service_name=oracle23c_service_name,
         user=oracle_user,
         password=oracle_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def oracle18c_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    oracle_docker_services: DockerServiceRegistry,
+    oracle_docker_compose_files: list[Path],
     oracle18c_port: int,
     oracle18c_service_name: str,
     oracle_system_password: str,
     oracle_user: str,
     oracle_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["ORACLE_PASSWORD"] = oracle_password
     os.environ["ORACLE_SYSTEM_PASSWORD"] = oracle_system_password
     os.environ["ORACLE_USER"] = oracle_user
     os.environ["ORACLE18C_SERVICE_NAME"] = oracle18c_service_name
     os.environ["ORACLE18C_PORT"] = str(oracle18c_port)
-    await docker_services.start(
+    await oracle_docker_services.start(
         "oracle18c",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=oracle_docker_compose_files,
         timeout=90,
         pause=1,
         check=oracle_responsive,
         port=oracle18c_port,
         service_name=oracle18c_service_name,
         user=oracle_user,
         password=oracle_password,
     )
+    yield
 
 
 # alias to the latest
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def oracle_service(
-    docker_services: DockerServiceRegistry,
+    oracle_docker_services: DockerServiceRegistry,
     default_oracle_service_name: str,
-    docker_compose_files: list[Path],
+    oracle_docker_compose_files: list[Path],
     oracle_port: int,
     oracle_service_name: str,
     oracle_system_password: str,
     oracle_user: str,
     oracle_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["ORACLE_PASSWORD"] = oracle_password
     os.environ["ORACLE_SYSTEM_PASSWORD"] = oracle_system_password
     os.environ["ORACLE_USER"] = oracle_user
     os.environ["ORACLE_SERVICE_NAME"] = oracle_service_name
     os.environ[f"{default_oracle_service_name.upper()}_PORT"] = str(oracle_port)
-    await docker_services.start(
+    await oracle_docker_services.start(
         name=default_oracle_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=oracle_docker_compose_files,
         timeout=90,
         pause=1,
         check=oracle_responsive,
         port=oracle_port,
         service_name=oracle_service_name,
         user=oracle_user,
         password=oracle_password,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/postgres.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,22 +20,29 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import asyncpg
 import pytest
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-postgres-{simple_string_hash(__file__)}"
 
 
 async def postgres_responsive(host: str, port: int, user: str, password: str, database: str) -> bool:
     try:
         conn = await asyncpg.connect(
             host=host,
             port=port,
@@ -49,223 +56,253 @@
     try:
         db_open = await conn.fetchrow("SELECT 1")
         return bool(db_open is not None and db_open[0] == 1)
     finally:
         await conn.close()
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
+def postgres_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def postgres_docker_services(
+    postgres_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=postgres_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def postgres_user() -> str:
     return "postgres"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres_password() -> str:
     return "super-secret"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres_database() -> str:
     return "postgres"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres11_port() -> int:
     return 5422
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres12_port() -> int:
     return 5423
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres13_port() -> int:
     return 5424
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres14_port() -> int:
     return 5425
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres15_port() -> int:
     return 5426
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres16_port() -> int:
     return 5427
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def default_postgres_service_name() -> str:
     return "postgres16"
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def postgres_port(postgres16_port: int) -> int:
     return postgres16_port
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def postgres_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.postgres.yml")]
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def postgres_docker_ip(postgres_docker_services: DockerServiceRegistry) -> str:
+    return postgres_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def postgres12_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    postgres_docker_services: DockerServiceRegistry,
+    postgres_docker_compose_files: list[Path],
     postgres12_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES12_PORT"] = str(postgres12_port)
-    await docker_services.start(
+    await postgres_docker_services.start(
         "postgres12",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=postgres_docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres12_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def postgres13_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    postgres_docker_services: DockerServiceRegistry,
+    postgres_docker_compose_files: list[Path],
     postgres13_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES13_PORT"] = str(postgres13_port)
-    await docker_services.start(
+    await postgres_docker_services.start(
         "postgres13",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=postgres_docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres13_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def postgres14_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    postgres_docker_services: DockerServiceRegistry,
+    postgres_docker_compose_files: list[Path],
     postgres14_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES14_PORT"] = str(postgres14_port)
-    await docker_services.start(
+    await postgres_docker_services.start(
         "postgres14",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=postgres_docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres14_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def postgres15_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    postgres_docker_services: DockerServiceRegistry,
+    postgres_docker_compose_files: list[Path],
     postgres15_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES15_PORT"] = str(postgres15_port)
-    await docker_services.start(
+    await postgres_docker_services.start(
         "postgres15",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=postgres_docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres15_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
+    yield
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def postgres16_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    postgres_docker_services: DockerServiceRegistry,
+    postgres_docker_compose_files: list[Path],
     postgres16_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES16_PORT"] = str(postgres16_port)
-    await docker_services.start(
+    await postgres_docker_services.start(
         "postgres16",
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=postgres_docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres16_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
+    yield
 
 
 # alias to the latest
-@pytest.fixture(autouse=False)
+@pytest.fixture(autouse=False, scope="session")
 async def postgres_service(
-    docker_services: DockerServiceRegistry,
+    postgres_docker_services: DockerServiceRegistry,
     default_postgres_service_name: str,
-    docker_compose_files: list[Path],
+    postgres_docker_compose_files: list[Path],
     postgres_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ[f"{default_postgres_service_name.upper()}_PORT"] = str(postgres_port)
-    await docker_services.start(
+    await postgres_docker_services.start(
         name=default_postgres_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=postgres_docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/redis.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/redis.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,57 +20,89 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import pytest
 from redis.asyncio import Redis as AsyncRedis
 from redis.exceptions import ConnectionError as RedisConnectionError
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-redis-{simple_string_hash(__file__)}"
 
 
 async def redis_responsive(host: str, port: int) -> bool:
     client: AsyncRedis = AsyncRedis(host=host, port=port)
     try:
         return await client.ping()
     except (ConnectionError, RedisConnectionError):
         return False
     finally:
         await client.aclose()  # type: ignore[attr-defined]
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
+def redis_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def redis_docker_services(
+    redis_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=redis_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def redis_port() -> int:
     return 6397
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def redis_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.redis.yml")]
 
 
 @pytest.fixture(scope="session")
 def default_redis_service_name() -> str:
     return "redis"
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def redis_docker_ip(redis_docker_services: DockerServiceRegistry) -> str:
+    return redis_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def redis_service(
-    docker_services: DockerServiceRegistry,
+    redis_docker_services: DockerServiceRegistry,
     default_redis_service_name: str,
-    docker_compose_files: list[Path],
+    redis_docker_compose_files: list[Path],
     redis_port: int,
-) -> None:
+) -> AsyncGenerator[None, None]:
     os.environ["REDIS_PORT"] = str(redis_port)
-    await docker_services.start(
+    await redis_docker_services.start(
         name=default_redis_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=redis_docker_compose_files,
         check=redis_responsive,
         port=redis_port,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/spanner.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,23 +21,30 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import contextlib
 import os
+import sys
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import pytest
 from google.auth.credentials import AnonymousCredentials, Credentials
 from google.cloud import spanner
 
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
+
 if TYPE_CHECKING:
-    from pytest_databases.docker import DockerServiceRegistry
+    from collections.abc import Generator
+
+
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-spanner-{simple_string_hash(__file__)}"
 
 
 def spanner_responsive(
     host: str,
     spanner_port: int,
     spanner_instance: str,
     spanner_database: str,
@@ -57,70 +64,95 @@
         with database.snapshot() as snapshot:
             resp = next(iter(snapshot.execute_sql("SELECT 1")))
         return resp[0] == 1
     except Exception:  # noqa: BLE001
         return False
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
+def spanner_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def spanner_docker_services(
+    spanner_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=spanner_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
 def spanner_port() -> int:
     return 9010
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def spanner_instance() -> str:
     return "test-instance"
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def spanner_database() -> str:
     return "test-database"
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def spanner_project() -> str:
     return "emulator-test-project"
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def spanner_credentials() -> Credentials:
     return AnonymousCredentials()
 
 
 @pytest.fixture(scope="session")
-def docker_compose_files() -> list[Path]:
+def spanner_docker_compose_files() -> list[Path]:
     return [Path(Path(__file__).parent / "docker-compose.spanner.yml")]
 
 
 @pytest.fixture(scope="session")
 def default_spanner_service_name() -> str:
     return "spanner"
 
 
-@pytest.fixture(autouse=False)
+@pytest.fixture(scope="session")
+def spanner_docker_ip(spanner_docker_services: DockerServiceRegistry) -> str:
+    return spanner_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def spanner_service(
-    docker_services: DockerServiceRegistry,
+    spanner_docker_services: DockerServiceRegistry,
     default_spanner_service_name: str,
-    docker_compose_files: list[Path],
-    docker_ip: str,
+    spanner_docker_compose_files: list[Path],
+    spanner_docker_ip: str,
     spanner_port: int,
     spanner_instance: str,
     spanner_database: str,
     spanner_project: str,
     spanner_credentials: Credentials,
-) -> None:
-    os.environ["SPANNER_EMULATOR_HOST"] = f"{docker_ip}:{spanner_port}"
+) -> AsyncGenerator[None, None]:
+    os.environ["SPANNER_EMULATOR_HOST"] = f"{spanner_docker_ip}:{spanner_port}"
     os.environ["SPANNER_DATABASE"] = spanner_database
     os.environ["SPANNER_INSTANCE"] = spanner_instance
     os.environ["SPANNER_PORT"] = str(spanner_port)
     os.environ["GOOGLE_CLOUD_PROJECT"] = spanner_project
-    await docker_services.start(
+    await spanner_docker_services.start(
         name=default_spanner_service_name,
-        docker_compose_files=docker_compose_files,
+        docker_compose_files=spanner_docker_compose_files,
         timeout=60,
         check=spanner_responsive,
         spanner_port=spanner_port,
         spanner_instance=spanner_instance,
         spanner_database=spanner_database,
         spanner_project=spanner_project,
         spanner_credentials=spanner_credentials,
     )
+    yield
```

### Comparing `pytest_databases-0.4.1/tests/__init__.py` & `pytest_databases-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/tests/conftest.py` & `pytest_databases-0.5.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 here = Path(__file__).parent
 root_path = here.parent
 pytest_plugins = [
     "pytest_databases.docker",
 ]
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def anyio_backend() -> str:
     return "asyncio"
```

### Comparing `pytest_databases-0.4.1/tests/docker/__init__.py` & `pytest_databases-0.5.0/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/tests/docker/test_alloydb_omni.py` & `pytest_databases-0.5.0/tests/docker/test_alloydb_omni.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,22 +48,22 @@
     assert alloydb_omni_port == 5420
     assert postgres_database == "postgres"
     assert postgres_user == "postgres"
     assert postgres_password == "super-secret"
 
 
 async def test_alloydb_omni_services(
-    docker_ip: str,
+    alloydb_docker_ip: str,
     alloydb_omni_service: DockerServiceRegistry,
     alloydb_omni_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await alloydb_omni_responsive(
-        docker_ip,
+        alloydb_docker_ip,
         port=alloydb_omni_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_bigquery.py` & `pytest_databases-0.5.0/tests/docker/test_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,39 +37,39 @@
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
     "pytest_databases.docker.bigquery",
 ]
 
 
 def test_bigquery_default_config(
-    docker_ip: str,
+    bigquery_docker_ip: str,
     bigquery_port: int,
     bigquery_grpc_port: int,
     bigquery_dataset: str,
     bigquery_endpoint: str,
     bigquery_project: str,
 ) -> None:
     assert bigquery_port == 9051
     assert bigquery_grpc_port == 9061
     assert bigquery_dataset == "test-dataset"
-    assert bigquery_endpoint == f"http://{docker_ip}:9051"
+    assert bigquery_endpoint == f"http://{bigquery_docker_ip}:9051"
     assert bigquery_project == "emulator-test-project"
 
 
 async def test_bigquery_services(
-    docker_ip: str,
+    bigquery_docker_ip: str,
     bigquery_service: DockerServiceRegistry,
     bigquery_endpoint: str,
     bigquery_dataset: str,
     bigquery_client_options: ClientOptions,
     bigquery_project: str,
     bigquery_credentials: Credentials,
 ) -> None:
     ping = await bigquery_responsive(
-        docker_ip,
+        bigquery_docker_ip,
         bigquery_endpoint=bigquery_endpoint,
         bigquery_dataset=bigquery_dataset,
         bigquery_project=bigquery_project,
         bigquery_credentials=bigquery_credentials,
         bigquery_client_options=bigquery_client_options,
     )
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_cockroachdb.py` & `pytest_databases-0.5.0/tests/docker/test_cockroachdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 ) -> None:
     assert cockroachdb_port == 26257
     assert cockroachdb_database == "defaultdb"
     assert cockroachdb_driver_opts == {"sslmode": "disable"}
 
 
 async def test_cockroachdb_service(
-    docker_ip: str,
+    cockroachdb_docker_ip: str,
     cockroachdb_service: DockerServiceRegistry,
     cockroachdb_database: str,
     cockroachdb_port: int,
     cockroachdb_driver_opts: dict[str, str],
 ) -> None:
-    ping = await cockroachdb_responsive(docker_ip, cockroachdb_port, cockroachdb_database, cockroachdb_driver_opts)
+    ping = await cockroachdb_responsive(
+        cockroachdb_docker_ip, cockroachdb_port, cockroachdb_database, cockroachdb_driver_opts
+    )
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_dragonfly.py` & `pytest_databases-0.5.0/tests/docker/test_dragonfly.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,13 +39,13 @@
 
 
 def test_dragonfly_default_config(dragonfly_port: int) -> None:
     assert dragonfly_port == 6398
 
 
 async def test_dragonfly_service(
-    docker_ip: str,
+    dragonfly_docker_ip: str,
     dragonfly_service: DockerServiceRegistry,
     dragonfly_port: int,
 ) -> None:
-    ping = await dragonfly_responsive(docker_ip, dragonfly_port)
+    ping = await dragonfly_responsive(dragonfly_docker_ip, dragonfly_port)
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_elasticsearch.py` & `pytest_databases-0.5.0/src/pytest_databases/docker/elastic_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,149 +19,184 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable
-from unittest import mock
+import os
+import sys
+from pathlib import Path
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import pytest
 from elasticsearch7 import AsyncElasticsearch as Elasticsearch7
-from elasticsearch8 import AsyncElasticsearch as Elasticsearch8
+from elasticsearch7 import AsyncElasticsearch as Elasticsearch8
 
-from pytest_databases.docker.elastic_search import elasticsearch7_responsive, elasticsearch8_responsive
+from pytest_databases.docker import DockerServiceRegistry
+from pytest_databases.helpers import simple_string_hash
 
 if TYPE_CHECKING:
-    from pathlib import Path
+    from collections.abc import Generator
 
-    from pytest_databases.docker import DockerServiceRegistry
 
-pytestmark = pytest.mark.anyio
-pytest_plugins = [
-    "pytest_databases.docker.elastic_search",
-]
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-elasticsearch-{simple_string_hash(__file__)}"
 
 
-@pytest.fixture
+async def elasticsearch7_responsive(scheme: str, host: str, port: int, user: str, password: str, database: str) -> bool:
+    try:
+        async with Elasticsearch7(
+            hosts=[{"host": host, "port": port, "scheme": scheme}], verify_certs=False, http_auth=(user, password)
+        ) as client:
+            return await client.ping()
+    except Exception:  # noqa: BLE001
+        return False
+
+
+async def elasticsearch8_responsive(scheme: str, host: str, port: int, user: str, password: str, database: str) -> bool:
+    try:
+        async with Elasticsearch8(
+            hosts=[{"host": host, "port": port, "scheme": scheme}], verify_certs=False, basic_auth=(user, password)
+        ) as client:
+            return await client.ping()
+    except Exception:  # noqa: BLE001
+        return False
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(autouse=False, scope="session")
+def elasticsearch_docker_services(
+    elasticsearch_compose_project_name: str, worker_id: str = "main"
+) -> Generator[DockerServiceRegistry, None, None]:
+    if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
+        pytest.skip("Docker not available on this platform")
+
+    registry = DockerServiceRegistry(worker_id, compose_project_name=elasticsearch_compose_project_name)
+    try:
+        yield registry
+    finally:
+        registry.down()
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_user() -> str:
+    return "elastic"
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_password() -> str:
+    return "changeme"
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_database() -> str:
+    return "db"
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_scheme() -> str:
+    return "http"
+
+
+@pytest.fixture(scope="session")
+def elasticsearch7_port() -> int:
+    return 9200
+
+
+@pytest.fixture(scope="session")
+def elasticsearch8_port() -> int:
+    return 9201
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.elasticsearch.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_elasticsearch_service_name() -> str:
+    return "elasticsearch8"
+
+
+@pytest.fixture(scope="session")
+def elasticsearch_docker_ip(elasticsearch_docker_services: DockerServiceRegistry) -> str:
+    return elasticsearch_docker_services.docker_ip
+
+
+@pytest.fixture(autouse=False, scope="session")
 async def elasticsearch7_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    elasticsearch_docker_services: DockerServiceRegistry,
+    elasticsearch_docker_compose_files: list[Path],
     elasticsearch7_port: int,
     elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
-) -> AsyncGenerator[Any, Any]:
-    """Overwrites fixture to stop container after the test."""
-    try:
-        await docker_services.start(
-            "elasticsearch7",
-            docker_compose_files=docker_compose_files,
-            timeout=45,
-            pause=1,
-            check=elasticsearch7_responsive,
-            port=elasticsearch7_port,
-            database=elasticsearch_database,
-            user=elasticsearch_user,
-            password=elasticsearch_password,
-            scheme=elasticsearch_scheme,
-        )
-        yield
-    finally:
-        docker_services.stop("elasticsearch7")
+) -> AsyncGenerator[None, None]:
+    await elasticsearch_docker_services.start(
+        "elasticsearch7",
+        docker_compose_files=elasticsearch_docker_compose_files,
+        timeout=45,
+        pause=1,
+        check=elasticsearch7_responsive,
+        port=elasticsearch7_port,
+        database=elasticsearch_database,
+        user=elasticsearch_user,
+        password=elasticsearch_password,
+        scheme=elasticsearch_scheme,
+    )
+    yield
 
 
-@pytest.fixture
+@pytest.fixture(autouse=False, scope="session")
 async def elasticsearch8_service(
-    docker_services: DockerServiceRegistry,
-    docker_compose_files: list[Path],
+    elasticsearch_docker_services: DockerServiceRegistry,
+    elasticsearch_docker_compose_files: list[Path],
     elasticsearch8_port: int,
     elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
-) -> AsyncGenerator[Any, Any]:
-    """Overwrites fixture to stop container after the test."""
-    try:
-        await docker_services.start(
-            "elasticsearch8",
-            docker_compose_files=docker_compose_files,
-            timeout=45,
-            pause=1,
-            check=elasticsearch8_responsive,
-            port=elasticsearch8_port,
-            database=elasticsearch_database,
-            user=elasticsearch_user,
-            password=elasticsearch_password,
-            scheme=elasticsearch_scheme,
-        )
-        yield
-    finally:
-        docker_services.stop("elasticsearch8")
-
-
-def test_elasticsearch7_default_config(
-    elasticsearch7_port: str, elasticsearch_user: str, elasticsearch_password: str, elasticsearch_scheme: str
-) -> None:
-    assert elasticsearch7_port == 9200
-    assert elasticsearch_user == "elastic"
-    assert elasticsearch_password == "changeme"
-    assert elasticsearch_scheme == "http"
-
-
-def test_elasticsearch8_default_config(
-    elasticsearch8_port: str, elasticsearch_user: str, elasticsearch_password: str, elasticsearch_scheme: str
-) -> None:
-    assert elasticsearch8_port == 9201
-    assert elasticsearch_user == "elastic"
-    assert elasticsearch_password == "changeme"
-    assert elasticsearch_scheme == "http"
-
-
-async def test_elasticsearch7_service(
-    docker_ip: str,
-    elasticsearch7_service: DockerServiceRegistry,
-    elasticsearch7_port: str,
-    elasticsearch_user: str,
-    elasticsearch_password: str,
-    elasticsearch_scheme: str,
-) -> None:
-    async with Elasticsearch7(
-        hosts=[{"host": docker_ip, "port": elasticsearch7_port, "scheme": elasticsearch_scheme}],
-        verify_certs=False,
-        http_auth=(elasticsearch_user, elasticsearch_password),
-    ) as client:
-        info = await client.info()
-
-    assert info["version"]["number"] == "7.17.19"
-
-
-async def test_elasticsearch8_service(
-    docker_ip: str,
-    elasticsearch8_service: DockerServiceRegistry,
-    elasticsearch8_port: str,
+) -> AsyncGenerator[None, None]:
+    await elasticsearch_docker_services.start(
+        "elasticsearch8",
+        docker_compose_files=elasticsearch_docker_compose_files,
+        timeout=45,
+        pause=1,
+        check=elasticsearch8_responsive,
+        port=elasticsearch8_port,
+        database=elasticsearch_database,
+        user=elasticsearch_user,
+        password=elasticsearch_password,
+        scheme=elasticsearch_scheme,
+    )
+    yield
+
+
+@pytest.fixture(autouse=False, scope="session")
+async def elasticsearch_service(
+    elasticsearch_docker_services: DockerServiceRegistry,
+    default_elasticsearch_service_name: str,
+    elasticsearch_docker_compose_files: list[Path],
+    elasticsearch8_port: int,
+    elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
-) -> None:
-    async with Elasticsearch8(
-        hosts=[{"host": docker_ip, "port": elasticsearch8_port, "scheme": elasticsearch_scheme}],
-        verify_certs=False,
-        basic_auth=(elasticsearch_user, elasticsearch_password),
-    ) as client:
-        info = await client.info()
-
-    assert info["version"]["number"] == "8.13.0"
-
-
-@pytest.mark.parametrize(
-    "responsive, path_to_mock",
-    (
-        (elasticsearch7_responsive, "pytest_databases.docker.elastic_search.Elasticsearch7.ping"),
-        (elasticsearch8_responsive, "pytest_databases.docker.elastic_search.Elasticsearch8.ping"),
-    ),
-)
-async def test_elasticsearch_responsive(responsive: Callable, path_to_mock: str) -> None:
-    with mock.patch(path_to_mock, mock.Mock(side_effect=Exception)):
-        assert not await responsive(scheme="", host="", port="", user="", password="", database="")
+) -> AsyncGenerator[None, None]:
+    await elasticsearch_docker_services.start(
+        name=default_elasticsearch_service_name,
+        docker_compose_files=elasticsearch_docker_compose_files,
+        timeout=45,
+        pause=1,
+        check=elasticsearch8_responsive,
+        port=elasticsearch8_port,
+        database=elasticsearch_database,
+        user=elasticsearch_user,
+        password=elasticsearch_password,
+        scheme=elasticsearch_scheme,
+    )
+    yield
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_keydb.py` & `pytest_databases-0.5.0/tests/docker/test_redis.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import pytest
 
-from pytest_databases.docker.keydb import keydb_responsive
+from pytest_databases.docker.redis import redis_responsive
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
 
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
-    "pytest_databases.docker.keydb",
+    "pytest_databases.docker.redis",
 ]
 
 
-def test_keydb_default_config(keydb_port: int) -> None:
-    assert keydb_port == 6396
+def test_redis_default_config(redis_port: int) -> None:
+    assert redis_port == 6397
 
 
-async def test_keydb_service(
-    docker_ip: str,
-    keydb_service: DockerServiceRegistry,
-    keydb_port: int,
+async def test_redis_service(
+    redis_docker_ip: str,
+    redis_service: DockerServiceRegistry,
+    redis_port: int,
 ) -> None:
-    ping = await keydb_responsive(docker_ip, keydb_port)
+    ping = await redis_responsive(redis_docker_ip, redis_port)
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_mariadb.py` & `pytest_databases-0.5.0/tests/docker/test_mariadb.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,40 +60,40 @@
     assert mariadb113_port == 3359
     assert mariadb_database == "db"
     assert mariadb_user == "app"
     assert mariadb_password == "super-secret"
 
 
 async def test_mariadb_services(
-    docker_ip: str,
+    mariadb_docker_ip: str,
     mariadb_service: DockerServiceRegistry,
     mariadb_port: int,
     mariadb_database: str,
     mariadb_user: str,
     mariadb_password: str,
 ) -> None:
     ping = await mariadb_responsive(
-        docker_ip,
+        mariadb_docker_ip,
         port=mariadb_port,
         database=mariadb_database,
         user=mariadb_user,
         password=mariadb_password,
     )
     assert ping
 
 
 async def test_mariadb_113_services(
-    docker_ip: str,
+    mariadb_docker_ip: str,
     mariadb113_service: DockerServiceRegistry,
     mariadb113_port: int,
     mariadb_database: str,
     mariadb_user: str,
     mariadb_password: str,
 ) -> None:
     ping = await mariadb_responsive(
-        docker_ip,
+        mariadb_docker_ip,
         port=mariadb113_port,
         database=mariadb_database,
         user=mariadb_user,
         password=mariadb_password,
     )
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_mssql.py` & `pytest_databases-0.5.0/tests/docker/test_mssql.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,32 +81,32 @@
     assert mssql2022_port == 4133
     assert mssql_database == "master"
     assert mssql_user == "sa"
     assert mssql_password == "Super-secret1"
 
 
 async def test_mssql_services(
-    docker_ip: str,
+    mssql_docker_ip: str,
     mssql_service: DockerServiceRegistry,
     mssql_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
 ) -> None:
-    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={docker_ip},{mssql_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
+    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={mssql_docker_ip},{mssql_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
 
-    ping = await mssql_responsive(docker_ip, connstring=connstring)
+    ping = await mssql_responsive(mssql_docker_ip, connstring=connstring)
     assert ping
 
 
 async def test_mssql_2022_services(
-    docker_ip: str,
+    mssql_docker_ip: str,
     mssql2022_service: DockerServiceRegistry,
     mssql2022_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
 ) -> None:
-    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={docker_ip},{mssql2022_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
+    connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={mssql_docker_ip},{mssql2022_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
 
-    ping = await mssql_responsive(docker_ip, connstring=connstring)
+    ping = await mssql_responsive(mssql_docker_ip, connstring=connstring)
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_mysql.py` & `pytest_databases-0.5.0/tests/docker/test_mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,76 +84,76 @@
     assert mysql56_port == 3362
     assert mysql_database == "db"
     assert mysql_user == "app"
     assert mysql_password == "super-secret"
 
 
 async def test_mysql_services(
-    docker_ip: str,
+    mysql_docker_ip: str,
     mysql_service: DockerServiceRegistry,
     mysql_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
 ) -> None:
     ping = await mysql_responsive(
-        docker_ip,
+        mysql_docker_ip,
         port=mysql_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
     assert ping
 
 
 async def test_mysql_57_services(
-    docker_ip: str,
+    mysql_docker_ip: str,
     mysql57_service: DockerServiceRegistry,
     mysql57_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
 ) -> None:
     ping = await mysql_responsive(
-        docker_ip,
+        mysql_docker_ip,
         port=mysql57_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
     assert ping
 
 
 async def test_mysql_56_services(
-    docker_ip: str,
+    mysql_docker_ip: str,
     mysql56_service: DockerServiceRegistry,
     mysql56_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
 ) -> None:
     ping = await mysql_responsive(
-        docker_ip,
+        mysql_docker_ip,
         port=mysql56_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
     assert ping
 
 
 async def test_mysql_8_services(
-    docker_ip: str,
+    mysql_docker_ip: str,
     mysql8_service: DockerServiceRegistry,
     mysql8_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
 ) -> None:
     ping = await mysql_responsive(
-        docker_ip,
+        mysql_docker_ip,
         port=mysql8_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_oracle.py` & `pytest_databases-0.5.0/tests/docker/test_oracle.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,38 +68,42 @@
     assert oracle_password == "super-secret"
     assert oracle_service_name == "FREEPDB1"
     assert oracle_port == 1513
     assert oracle_port == oracle23c_port
 
 
 async def test_oracle18c_service(
-    docker_ip: str,
+    oracle_docker_ip: str,
     oracle18c_service: DockerServiceRegistry,
     oracle18c_service_name: str,
     oracle18c_port: int,
     oracle_user: str,
     oracle_password: str,
 ) -> None:
     conn = oracledb.connect(
-        user=oracle_user, password=oracle_password, dsn=f"{docker_ip}:{oracle18c_port!s}/{oracle18c_service_name}"
+        user=oracle_user,
+        password=oracle_password,
+        dsn=f"{oracle_docker_ip}:{oracle18c_port!s}/{oracle18c_service_name}",
     )
     with conn.cursor() as cur:
         cur.execute("SELECT 'Hello World!' FROM dual")
         res = cur.fetchall()[0][0]
         assert "Hello World!" in res
 
 
 async def test_oracle23c_service(
-    docker_ip: str,
+    oracle_docker_ip: str,
     oracle23c_service: DockerServiceRegistry,
     oracle23c_service_name: str,
     oracle23c_port: int,
     oracle_user: str,
     oracle_password: str,
 ) -> None:
     conn = oracledb.connect(
-        user=oracle_user, password=oracle_password, dsn=f"{docker_ip}:{oracle23c_port!s}/{oracle23c_service_name}"
+        user=oracle_user,
+        password=oracle_password,
+        dsn=f"{oracle_docker_ip}:{oracle23c_port!s}/{oracle23c_service_name}",
     )
     with conn.cursor() as cur:
         cur.execute("SELECT 'Hello World!' FROM dual")
         res = cur.fetchall()[0][0]
         assert "Hello World!" in res
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_postgres.py` & `pytest_databases-0.5.0/tests/docker/test_postgres.py`

 * *Files 11% similar despite different names*

```diff
@@ -108,112 +108,112 @@
     assert postgres16_port == 5427
     assert postgres_database == "postgres"
     assert postgres_user == "postgres"
     assert postgres_password == "super-secret"
 
 
 async def test_postgres_services(
-    docker_ip: str,
+    postgres_docker_ip: str,
     postgres_service: DockerServiceRegistry,
     postgres_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await postgres_responsive(
-        docker_ip,
+        postgres_docker_ip,
         port=postgres_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
 
 
 async def test_postgres_12_services(
-    docker_ip: str,
+    postgres_docker_ip: str,
     postgres12_service: DockerServiceRegistry,
     postgres12_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await postgres_responsive(
-        docker_ip,
+        postgres_docker_ip,
         port=postgres12_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
 
 
 async def test_postgres_13_services(
-    docker_ip: str,
+    postgres_docker_ip: str,
     postgres13_service: DockerServiceRegistry,
     postgres13_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await postgres_responsive(
-        docker_ip,
+        postgres_docker_ip,
         port=postgres13_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
 
 
 async def test_postgres_14_services(
-    docker_ip: str,
+    postgres_docker_ip: str,
     postgres14_service: DockerServiceRegistry,
     postgres14_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await postgres_responsive(
-        docker_ip,
+        postgres_docker_ip,
         port=postgres14_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
 
 
 async def test_postgres_15_services(
-    docker_ip: str,
+    postgres_docker_ip: str,
     postgres15_service: DockerServiceRegistry,
     postgres15_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await postgres_responsive(
-        docker_ip,
+        postgres_docker_ip,
         port=postgres15_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
 
 
 async def test_postgres_16_services(
-    docker_ip: str,
+    postgres_docker_ip: str,
     postgres16_service: DockerServiceRegistry,
     postgres16_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     ping = await postgres_responsive(
-        docker_ip,
+        postgres_docker_ip,
         port=postgres16_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
     assert ping
```

### Comparing `pytest_databases-0.4.1/tests/docker/test_spanner.py` & `pytest_databases-0.5.0/tests/docker/test_spanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,24 @@
     assert spanner_port == 9010
     assert spanner_instance == "test-instance"
     assert spanner_database == "test-database"
     assert spanner_project == "emulator-test-project"
 
 
 async def test_spanner_services(
-    docker_ip: str,
+    spanner_docker_ip: str,
     spanner_service: DockerServiceRegistry,
     spanner_port: int,
     spanner_instance: str,
     spanner_database: str,
     spanner_project: str,
     spanner_credentials: Credentials,
 ) -> None:
     ping = spanner_responsive(
-        docker_ip,
+        spanner_docker_ip,
         spanner_port=spanner_port,
         spanner_instance=spanner_instance,
         spanner_database=spanner_database,
         spanner_project=spanner_project,
         spanner_credentials=spanner_credentials,
     )
     assert ping
```

### Comparing `pytest_databases-0.4.1/.gitignore` & `pytest_databases-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/LICENSE` & `pytest_databases-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/README.md` & `pytest_databases-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.1/pyproject.toml` & `pytest_databases-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.1"
+version = "0.5.0"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
```

### Comparing `pytest_databases-0.4.1/PKG-INFO` & `pytest_databases-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-databases
-Version: 0.4.1
+Version: 0.5.0
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

