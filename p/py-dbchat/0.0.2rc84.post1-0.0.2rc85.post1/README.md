# Comparing `tmp/py_dbchat-0.0.2rc84.post1.tar.gz` & `tmp/py_dbchat-0.0.2rc85.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dbchat-0.0.2rc84.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_dbchat-0.0.2rc85.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_dbchat-0.0.2rc84.post1.tar` & `py_dbchat-0.0.2rc85.post1.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0   600200 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.devcontainer/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      462 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1822 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      843 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0      417 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.gitignore
--rw-r--r--   0        0        0     1381 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.pypirc
--rw-r--r--   0        0        0      791 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1213 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/LICENSE
--rw-r--r--   0        0        0       41 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/README.md
--rw-r--r--   0        0        0     2780 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/SUPPORT.md
--rw-r--r--   0        0        0      655 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/Test.session.sql
--rw-r--r--   0        0        0      634 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/make.bat
--rw-r--r--   0        0        0       50 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/pyproject.md
--rw-r--r--   0        0        0      423 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/python_package.rst
--rw-r--r--   0        0        0       65 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/docs/workflows.md
--rw-r--r--   0        0        0      274 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/main.py
--rw-r--r--   0        0        0      203 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/playground.py
--rw-r--r--   0        0        0     6679 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/pyproject.toml
--rw-r--r--   0        0        0       70 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/requirements.txt
--rw-r--r--   0        0        0      109 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/README.md
--rw-r--r--   0        0        0      161 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/Roadmap.md
--rw-r--r--   0        0        0        0 2024-04-21 12:18:19.719412 py_dbchat-0.0.2rc84.post1/src/api/__init__.py
--rw-r--r--   0        0        0     3110 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/database/repository.py
--rw-r--r--   0        0        0      637 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/dependencies.py
--rw-r--r--   0        0        0        0 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/internal/__init__.py
--rw-r--r--   0        0        0      146 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/internal/admin.py
--rw-r--r--   0        0        0      609 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/main.py
--rw-r--r--   0        0        0      272 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/models/AppSettings.py
--rw-r--r--   0        0        0        0 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/models/__init__.py
--rw-r--r--   0        0        0      163 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/models/model_map.py
--rw-r--r--   0        0        0        0 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/routers/__init__.py
--rw-r--r--   0        0        0     1010 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/routers/items.py
--rw-r--r--   0        0        0     1319 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/routers/settings.py
--rw-r--r--   0        0        0      406 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/routers/users.py
--rw-r--r--   0        0        0      441 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/api/settings.py
--rw-r--r--   0        0        0     6148 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/.DS_Store
--rw-r--r--   0        0        0      374 2024-04-21 12:18:19.719412 py_dbchat-0.0.2rc84.post1/src/db_chat/__init__.py
--rw-r--r--   0        0        0      725 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/ask.py
--rw-r--r--   0        0        0      662 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/hello_world.py
--rw-r--r--   0        0        0     3833 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/llm/classic_prompt.py
--rw-r--r--   0        0        0     3518 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/llm/function_calling.py
--rw-r--r--   0        0        0     6791 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/llm/llm.py
--rw-r--r--   0        0        0     1135 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/llm/llm_langchain_sample.py
--rw-r--r--   0        0        0      250 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/Filter.py
--rw-r--r--   0        0        0      236 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/FilterOperator.py
--rw-r--r--   0        0        0     2478 2024-04-21 12:18:04.771414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/Query.py
--rw-r--r--   0        0        0      159 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/SortOrder.py
--rw-r--r--   0        0        0        0 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/__init__.py
--rw-r--r--   0        0        0      453 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/mappings.py
--rw-r--r--   0        0        0     5193 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/schema.py
--rw-r--r--   0        0        0     8781 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/sql_builder.py
--rw-r--r--   0        0        0    16036 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
--rw-r--r--   0        0        0      436 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/.eslintrc.cjs
--rw-r--r--   0        0        0      253 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/.gitignore
--rw-r--r--   0        0        0     1300 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/README.md
--rw-r--r--   0        0        0      484 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/index.html
--rw-r--r--   0        0        0   118627 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/package-lock.json
--rw-r--r--   0        0        0      909 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/package.json
--rw-r--r--   0        0        0     1497 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/public/vite.svg
--rw-r--r--   0        0        0     1286 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/App.css
--rw-r--r--   0        0        0     1345 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/App.tsx
--rw-r--r--   0        0        0     2762 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/api/baseApi.ts
--rw-r--r--   0        0        0     4126 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/assets/react.svg
--rw-r--r--   0        0        0     1161 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/index.css
--rw-r--r--   0        0        0      236 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/main.tsx
--rw-r--r--   0        0        0       83 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/types/Setting.ts
--rw-r--r--   0        0        0       64 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/types/schema.ts
--rw-r--r--   0        0        0       38 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/src/vite-env.d.ts
--rw-r--r--   0        0        0      605 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/tsconfig.json
--rw-r--r--   0        0        0      233 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/tsconfig.node.json
--rw-r--r--   0        0        0      167 2024-04-21 12:18:04.775414 py_dbchat-0.0.2rc84.post1/src/ui/vite.config.ts
--rw-r--r--   0        0        0   600200 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/test/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      989 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/tests/conftest.py
--rw-r--r--   0        0        0     2922 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/tests/test_explicit_joins.py
--rw-r--r--   0        0        0     1210 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/tests/test_methods.py
--rw-r--r--   0        0        0      269 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/tests/test_schema_builder.py
--rw-r--r--   0        0        0    12288 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/tests/test_sql_builder.py
--rw-r--r--   0        0        0     7124 2024-04-21 12:18:04.779414 py_dbchat-0.0.2rc84.post1/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc84.post1/PKG-INFO
+-rw-r--r--   0        0        0   600200 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      462 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1822 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      843 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0      417 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.gitignore
+-rw-r--r--   0        0        0     1381 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.pypirc
+-rw-r--r--   0        0        0      791 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1213 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/LICENSE
+-rw-r--r--   0        0        0       41 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/SUPPORT.md
+-rw-r--r--   0        0        0      655 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/Test.session.sql
+-rw-r--r--   0        0        0      634 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/make.bat
+-rw-r--r--   0        0        0       50 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      423 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       65 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/docs/workflows.md
+-rw-r--r--   0        0        0      274 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/main.py
+-rw-r--r--   0        0        0      203 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/playground.py
+-rw-r--r--   0        0        0     6679 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/requirements.txt
+-rw-r--r--   0        0        0      109 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/README.md
+-rw-r--r--   0        0        0      161 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/Roadmap.md
+-rw-r--r--   0        0        0        0 2024-04-22 01:39:16.116345 py_dbchat-0.0.2rc85.post1/src/api/__init__.py
+-rw-r--r--   0        0        0     3110 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/database/repository.py
+-rw-r--r--   0        0        0      637 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/internal/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/internal/admin.py
+-rw-r--r--   0        0        0      807 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/main.py
+-rw-r--r--   0        0        0      272 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/models/AppSettings.py
+-rw-r--r--   0        0        0        0 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/models/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/models/model_map.py
+-rw-r--r--   0        0        0        0 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/__init__.py
+-rw-r--r--   0        0        0     1010 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/items.py
+-rw-r--r--   0        0        0     1319 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/settings.py
+-rw-r--r--   0        0        0      406 2024-04-22 01:39:03.636242 py_dbchat-0.0.2rc85.post1/src/api/routers/users.py
+-rw-r--r--   0        0        0      441 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/api/settings.py
+-rw-r--r--   0        0        0     6148 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/.DS_Store
+-rw-r--r--   0        0        0      374 2024-04-22 01:39:16.116345 py_dbchat-0.0.2rc85.post1/src/db_chat/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/ask.py
+-rw-r--r--   0        0        0      662 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/hello_world.py
+-rw-r--r--   0        0        0     3833 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/classic_prompt.py
+-rw-r--r--   0        0        0     3518 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/function_calling.py
+-rw-r--r--   0        0        0     6791 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm.py
+-rw-r--r--   0        0        0     1135 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm_langchain_sample.py
+-rw-r--r--   0        0        0      250 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/Filter.py
+-rw-r--r--   0        0        0      236 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/FilterOperator.py
+-rw-r--r--   0        0        0     2478 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/Query.py
+-rw-r--r--   0        0        0      159 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/SortOrder.py
+-rw-r--r--   0        0        0        0 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/mappings.py
+-rw-r--r--   0        0        0     5193 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/schema.py
+-rw-r--r--   0        0        0     8781 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sql_builder.py
+-rw-r--r--   0        0        0    16036 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
+-rw-r--r--   0        0        0      436 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/.eslintrc.cjs
+-rw-r--r--   0        0        0      253 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/.gitignore
+-rw-r--r--   0        0        0     1300 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/README.md
+-rw-r--r--   0        0        0      484 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/index.html
+-rw-r--r--   0        0        0   118627 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/package-lock.json
+-rw-r--r--   0        0        0      909 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/package.json
+-rw-r--r--   0        0        0     1497 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/public/vite.svg
+-rw-r--r--   0        0        0     1286 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/App.css
+-rw-r--r--   0        0        0     1873 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/App.tsx
+-rw-r--r--   0        0        0     3200 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/api/baseApi.ts
+-rw-r--r--   0        0        0     4126 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/assets/react.svg
+-rw-r--r--   0        0        0     1161 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/index.css
+-rw-r--r--   0        0        0      236 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/main.tsx
+-rw-r--r--   0        0        0     1101 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/store/appSettingStore.ts
+-rw-r--r--   0        0        0       83 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/types/Setting.ts
+-rw-r--r--   0        0        0       64 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/types/schema.ts
+-rw-r--r--   0        0        0       38 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/tsconfig.node.json
+-rw-r--r--   0        0        0      167 2024-04-22 01:39:03.640242 py_dbchat-0.0.2rc85.post1/src/ui/vite.config.ts
+-rw-r--r--   0        0        0   600200 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/test/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      989 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2922 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_explicit_joins.py
+-rw-r--r--   0        0        0     1210 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_methods.py
+-rw-r--r--   0        0        0      269 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_schema_builder.py
+-rw-r--r--   0        0        0    12288 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_sql_builder.py
+-rw-r--r--   0        0        0     7124 2024-04-22 01:39:03.644242 py_dbchat-0.0.2rc85.post1/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc85.post1/PKG-INFO
```

### Comparing `py_dbchat-0.0.2rc84.post1/.devcontainer/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc85.post1/.devcontainer/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.devcontainer/devcontainer.json` & `py_dbchat-0.0.2rc85.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.devcontainer/docker-compose.yml` & `py_dbchat-0.0.2rc85.post1/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.github/workflows/schedule-update-actions.yml` & `py_dbchat-0.0.2rc85.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.gitignore` & `py_dbchat-0.0.2rc85.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.pre-commit-config.yaml` & `py_dbchat-0.0.2rc85.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.vscode/launch.json` & `py_dbchat-0.0.2rc85.post1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/.vscode/settings.json` & `py_dbchat-0.0.2rc85.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/LICENSE` & `py_dbchat-0.0.2rc85.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/SECURITY.md` & `py_dbchat-0.0.2rc85.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/SUPPORT.md` & `py_dbchat-0.0.2rc85.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/Test.session.sql` & `py_dbchat-0.0.2rc85.post1/Test.session.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/docs/Makefile` & `py_dbchat-0.0.2rc85.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/docs/conf.py` & `py_dbchat-0.0.2rc85.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/docs/make.bat` & `py_dbchat-0.0.2rc85.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/docs/pylint.md` & `py_dbchat-0.0.2rc85.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/pyproject.toml` & `py_dbchat-0.0.2rc85.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/api/database/repository.py` & `py_dbchat-0.0.2rc85.post1/src/api/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/api/dependencies.py` & `py_dbchat-0.0.2rc85.post1/src/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/api/main.py` & `py_dbchat-0.0.2rc85.post1/src/api/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from fastapi import Depends, FastAPI
 
 from api.dependencies import get_query_token, get_token_header
 from api.internal import admin
 from api.routers import items, users,settings
