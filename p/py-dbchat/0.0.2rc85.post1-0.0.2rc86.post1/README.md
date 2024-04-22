# Comparing `tmp/py_dbchat-0.0.2rc85.post1.tar.gz` & `tmp/py_dbchat-0.0.2rc86.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dbchat-0.0.2rc85.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_dbchat-0.0.2rc86.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_dbchat-0.0.2rc85.post1.tar` & `py_dbchat-0.0.2rc86.post1.tar`

### file list

```diff
@@ -1,103 +1,111 @@
--rw-r--r--   0        0        0   600200 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      462 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1822 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      843 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0      417 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.gitignore
--rw-r--r--   0        0        0     1381 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.pypirc
--rw-r--r--   0        0        0      791 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1213 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/LICENSE
--rw-r--r--   0        0        0       41 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/README.md
--rw-r--r--   0        0        0     2780 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/SUPPORT.md
--rw-r--r--   0        0        0      655 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/Test.session.sql
--rw-r--r--   0        0        0      634 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/make.bat
--rw-r--r--   0        0        0       50 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/pyproject.md
--rw-r--r--   0        0        0      423 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/python_package.rst
--rw-r--r--   0        0        0       65 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/workflows.md
--rw-r--r--   0        0        0      274 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/main.py
--rw-r--r--   0        0        0      203 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/playground.py
--rw-r--r--   0        0        0     6679 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/pyproject.toml
--rw-r--r--   0        0        0       70 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/requirements.txt
--rw-r--r--   0        0        0      109 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/README.md
--rw-r--r--   0        0        0      161 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/Roadmap.md
--rw-r--r--   0        0        0        0 2024-04-22 01:39:16.116345 py_dbchat-0.0.2rc85.post1/src/api/__init__.py
--rw-r--r--   0        0        0     3110 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/database/repository.py
--rw-r--r--   0        0        0      637 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/dependencies.py
--rw-r--r--   0        0        0        0 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/internal/__init__.py
--rw-r--r--   0        0        0      146 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/internal/admin.py
--rw-r--r--   0        0        0      807 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/main.py
--rw-r--r--   0        0        0      272 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/models/AppSettings.py
--rw-r--r--   0        0        0        0 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/models/__init__.py
--rw-r--r--   0        0        0      163 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/models/model_map.py
--rw-r--r--   0        0        0        0 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/__init__.py
--rw-r--r--   0        0        0     1010 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/items.py
--rw-r--r--   0        0        0     1319 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/settings.py
--rw-r--r--   0        0        0      406 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/users.py
--rw-r--r--   0        0        0      441 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/api/settings.py
--rw-r--r--   0        0        0     6148 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/.DS_Store
--rw-r--r--   0        0        0      374 2024-04-22 01:39:16.116345 py_dbchat-0.0.2rc85.post1/src/db_chat/__init__.py
--rw-r--r--   0        0        0      725 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/ask.py
--rw-r--r--   0        0        0      662 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/hello_world.py
--rw-r--r--   0        0        0     3833 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/classic_prompt.py
--rw-r--r--   0        0        0     3518 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/function_calling.py
--rw-r--r--   0        0        0     6791 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm.py
--rw-r--r--   0        0        0     1135 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm_langchain_sample.py
--rw-r--r--   0        0        0      250 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/Filter.py
--rw-r--r--   0        0        0      236 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/FilterOperator.py
--rw-r--r--   0        0        0     2478 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/Query.py
--rw-r--r--   0        0        0      159 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/SortOrder.py
--rw-r--r--   0        0        0        0 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/__init__.py
--rw-r--r--   0        0        0      453 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/mappings.py
--rw-r--r--   0        0        0     5193 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/schema.py
--rw-r--r--   0        0        0     8781 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sql_builder.py
--rw-r--r--   0        0        0    16036 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
--rw-r--r--   0        0        0      436 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/.eslintrc.cjs
--rw-r--r--   0        0        0      253 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/.gitignore
--rw-r--r--   0        0        0     1300 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/README.md
--rw-r--r--   0        0        0      484 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/index.html
--rw-r--r--   0        0        0   118627 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/package-lock.json
--rw-r--r--   0        0        0      909 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/package.json
--rw-r--r--   0        0        0     1497 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/public/vite.svg
--rw-r--r--   0        0        0     1286 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/App.css
--rw-r--r--   0        0        0     1873 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/App.tsx
--rw-r--r--   0        0        0     3200 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/api/baseApi.ts
--rw-r--r--   0        0        0     4126 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/assets/react.svg
--rw-r--r--   0        0        0     1161 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/index.css
--rw-r--r--   0        0        0      236 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/main.tsx
--rw-r--r--   0        0        0     1101 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/store/appSettingStore.ts
--rw-r--r--   0        0        0       83 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/types/Setting.ts
--rw-r--r--   0        0        0       64 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/types/schema.ts
--rw-r--r--   0        0        0       38 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/vite-env.d.ts
--rw-r--r--   0        0        0      605 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/tsconfig.json
--rw-r--r--   0        0        0      233 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/tsconfig.node.json
--rw-r--r--   0        0        0      167 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/vite.config.ts
--rw-r--r--   0        0        0   600200 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/test/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      989 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/conftest.py
--rw-r--r--   0        0        0     2922 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_explicit_joins.py
--rw-r--r--   0        0        0     1210 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_methods.py
--rw-r--r--   0        0        0      269 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_schema_builder.py
--rw-r--r--   0        0        0    12288 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_sql_builder.py
--rw-r--r--   0        0        0     7124 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc85.post1/PKG-INFO
+-rw-r--r--   0        0        0   600200 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.devcontainer/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      462 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1822 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      843 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0      417 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.gitignore
+-rw-r--r--   0        0        0     1381 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.pypirc
+-rw-r--r--   0        0        0      791 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1213 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/LICENSE
+-rw-r--r--   0        0        0       41 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/SUPPORT.md
+-rw-r--r--   0        0        0      655 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/Test.session.sql
+-rw-r--r--   0        0        0      634 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/make.bat
+-rw-r--r--   0        0        0       50 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      423 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       65 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/docs/workflows.md
+-rw-r--r--   0        0        0      274 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/main.py
+-rw-r--r--   0        0        0     3399 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/package-lock.json
+-rw-r--r--   0        0        0       62 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/package.json
+-rw-r--r--   0        0        0      203 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/playground.py
+-rw-r--r--   0        0        0     6679 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/requirements.txt
+-rw-r--r--   0        0        0      109 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/README.md
+-rw-r--r--   0        0        0      161 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/Roadmap.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:46:29.142677 py_dbchat-0.0.2rc86.post1/src/api/__init__.py
+-rw-r--r--   0        0        0     3110 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/api/database/repository.py
+-rw-r--r--   0        0        0      637 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/api/dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/api/internal/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/api/internal/admin.py
+-rw-r--r--   0        0        0      807 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/api/main.py
+-rw-r--r--   0        0        0      272 2024-04-22 03:46:16.898694 py_dbchat-0.0.2rc86.post1/src/api/models/AppSettings.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/models/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/models/model_map.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/routers/__init__.py
+-rw-r--r--   0        0        0     1010 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/routers/items.py
+-rw-r--r--   0        0        0     1319 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/routers/settings.py
+-rw-r--r--   0        0        0      406 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/routers/users.py
+-rw-r--r--   0        0        0      441 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/api/settings.py
+-rw-r--r--   0        0        0     6148 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/.DS_Store
+-rw-r--r--   0        0        0      374 2024-04-22 03:46:29.142677 py_dbchat-0.0.2rc86.post1/src/db_chat/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/ask.py
+-rw-r--r--   0        0        0      662 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/hello_world.py
+-rw-r--r--   0        0        0     3833 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/llm/classic_prompt.py
+-rw-r--r--   0        0        0     3518 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/llm/function_calling.py
+-rw-r--r--   0        0        0     6791 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/llm/llm.py
+-rw-r--r--   0        0        0     1135 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/llm/llm_langchain_sample.py
+-rw-r--r--   0        0        0      250 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/Filter.py
+-rw-r--r--   0        0        0      236 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/FilterOperator.py
+-rw-r--r--   0        0        0     2478 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/Query.py
+-rw-r--r--   0        0        0      159 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/SortOrder.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/mappings.py
+-rw-r--r--   0        0        0     5193 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/schema.py
+-rw-r--r--   0        0        0     8781 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/sql_builder.py
+-rw-r--r--   0        0        0    16036 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
+-rw-r--r--   0        0        0      436 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/.eslintrc.cjs
+-rw-r--r--   0        0        0      253 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/.gitignore
+-rw-r--r--   0        0        0     1300 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/README.md
+-rw-r--r--   0        0        0      484 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/index.html
+-rw-r--r--   0        0        0   120043 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/package-lock.json
+-rw-r--r--   0        0        0      944 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/package.json
+-rw-r--r--   0        0        0     1497 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/public/vite.svg
+-rw-r--r--   0        0        0     1286 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/App.css
+-rw-r--r--   0        0        0     1129 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/App.tsx
+-rw-r--r--   0        0        0     3200 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/api/baseApi.ts
+-rw-r--r--   0        0        0     4126 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/assets/react.svg
+-rw-r--r--   0        0        0      557 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/components/menu/menu.tsx
+-rw-r--r--   0        0        0     1161 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/index.css
+-rw-r--r--   0        0        0      236 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/main.tsx
+-rw-r--r--   0        0        0     1085 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/pages/home/home.tsx
+-rw-r--r--   0        0        0      861 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/pages/settings/settings.tsx
+-rw-r--r--   0        0        0     1101 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/store/appSettingStore.ts
+-rw-r--r--   0        0        0      606 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/store/uiStore.ts
+-rw-r--r--   0        0        0       83 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/types/Setting.ts
+-rw-r--r--   0        0        0       40 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/types/index.ts
+-rw-r--r--   0        0        0       84 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/types/menu.ts
+-rw-r--r--   0        0        0       64 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/types/schema.ts
+-rw-r--r--   0        0        0       38 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/tsconfig.node.json
+-rw-r--r--   0        0        0      167 2024-04-22 03:46:16.902694 py_dbchat-0.0.2rc86.post1/src/ui/vite.config.ts
+-rw-r--r--   0        0        0   600200 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/test/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      989 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2922 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/tests/test_explicit_joins.py
+-rw-r--r--   0        0        0     1210 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/tests/test_methods.py
+-rw-r--r--   0        0        0      269 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/tests/test_schema_builder.py
+-rw-r--r--   0        0        0    12288 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/tests/test_sql_builder.py
+-rw-r--r--   0        0        0     7124 2024-04-22 03:46:16.906694 py_dbchat-0.0.2rc86.post1/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc86.post1/PKG-INFO
```