+from fastapi.middleware.cors import CORSMiddleware
 
 app = FastAPI() # dependencies=[Depends(get_query_token)])
 
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=["*"],
+    allow_credentials=True,
+    allow_methods=["*"],
+    allow_headers=["*"],
+)
+
+
 
 app.include_router(users.router)
 app.include_router(items.router)
 app.include_router(settings.router)
 app.include_router(
     admin.router,
     prefix="/admin",
```

### Comparing `py_dbchat-0.0.2rc84.post1/src/api/routers/items.py` & `py_dbchat-0.0.2rc85.post1/src/api/routers/items.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/api/routers/settings.py` & `py_dbchat-0.0.2rc85.post1/src/api/routers/settings.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/.DS_Store` & `py_dbchat-0.0.2rc85.post1/src/db_chat/.DS_Store`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/ask.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/ask.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/hello_world.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/hello_world.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/llm/classic_prompt.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/classic_prompt.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/llm/function_calling.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/llm/llm.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/llm/llm_langchain_sample.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/llm/llm_langchain_sample.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/Query.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/Query.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/schema.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/schema.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/sql_builder.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py` & `py_dbchat-0.0.2rc85.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/README.md` & `py_dbchat-0.0.2rc85.post1/src/ui/README.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/package-lock.json` & `py_dbchat-0.0.2rc85.post1/src/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/package.json` & `py_dbchat-0.0.2rc85.post1/src/ui/package.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/public/vite.svg` & `py_dbchat-0.0.2rc85.post1/src/ui/public/vite.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/src/App.css` & `py_dbchat-0.0.2rc85.post1/src/ui/src/App.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/src/api/baseApi.ts` & `py_dbchat-0.0.2rc85.post1/src/ui/src/api/baseApi.ts`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,26 @@
         });
         if (!response.ok) {
             throw new Error('Failed to fetch');
         }
         const data = await response.json();
         return data;
     }
+    public async GetOne<T>(url: string, params: URLSearchParams = new URLSearchParams({})): Promise<T> {
+        const response = await fetch(`${this.base_url}${url}?` + params, {
+            headers: {
+                'Authorization': get_bearer_token()
+            }
+        });
+        if (!response.ok) {
+            throw new Error('Failed to fetch');
+        }
+        const data = await response.json();
+        return data;
+    }
     public async GetById<T>(url: string, id: string): Promise<T> {
         const response = await fetch(`${this.base_url}${url}/${id}`, {
             headers: {
                 'Authorization': get_bearer_token()
             }
         });
         if (!response.ok) {
```

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/src/assets/react.svg` & `py_dbchat-0.0.2rc85.post1/src/ui/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/src/index.css` & `py_dbchat-0.0.2rc85.post1/src/ui/src/index.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/src/ui/tsconfig.json` & `py_dbchat-0.0.2rc85.post1/src/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/test/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc85.post1/test/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/tests/conftest.py` & `py_dbchat-0.0.2rc85.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/tests/test_explicit_joins.py` & `py_dbchat-0.0.2rc85.post1/tests/test_explicit_joins.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/tests/test_methods.py` & `py_dbchat-0.0.2rc85.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/tests/test_sql_builder.py` & `py_dbchat-0.0.2rc85.post1/tests/test_sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/tests/test_sqlalchemy.py` & `py_dbchat-0.0.2rc85.post1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc84.post1/PKG-INFO` & `py_dbchat-0.0.2rc85.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbchat
-Version: 0.0.2rc84.post1
+Version: 0.0.2rc85.post1
 Summary: Chat with your existing database without using vector DB.
 Author-email: Dhanilan <mail2dhanilan@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