### Comparing `py_dbchat-0.0.2rc85.post1/.devcontainer/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc86.post1/.devcontainer/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.devcontainer/devcontainer.json` & `py_dbchat-0.0.2rc86.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.devcontainer/docker-compose.yml` & `py_dbchat-0.0.2rc86.post1/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.github/workflows/schedule-update-actions.yml` & `py_dbchat-0.0.2rc86.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.gitignore` & `py_dbchat-0.0.2rc86.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.pre-commit-config.yaml` & `py_dbchat-0.0.2rc86.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.vscode/launch.json` & `py_dbchat-0.0.2rc86.post1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/.vscode/settings.json` & `py_dbchat-0.0.2rc86.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/LICENSE` & `py_dbchat-0.0.2rc86.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/SECURITY.md` & `py_dbchat-0.0.2rc86.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/SUPPORT.md` & `py_dbchat-0.0.2rc86.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/Test.session.sql` & `py_dbchat-0.0.2rc86.post1/Test.session.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/docs/Makefile` & `py_dbchat-0.0.2rc86.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/docs/conf.py` & `py_dbchat-0.0.2rc86.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/docs/make.bat` & `py_dbchat-0.0.2rc86.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/docs/pylint.md` & `py_dbchat-0.0.2rc86.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/pyproject.toml` & `py_dbchat-0.0.2rc86.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/api/database/repository.py` & `py_dbchat-0.0.2rc86.post1/src/api/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/api/dependencies.py` & `py_dbchat-0.0.2rc86.post1/src/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/api/main.py` & `py_dbchat-0.0.2rc86.post1/src/api/main.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/api/routers/items.py` & `py_dbchat-0.0.2rc86.post1/src/api/routers/items.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/api/routers/settings.py` & `py_dbchat-0.0.2rc86.post1/src/api/routers/settings.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/.DS_Store` & `py_dbchat-0.0.2rc86.post1/src/db_chat/.DS_Store`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/ask.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/ask.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/hello_world.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/hello_world.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/classic_prompt.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/llm/classic_prompt.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/function_calling.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/llm/llm.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm_langchain_sample.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/llm/llm_langchain_sample.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/Query.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/Query.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/schema.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/schema.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sql_builder.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py` & `py_dbchat-0.0.2rc86.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/README.md` & `py_dbchat-0.0.2rc86.post1/src/ui/README.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/package-lock.json` & `py_dbchat-0.0.2rc86.post1/src/ui/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986826223544973%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'react-router-dom': '^6.22.3'}}, "*

 * *               "'node_modules/react-router': {'version': '6.22.3', 'resolved': "*

 * *               "'https://registry.npmjs.org/react-router/-/react-router-6.22.3.tgz', 'integrity': "*

 * *               "'sha512-dr2eb3Mj5zK2YISHK++foM9w4eBnO23eKnZEDs7c880P6oKbrjz/Svg9+nxqtHQK+oMW4OtjZca0RqPglXxguQ==', "*

 * *               "'dependencies': {replace: OrderedDict([('@remix-run/router', '1.15.3')])}, "*

 * *               "'peerDependencies': {'react': ' […]*

```diff
@@ -6,14 +6,15 @@
             "dependencies": {
                 "@popperjs/core": "^2.11.8",
                 "bootstrap": "^5.3.3",
                 "boxicons": "^2.1.4",
                 "react": "^18.2.0",
                 "react-bootstrap": "^2.10.2",
                 "react-dom": "^18.2.0",
+                "react-router-dom": "^6.22.3",
                 "zustand": "^4.5.2"
             },
             "devDependencies": {
                 "@types/react": "^18.2.66",
                 "@types/react-dom": "^18.2.22",
                 "@typescript-eslint/eslint-plugin": "^7.2.0",
                 "@typescript-eslint/parser": "^7.2.0",
@@ -603,14 +604,22 @@
             "integrity": "sha512-0gKkgDYdnq1w+ey8KzG9l+H5Z821qh9vVjztk55rUg71vTk/Eaebeir+WtzcLLwTjw3m/asIjx8Y59y1lJZhBw==",
             "peerDependencies": {
                 "react": "^16.8.0 || ^17.0.0-rc.1 || ^18.0.0"
             },
             "resolved": "https://registry.npmjs.org/@react-aria/ssr/-/ssr-3.9.2.tgz",
             "version": "3.9.2"
         },
+        "node_modules/@remix-run/router": {
+            "engines": {
+                "node": ">=14.0.0"
+            },
+            "integrity": "sha512-Oy8rmScVrVxWZVOpEF57ovlnhpZ8CCPlnIIumVcV9nFdiSIrus99+Lw78ekXyGvVDlIsFJbSfmSovJUhCWYV3w==",
+            "resolved": "https://registry.npmjs.org/@remix-run/router/-/router-1.15.3.tgz",
+            "version": "1.15.3"
+        },
         "node_modules/@restart/hooks": {
             "dependencies": {
                 "dequal": "^2.0.3"
             },
             "integrity": "sha512-f7aCv7c+nU/3mF7NWLtVVr0Ra80RqsO89hO72r+Y/nvQr5+q0UFGkocElTH6MJApvReVh6JHUFYn2cw1WdHF3w==",
             "peerDependencies": {
                 "react": ">=16.8.0"
@@ -1503,14 +1512,47 @@
             "integrity": "sha512-1gCeQXDLoIqMgqD3IO2Ah9bnf0w9kzhwN5q4FGnHZ67hBm9yePzB5JJAIQCc8x3pFnNlwFq4RidZggNAAkzWWw==",
             "peerDependencies": {
                 "react": "^16.14.0"
             },
             "resolved": "https://registry.npmjs.org/react-dom/-/react-dom-16.14.0.tgz",
             "version": "16.14.0"
         },
+        "node_modules/boxicons/node_modules/react-router": {
+            "dependencies": {
+                "history": "^4.7.2",
+                "hoist-non-react-statics": "^2.5.0",
+                "invariant": "^2.2.4",
+                "loose-envify": "^1.3.1",
+                "path-to-regexp": "^1.7.0",
+                "prop-types": "^15.6.1",
+                "warning": "^4.0.1"
+            },
+            "integrity": "sha512-yrvL8AogDh2X42Dt9iknk4wF4V8bWREPirFfS9gLU1huk6qK41sg7Z/1S81jjTrGHxa3B8R3J6xIkDAA6CVarg==",
+            "peerDependencies": {
+                "react": ">=15"
+            },
+            "resolved": "https://registry.npmjs.org/react-router/-/react-router-4.3.1.tgz",
+            "version": "4.3.1"
+        },
+        "node_modules/boxicons/node_modules/react-router-dom": {
+            "dependencies": {
+                "history": "^4.7.2",
+                "invariant": "^2.2.4",
+                "loose-envify": "^1.3.1",
+                "prop-types": "^15.6.1",
+                "react-router": "^4.3.1",
+                "warning": "^4.0.1"
+            },
+            "integrity": "sha512-c/MlywfxDdCp7EnB7YfPMOfMD3tOtIjrQlj/CKfNMBxdmpJP8xcz5P/UAFn3JbnQCNUxsHyVVqllF9LhgVyFCA==",
+            "peerDependencies": {
+                "react": ">=15"
+            },
+            "resolved": "https://registry.npmjs.org/react-router-dom/-/react-router-dom-4.3.1.tgz",
+            "version": "4.3.1"
+        },
         "node_modules/boxicons/node_modules/scheduler": {
             "dependencies": {
                 "loose-envify": "^1.1.0",
                 "object-assign": "^4.1.1"
             },
             "integrity": "sha512-n/zwRWRYSUj0/3g/otKDRPMh6qv2SYMWNq85IEa8iZyAv8od9zDYpGSnpBEjNgcMNq6Scbu5KfIPxNF72R/2EA==",
             "resolved": "https://registry.npmjs.org/scheduler/-/scheduler-0.19.1.tgz",
@@ -2835,44 +2877,41 @@
         "node_modules/react-lifecycles-compat": {
             "integrity": "sha512-fBASbA6LnOU9dOU2eW7aQ8xmYBSXUIWr+UmF9b1efZBazGNO+rcXT/icdKnYm2pTwcRylVUYwW7H1PHfLekVzA==",
             "resolved": "https://registry.npmjs.org/react-lifecycles-compat/-/react-lifecycles-compat-3.0.4.tgz",
             "version": "3.0.4"
         },
         "node_modules/react-router": {
             "dependencies": {
-                "history": "^4.7.2",
-                "hoist-non-react-statics": "^2.5.0",
-                "invariant": "^2.2.4",
-                "loose-envify": "^1.3.1",
-                "path-to-regexp": "^1.7.0",
-                "prop-types": "^15.6.1",
-                "warning": "^4.0.1"
+                "@remix-run/router": "1.15.3"
             },
-            "integrity": "sha512-yrvL8AogDh2X42Dt9iknk4wF4V8bWREPirFfS9gLU1huk6qK41sg7Z/1S81jjTrGHxa3B8R3J6xIkDAA6CVarg==",
+            "engines": {
+                "node": ">=14.0.0"
+            },
+            "integrity": "sha512-dr2eb3Mj5zK2YISHK++foM9w4eBnO23eKnZEDs7c880P6oKbrjz/Svg9+nxqtHQK+oMW4OtjZca0RqPglXxguQ==",
             "peerDependencies": {
-                "react": ">=15"
+                "react": ">=16.8"
             },
-            "resolved": "https://registry.npmjs.org/react-router/-/react-router-4.3.1.tgz",
-            "version": "4.3.1"
+            "resolved": "https://registry.npmjs.org/react-router/-/react-router-6.22.3.tgz",
+            "version": "6.22.3"
         },
         "node_modules/react-router-dom": {
             "dependencies": {
-                "history": "^4.7.2",
-                "invariant": "^2.2.4",
-                "loose-envify": "^1.3.1",
-                "prop-types": "^15.6.1",
-                "react-router": "^4.3.1",
-                "warning": "^4.0.1"
+                "@remix-run/router": "1.15.3",
+                "react-router": "6.22.3"
             },
-            "integrity": "sha512-c/MlywfxDdCp7EnB7YfPMOfMD3tOtIjrQlj/CKfNMBxdmpJP8xcz5P/UAFn3JbnQCNUxsHyVVqllF9LhgVyFCA==",
+            "engines": {
+                "node": ">=14.0.0"
+            },
+            "integrity": "sha512-7ZILI7HjcE+p31oQvwbokjk6OA/bnFxrhJ19n82Ex9Ph8fNAq+Hm/7KchpMGlTgWhUxRHMMCut+vEtNpWpowKw==",
             "peerDependencies": {
-                "react": ">=15"
+                "react": ">=16.8",
+                "react-dom": ">=16.8"
             },
-            "resolved": "https://registry.npmjs.org/react-router-dom/-/react-router-dom-4.3.1.tgz",
-            "version": "4.3.1"
+            "resolved": "https://registry.npmjs.org/react-router-dom/-/react-router-dom-6.22.3.tgz",
+            "version": "6.22.3"
         },
         "node_modules/react-transition-group": {
             "dependencies": {
                 "@babel/runtime": "^7.5.5",
                 "dom-helpers": "^5.0.1",
                 "loose-envify": "^1.4.0",
                 "prop-types": "^15.6.2"
```

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/package.json` & `py_dbchat-0.0.2rc86.post1/src/ui/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'dependencies'": "{'react-router-dom': '^6.22.3'}"}*

```diff
@@ -2,14 +2,15 @@
     "dependencies": {
         "@popperjs/core": "^2.11.8",
         "bootstrap": "^5.3.3",
         "boxicons": "^2.1.4",
         "react": "^18.2.0",
         "react-bootstrap": "^2.10.2",
         "react-dom": "^18.2.0",
+        "react-router-dom": "^6.22.3",
         "zustand": "^4.5.2"
     },
     "devDependencies": {
         "@types/react": "^18.2.66",
         "@types/react-dom": "^18.2.22",
         "@typescript-eslint/eslint-plugin": "^7.2.0",
         "@typescript-eslint/parser": "^7.2.0",
```

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/public/vite.svg` & `py_dbchat-0.0.2rc86.post1/src/ui/public/vite.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/src/App.css` & `py_dbchat-0.0.2rc86.post1/src/ui/src/App.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/src/api/baseApi.ts` & `py_dbchat-0.0.2rc86.post1/src/ui/src/api/baseApi.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/src/assets/react.svg` & `py_dbchat-0.0.2rc86.post1/src/ui/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/src/index.css` & `py_dbchat-0.0.2rc86.post1/src/ui/src/index.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/src/store/appSettingStore.ts` & `py_dbchat-0.0.2rc86.post1/src/ui/src/store/appSettingStore.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/src/ui/tsconfig.json` & `py_dbchat-0.0.2rc86.post1/src/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/test/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc86.post1/test/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/tests/conftest.py` & `py_dbchat-0.0.2rc86.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/tests/test_explicit_joins.py` & `py_dbchat-0.0.2rc86.post1/tests/test_explicit_joins.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/tests/test_methods.py` & `py_dbchat-0.0.2rc86.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/tests/test_sql_builder.py` & `py_dbchat-0.0.2rc86.post1/tests/test_sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/tests/test_sqlalchemy.py` & `py_dbchat-0.0.2rc86.post1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc85.post1/PKG-INFO` & `py_dbchat-0.0.2rc86.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbchat
-Version: 0.0.2rc85.post1
+Version: 0.0.2rc86.post1
 Summary: Chat with your existing database without using vector DB.
 Author-email: Dhanilan <mail2dhanilan@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

