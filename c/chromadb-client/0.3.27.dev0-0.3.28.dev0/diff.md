# Comparing `tmp/chromadb-client-0.3.27.dev0.tar.gz` & `tmp/chromadb-client-0.3.28.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-client-0.3.27.dev0.tar", last modified: Mon Jun  5 18:02:18 2023, max compression
+gzip compressed data, was "chromadb-client-0.3.28.dev0.tar", last modified: Mon Jul 10 19:51:07 2023, max compression
```

## Comparing `chromadb-client-0.3.27.dev0.tar` & `chromadb-client-0.3.28.dev0.tar`

### file list

```diff
@@ -1,231 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.518897 chromadb-client-0.3.27.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-05 18:02:13.000000 chromadb-client-0.3.27.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/RELEASE_PROCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/backup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/integration-test
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/restore.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/setup_linux.sh
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/setup_mac.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12480 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22262 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 18:02:13.000000 chromadb-client-0.3.27.dev0/chromadb/is_thin_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.518897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/vector/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/test/db/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/hnswlib/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/property/
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15026 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/segment/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    40112 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/utils/messageid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.542897 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/clients/js/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/examples/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/app.ts
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    71072 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/examples/node/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     1075 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/genapi.sh
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/openapitools.json
--rw-r--r--   0 runner    (1001) docker     (123)   450648 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/ChromaClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)    19403 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/Collection.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/js/src/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    56700 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/api.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/configuration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/models.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/runtime.ts
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/types.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/add.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/collection.client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/get.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/initClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/query.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/update.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/tsconfig.module.json
--rw-r--r--   0 runner    (1001) docker     (123)   157735 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/integration-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/is_thin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/config/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/config/backup_disk.xml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/config/chroma_users.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/docker-compose.server.example.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/examples/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/where_filtering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/log_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/migrations/embeddings_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/migrations/metadb/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/migrations/sysdb/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 18:02:13.000000 chromadb-client-0.3.27.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.386009 chromadb-client-0.3.28.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.394009 chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.398009 chromadb-client-0.3.28.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.398009 chromadb-client-0.3.28.dev0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-10 19:51:01.000000 chromadb-client-0.3.28.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.398009 chromadb-client-0.3.28.dev0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/backup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/integration-test
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/restore.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/setup_linux.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/setup_mac.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.398009 chromadb-client-0.3.28.dev0/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/bin/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.398009 chromadb-client-0.3.28.dev0/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19109 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/api/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/api/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/experimental/density_relevance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 19:51:01.000000 chromadb-client-0.3.28.dev0/chromadb/is_thin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.390009 chromadb-client-0.3.28.dev0/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/segment/impl/vector/local_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.402009 chromadb-client-0.3.28.dev0/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/test/hnswlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.406010 chromadb-client-0.3.28.dev0/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19043 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.410010 chromadb-client-0.3.28.dev0/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15132 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40736 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.410010 chromadb-client-0.3.28.dev0/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.410010 chromadb-client-0.3.28.dev0/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/chromadb/utils/messageid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.410010 chromadb-client-0.3.28.dev0/chromadb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-10 19:51:07.000000 chromadb-client-0.3.28.dev0/chromadb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-10 19:51:07.000000 chromadb-client-0.3.28.dev0/chromadb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:51:07.000000 chromadb-client-0.3.28.dev0/chromadb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 19:51:07.000000 chromadb-client-0.3.28.dev0/chromadb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 19:51:07.000000 chromadb-client-0.3.28.dev0/chromadb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.390009 chromadb-client-0.3.28.dev0/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.414010 chromadb-client-0.3.28.dev0/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.390009 chromadb-client-0.3.28.dev0/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.414010 chromadb-client-0.3.28.dev0/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.414010 chromadb-client-0.3.28.dev0/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1075 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   450648 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.414010 chromadb-client-0.3.28.dev0/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.414010 chromadb-client-0.3.28.dev0/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.418010 chromadb-client-0.3.28.dev0/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    56700 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.418010 chromadb-client-0.3.28.dev0/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   157735 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.418010 chromadb-client-0.3.28.dev0/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/clients/python/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.418010 chromadb-client-0.3.28.dev0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/config/backup_disk.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/config/chroma_users.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.418010 chromadb-client-0.3.28.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.418010 chromadb-client-0.3.28.dev0/examples/basic_functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/basic_functionality/alternative_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/basic_functionality/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/basic_functionality/where_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.394009 chromadb-client-0.3.28.dev0/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.394009 chromadb-client-0.3.28.dev0/examples/use_with/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/examples/use_with/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/use_with/cohere/cohere_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/use_with/cohere/cohere_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/examples/use_with/cohere/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/log_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.394009 chromadb-client-0.3.28.dev0/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/migrations/sysdb/00003-collection-dimension.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 19:51:01.000000 chromadb-client-0.3.28.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 19:50:49.000000 chromadb-client-0.3.28.dev0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:51:07.422010 chromadb-client-0.3.28.dev0/setup.cfg
```

### Comparing `chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-client-0.3.28.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/.github/workflows/chroma-client-integration-test.yml` & `chromadb-client-0.3.28.dev0/.github/workflows/chroma-client-integration-test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 on:
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
+      - '*'
 
 jobs:
   test:
     timeout-minutes: 90
     strategy:
       matrix:
         python: ['3.7', '3.8', '3.9', '3.10']
```

### Comparing `chromadb-client-0.3.27.dev0/.github/workflows/chroma-integration-test.yml` & `chromadb-client-0.3.28.dev0/.github/workflows/chroma-integration-test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
     branches:
       - main
       - team/hypothesis-tests
   pull_request:
     branches:
       - main
-      - team/hypothesis-tests
+      - '*'
 
 jobs:
   test:
     strategy:
       matrix:
         python: ['3.7']
         platform: [ubuntu-latest]
```

### Comparing `chromadb-client-0.3.27.dev0/.github/workflows/chroma-release-python-client.yml` & `chromadb-client-0.3.28.dev0/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/.github/workflows/chroma-release.yml` & `chromadb-client-0.3.28.dev0/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/.github/workflows/chroma-test.yml` & `chromadb-client-0.3.28.dev0/.github/workflows/chroma-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
     branches:
       - main
       - team/hypothesis-tests
   pull_request:
     branches:
       - main
-      - team/hypothesis-tests
+      - '*'
 
 jobs:
   test:
     timeout-minutes: 90
     strategy:
       matrix:
         python: ['3.7', '3.8', '3.9', '3.10']
```

### Comparing `chromadb-client-0.3.27.dev0/.github/workflows/pr-review-checklist.yml` & `chromadb-client-0.3.28.dev0/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/.pre-commit-config.yaml` & `chromadb-client-0.3.28.dev0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,8 @@
           - "--max-line-length=88"
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.2.0"
     hooks:
       - id: mypy
         args: [--strict, --ignore-missing-imports, --follow-imports=silent, --disable-error-code=type-abstract]
-        additional_dependencies:
-          [
-            "types-requests",
-            "pydantic",
-            "overrides",
-            "hypothesis",
-            "pytest",
-            "numpy",
-          ]
+        additional_dependencies: ["types-requests", "pydantic", "overrides", "hypothesis", "pytest", "pypika", "numpy"]
```

### Comparing `chromadb-client-0.3.27.dev0/.vscode/settings.json` & `chromadb-client-0.3.28.dev0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/DEVELOP.md` & `chromadb-client-0.3.28.dev0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/Dockerfile` & `chromadb-client-0.3.28.dev0/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 FROM python:3.10-slim-bullseye as builder
 
 #RUN apt-get update -qq
 #RUN apt-get install python3.10 python3-pip -y --no-install-recommends && rm -rf /var/lib/apt/lists_/*
-RUN apt-get update && apt-get install build-essential -y
+RUN apt-get update --fix-missing && apt-get install -y --fix-missing build-essential
 
 RUN mkdir /install
 WORKDIR /install
 
 COPY ./requirements.txt requirements.txt
 
 RUN pip install --no-cache-dir --upgrade --prefix="/install" -r requirements.txt
```

### Comparing `chromadb-client-0.3.27.dev0/LICENSE` & `chromadb-client-0.3.28.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/PKG-INFO` & `chromadb-client-0.3.28.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.27.dev0
+Version: 0.3.28.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
 client = chromadb.Client(Settings(chroma_api_impl="rest",
                                   chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+                                  chroma_server_http_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.27.dev0 Summary:
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.28.dev0 Summary:
 Chroma Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
 you can do the following: ```python import chromadb from chromadb.config import
 Settings # Example setup of the client to connect to your chroma server client
 = chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_port=8000)) collection =
+chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
 client.create_collection("all-my-documents") collection.add( documents=["This
 is document1", "This is document2"], metadatas=[{"source": "notion"},
 {"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
 for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
 collection.query( query_texts=["This is a query document"], n_results=2, #
 where={"metadata_field": "is_equal_to_this"}, # optional filter #
 where_document={"$contains":"search_string"} # optional filter ) ``` ## License
```

### Comparing `chromadb-client-0.3.27.dev0/README.md` & `chromadb-client-0.3.28.dev0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
 client = chromadb.Client(Settings(chroma_api_impl="rest",
                                   chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+                                  chroma_server_http_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
 you can do the following: ```python import chromadb from chromadb.config import
 Settings # Example setup of the client to connect to your chroma server client
 = chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_port=8000)) collection =
+chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
 client.create_collection("all-my-documents") collection.add( documents=["This
 is document1", "This is document2"], metadatas=[{"source": "notion"},
 {"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
 for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
 collection.query( query_texts=["This is a query document"], n_results=2, #
 where={"metadata_field": "is_equal_to_this"}, # optional filter #
 where_document={"$contains":"search_string"} # optional filter ) ``` ## License
```

### Comparing `chromadb-client-0.3.27.dev0/RELEASE_PROCESS.md` & `chromadb-client-0.3.28.dev0/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/bin/backup.sh` & `chromadb-client-0.3.28.dev0/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/bin/generate_cloudformation.py` & `chromadb-client-0.3.28.dev0/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/bin/restore.sh` & `chromadb-client-0.3.28.dev0/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/bin/setup_linux.sh` & `chromadb-client-0.3.28.dev0/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/bin/templates/docker-compose.yml` & `chromadb-client-0.3.28.dev0/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from chromadb.config import Settings, System
 from chromadb.api import API
 
 logger = logging.getLogger(__name__)
 
 __settings = Settings()
 
-__version__ = "0.3.26"
+__version__ = "0.3.27"
 
 
 def configure(**kwargs) -> None:  # type: ignore
     """Override Chroma's default settings, environment variables or .env files"""
     global __settings
     __settings = chromadb.config.Settings(**kwargs)
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/api/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     Where,
     QueryResult,
     GetResult,
     WhereDocument,
 )
 from chromadb.config import Component
 import chromadb.utils.embedding_functions as ef
-from overrides import override
 
 
 class API(Component, ABC):
     @abstractmethod
     def heartbeat(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive
 
@@ -282,22 +281,20 @@
         Args:
             embedding: The embedding to find the nearest neighbors of
             n_results: The number of nearest neighbors to return. Defaults to 10.
             where: A dictionary of key-value pairs to filter the embeddings by. Defaults to {}.
         """
         pass
 
-    @override
     @abstractmethod
-    def reset(self) -> None:
+    def reset(self) -> bool:
         """Resets the database
         ⚠️ This is destructive and will delete all data in the database.
         Args:
             None
-
         Returns:
             None
         """
         pass
 
     @abstractmethod
     def raw_sql(self, sql: str) -> pd.DataFrame:
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/api/fastapi.py` & `chromadb-client-0.3.28.dev0/chromadb/api/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,18 +335,19 @@
             distances=body.get("distances", None),
             embeddings=body.get("embeddings", None),
             metadatas=body.get("metadatas", None),
             documents=body.get("documents", None),
         )
 
     @override
-    def reset(self) -> None:
+    def reset(self) -> bool:
         """Resets the database"""
         resp = requests.post(self._api_url + "/reset")
         raise_chroma_error(resp)
+        return cast(bool, resp.json())
 
     @override
     def persist(self) -> bool:
         """Persists the database"""
         resp = requests.post(self._api_url + "/persist")
         raise_chroma_error(resp)
         return cast(bool, resp.json())
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/api/local.py` & `chromadb-client-0.3.28.dev0/chromadb/api/local.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import time
 from uuid import UUID
 from typing import List, Optional, Sequence, cast
 from chromadb import __version__
-import chromadb.errors as errors
 from chromadb.api import API
 from chromadb.db import DB
 from chromadb.api.types import (
     Documents,
     EmbeddingFunction,
     Embeddings,
     GetResult,
@@ -15,24 +14,28 @@
     Include,
     Metadata,
     Metadatas,
     QueryResult,
     Where,
     WhereDocument,
     CollectionMetadata,
+    validate_metadata,
 )
 from chromadb.api.models.Collection import Collection
 from chromadb.config import System
 import chromadb.utils.embedding_functions as ef
 import re
 
 from chromadb.telemetry import Telemetry
 from chromadb.telemetry.events import CollectionAddEvent, CollectionDeleteEvent
 from overrides import override
 import pandas as pd
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 # mimics s3 bucket requirements for naming
 def check_index_name(index_name: str) -> None:
     msg = (
         "Expected collection name that "
         "(1) contains 3-63 characters, "
@@ -62,18 +65,18 @@
         self._telemetry_client = self.require(Telemetry)
 
     @override
     def heartbeat(self) -> int:
         """Ping the database to ensure it is alive
 
         Returns:
-            The current time in milliseconds
+            The current time in nanoseconds since epoch
 
         """
-        return int(1000 * time.time_ns())
+        return int(time.time_ns())
 
     #
     # COLLECTION METHODS
     #
     @override
     def create_collection(
         self,
@@ -103,14 +106,17 @@
 
             client.create_collection("my_collection", metadata={"foo": "bar"})
             # collection(name="my_collection", metadata={"foo": "bar"})
             ```
         """
         check_index_name(name)
 
+        if metadata is not None:
+            validate_metadata(metadata)
+
         res = self._db.create_collection(name, metadata, get_or_create)
         return Collection(
             client=self,
             name=name,
             embedding_function=embedding_function,
             id=res[0][0],
             metadata=res[0][2],
@@ -134,14 +140,18 @@
 
         Examples:
             ```python
             client.get_or_create_collection("my_collection")
             # collection(name="my_collection", metadata={})
             ```
         """
+
+        if metadata is not None:
+            validate_metadata(metadata)
+
         return self.create_collection(
             name, metadata, embedding_function, get_or_create=True
         )
 
     @override
     def get_collection(
         self,
@@ -238,19 +248,40 @@
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
-        existing_ids = self._get(collection_id, ids=ids, include=[])["ids"]
+        existing_ids = set(self._get(collection_id, ids=ids, include=[])["ids"])
         if len(existing_ids) > 0:
-            raise errors.IDAlreadyExistsError(
-                f"IDs {existing_ids} already exist in collection {collection_id}"
-            )
+            logger.info(f"Adding {len(existing_ids)} items with ids that already exist")
+            # Partially add the items that don't already exist
+            valid_indices = [i for i, id in enumerate(ids) if id not in existing_ids]
+            if len(valid_indices) == 0:
+                return False
+            filtered_ids: IDs = []
+            filtered_embeddings: Embeddings = []
+            if metadatas is not None:
+                filtered_metadatas: Metadatas = []
+            if documents is not None:
+                filtered_documents: Documents = []
+            for index in valid_indices:
+                filtered_ids.append(ids[index])
+                filtered_embeddings.append(embeddings[index])
+                if metadatas is not None:
+                    filtered_metadatas.append(metadatas[index])
+                if documents is not None:
+                    filtered_documents.append(documents[index])
+            ids = filtered_ids
+            embeddings = filtered_embeddings
+            if metadatas is not None:
+                metadatas = filtered_metadatas
+            if documents is not None:
+                documents = filtered_documents
 
         added_uuids = self._db.add(
             collection_id,
             embeddings=embeddings,
             metadatas=metadatas,
             documents=documents,
             ids=ids,
@@ -431,22 +462,23 @@
         return deleted_uuids
 
     @override
     def _count(self, collection_id: UUID) -> int:
         return self._db.count(collection_id)
 
     @override
-    def reset(self) -> None:
+    def reset(self) -> bool:
         """Reset the database. This will delete all collections and items.
 
         Returns:
             True if the database was reset successfully
 
         """
-        self._db.reset()
+        self._db.reset_state()
+        return True
 
     @override
     def _query(
         self,
         collection_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/api/models/Collection.py` & `chromadb-client-0.3.28.dev0/chromadb/api/models/Collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     QueryResult,
     ID,
     OneOrMany,
     WhereDocument,
     maybe_cast_one_to_many,
     validate_ids,
     validate_include,
+    validate_metadata,
     validate_metadatas,
     validate_where,
     validate_where_document,
     validate_n_results,
     validate_embeddings,
 )
 import logging
@@ -72,18 +73,17 @@
         metadatas: Optional[OneOrMany[Metadata]] = None,
         documents: Optional[OneOrMany[Document]] = None,
         increment_index: bool = True,
     ) -> None:
         """Add embeddings to the data store.
         Args:
             ids: The ids of the embeddings you wish to add
-            embedding: The embeddings to add. If None, embeddings will be computed based on the documents using the embedding_function set for the Collection. Optional.
-            metadata: The metadata to associate with the embeddings. When querying, you can filter on this metadata. Optional.
+            embeddings: The embeddings to add. If None, embeddings will be computed based on the documents using the embedding_function set for the Collection. Optional.
+            metadatas: The metadata to associate with the embeddings. When querying, you can filter on this metadata. Optional.
             documents: The documents to associate with the embeddings. Optional.
-            ids: The ids to associate with the embeddings. Optional.
 
         Returns:
             None
 
         Raises:
             ValueError: If you don't provide either embeddings or documents
             ValueError: If the length of ids, embeddings, metadatas, or documents don't match
@@ -237,14 +237,17 @@
         Args:
             name: The updated name for the collection. Optional.
             metadata: The updated metadata for the collection. Optional.
 
         Returns:
             None
         """
+        if metadata is not None:
+            validate_metadata(metadata)
+
         self._client._modify(id=self.id, new_name=name, new_metadata=metadata)
         if name:
             self.name = name
         if metadata:
             self.metadata = metadata
 
     def update(
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/api/types.py` & `chromadb-client-0.3.28.dev0/chromadb/api/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from typing import Any, Optional, Union, Dict, Sequence, TypeVar, List
+from typing import Optional, Union, Sequence, TypeVar, List, Dict, Any
 from typing_extensions import Literal, TypedDict, Protocol
 import chromadb.errors as errors
 from chromadb.types import (
     Metadata,
+    UpdateMetadata,
     Vector,
     LiteralValue,
     LogicalOperator,
     WhereOperator,
     OperatorExpression,
     Where,
     WhereDocumentOperator,
     WhereDocument,
 )
 
 # Re-export types from chromadb.types
-__all__ = ["Metadata", "Where", "WhereDocument"]
+__all__ = ["Metadata", "Where", "WhereDocument", "UpdateCollectionMetadata"]
 
 ID = str
 IDs = List[ID]
 
 Embedding = Vector
 Embeddings = List[Embedding]
 
 Metadatas = List[Metadata]
 
-CollectionMetadata = Dict[Any, Any]
+CollectionMetadata = Dict[str, Any]
+UpdateCollectionMetadata = UpdateMetadata
 
 Document = str
 Documents = List[Document]
 
 Parameter = TypeVar("Parameter", Embedding, Document, Metadata, ID)
 T = TypeVar("T")
 OneOrMany = Union[T, List[T]]
@@ -120,18 +122,39 @@
     return ids
 
 
 def validate_metadata(metadata: Metadata) -> Metadata:
     """Validates metadata to ensure it is a dictionary of strings to strings, ints, or floats"""
     if not isinstance(metadata, dict):
         raise ValueError(f"Expected metadata to be a dict, got {metadata}")
+    if len(metadata) == 0:
+        raise ValueError(f"Expected metadata to be a non-empty dict, got {metadata}")
+    for key, value in metadata.items():
+        if not isinstance(key, str):
+            raise ValueError(
+                f"Expected metadata key to be a str, got {key} which is a {type(key)}"
+            )
+        # isinstance(True, int) evaluates to True, so we need to check for bools separately
+        if not isinstance(value, (str, int, float)) or isinstance(value, bool):
+            raise ValueError(
+                f"Expected metadata value to be a str, int, or float, got {value} which is a {type(value)}"
+            )
+    return metadata
+
+
+def validate_update_metadata(metadata: UpdateMetadata) -> UpdateMetadata:
+    """Validates metadata to ensure it is a dictionary of strings to strings, ints, or floats"""
+    if not isinstance(metadata, dict):
+        raise ValueError(f"Expected metadata to be a dict, got {metadata}")
+    if len(metadata) == 0:
+        raise ValueError(f"Expected metadata to be a non-empty dict, got {metadata}")
     for key, value in metadata.items():
         if not isinstance(key, str):
             raise ValueError(f"Expected metadata key to be a str, got {key}")
-        if not isinstance(value, (str, int, float)):
+        if not isinstance(value, (str, int, float, type(None))):
             raise ValueError(
                 f"Expected metadata value to be a str, int, or float, got {value}"
             )
     return metadata
 
 
 def validate_metadatas(metadatas: Metadatas) -> Metadatas:
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/config.py` & `chromadb-client-0.3.28.dev0/chromadb/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,32 +29,40 @@
 # TODO: Don't use concrete types here to avoid circular deps. Strings are fine for right here!
 _abstract_type_keys: Dict[str, str] = {
     "chromadb.db.DB": "chroma_db_impl",
     "chromadb.api.API": "chroma_api_impl",
     "chromadb.telemetry.Telemetry": "chroma_telemetry_impl",
     "chromadb.ingest.Producer": "chroma_producer_impl",
     "chromadb.ingest.Consumer": "chroma_consumer_impl",
+    "chromadb.db.system.SysDB": "chroma_sysdb_impl",
+    "chromadb.segment.SegmentManager": "chroma_segment_manager_impl",
 }
 
 
 class Settings(BaseSettings):
     environment: str = ""
 
     chroma_db_impl: str = "chromadb.db.duckdb.DuckDB"
     chroma_api_impl: str = "chromadb.api.local.LocalAPI"
     chroma_telemetry_impl: str = "chromadb.telemetry.posthog.Posthog"
 
     # New architecture components
     chroma_sysdb_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
     chroma_producer_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
     chroma_consumer_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
+    chroma_segment_manager_impl: str = (
+        "chromadb.segment.impl.manager.local.LocalSegmentManager"
+    )
 
     clickhouse_host: Optional[str] = None
     clickhouse_port: Optional[str] = None
 
+    tenant_id: str = "default"
+    topic_namespace: str = "default"
+
     persist_directory: str = ".chroma"
 
     chroma_server_host: Optional[str] = None
     chroma_server_http_port: Optional[str] = None
     chroma_server_ssl_enabled: Optional[bool] = False
     chroma_server_grpc_port: Optional[str] = None
     chroma_server_cors_allow_origins: List[str] = []  # eg ["http://localhost:3000"]
@@ -110,44 +118,38 @@
     def dependencies(self) -> Set["Component"]:
         """Return the full set of components this component depends on."""
         return self._dependencies
 
     def stop(self) -> None:
         """Idempotently stop this component's execution and free all associated
         resources."""
+        logger.debug(f"Stopping component {self.__class__.__name__}")
         self._running = False
 
     def start(self) -> None:
         """Idempotently start this component's execution"""
+        logger.debug(f"Starting component {self.__class__.__name__}")
         self._running = True
 
-    def reset(self) -> None:
+    def reset_state(self) -> None:
         """Reset this component's state to its initial blank state. Only intended to be
         called from tests."""
-        pass
+        logger.debug(f"Resetting component {self.__class__.__name__}")
 
 
 class System(Component):
     settings: Settings
 
     _instances: Dict[Type[Component], Component]
 
     def __init__(self, settings: Settings):
         self.settings = settings
         self._instances = {}
         super().__init__(self)
 
-        if is_thin_client:
-            # The thin client is a system with only the API component
-            if self.settings["chroma_api_impl"] != "chromadb.api.fastapi.FastAPI":
-                raise RuntimeError(
-                    "Chroma is running in http-only client mode, and can only be run with 'chromadb.api.fastapi.FastAPI' or 'rest' as the chroma_api_impl. \
-            see https://docs.trychroma.com/usage-guide?lang=py#using-the-python-http-only-client for more information."
-                )
-
     def instance(self, type: Type[T]) -> T:
         """Return an instance of the component type specified. If the system is running,
         the component will be started as well."""
 
         if inspect.isabstract(type):
             type_fqn = get_fqn(type)
             if type_fqn not in _abstract_type_keys:
@@ -183,19 +185,20 @@
     @override
     def stop(self) -> None:
         super().stop()
         for component in reversed(list(self.components())):
             component.stop()
 
     @override
-    def reset(self) -> None:
+    def reset_state(self) -> None:
+        """Reset the state of this system and all constituents in reverse dependency order"""
         if not self.settings.allow_reset:
             raise ValueError("Resetting is not allowed by this configuration")
-        for component in self.components():
-            component.reset()
+        for component in reversed(list(self.components())):
+            component.reset_state()
 
 
 C = TypeVar("C")
 
 
 def get_class(fqn: str, type: Type[C]) -> Type[C]:
     """Given a fully qualifed class name, import the module and return the class"""
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/db/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from abc import abstractmethod
 from typing import List, Sequence, Optional, Tuple
 from uuid import UUID
-import numpy.typing as npt
 from chromadb.api.types import (
     Embeddings,
     Documents,
     IDs,
     Metadatas,
     Metadata,
     Where,
     WhereDocument,
 )
 from chromadb.config import Component
-from overrides import override
 
 
 class DB(Component):
     @abstractmethod
     def create_collection(
         self,
         name: str,
@@ -104,27 +102,22 @@
         collection_uuid: Optional[UUID] = None,
         ids: Optional[IDs] = None,
         where_document: WhereDocument = {},
     ) -> List[str]:
         pass
 
     @abstractmethod
-    @override
-    def reset(self) -> None:
-        pass
-
-    @abstractmethod
     def get_nearest_neighbors(
         self,
         collection_uuid: UUID,
         where: Where = {},
         embeddings: Optional[Embeddings] = None,
         n_results: int = 10,
         where_document: WhereDocument = {},
-    ) -> Tuple[List[List[UUID]], npt.NDArray]:
+    ) -> Tuple[List[List[UUID]], List[List[float]]]:
         pass
 
     @abstractmethod
     def get_by_ids(
         self, uuids: List[UUID], columns: Optional[List[str]] = None
     ) -> Sequence:  # type: ignore
         pass
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/base.py` & `chromadb-client-0.3.28.dev0/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/clickhouse.py` & `chromadb-client-0.3.28.dev0/chromadb/db/clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import clickhouse_connect
 from clickhouse_connect.driver.client import Client
 from clickhouse_connect import common
 import logging
 from uuid import UUID
 from chromadb.config import System
 from overrides import override
-import numpy.typing as npt
 from chromadb.api.types import Metadata
 
 logger = logging.getLogger(__name__)
 
 COLLECTION_TABLE_SCHEMA = [{"uuid": "UUID"}, {"name": "String"}, {"metadata": "String"}]
 
 EMBEDDING_TABLE_SCHEMA = [
@@ -583,15 +582,15 @@
     def get_nearest_neighbors(
         self,
         collection_uuid: UUID,
         where: Where = {},
         embeddings: Optional[Embeddings] = None,
         n_results: int = 10,
         where_document: WhereDocument = {},
-    ) -> Tuple[List[List[UUID]], npt.NDArray]:
+    ) -> Tuple[List[List[UUID]], List[List[float]]]:
         # Either the collection name or the collection uuid must be provided
         if collection_uuid is None:
             raise TypeError("Argument collection_uuid cannot be None")
 
         if len(where) != 0 or len(where_document) != 0:
             results = self.get(
                 collection_uuid=collection_uuid,
@@ -639,15 +638,15 @@
         index.add(ids, embeddings)
 
     def reset_indexes(self):
         delete_all_indexes(self._settings)
         self.index_cache = {}
 
     @override
-    def reset(self):
+    def reset_state(self):
         conn = self._get_conn()
         conn.command("DROP TABLE collections")
         conn.command("DROP TABLE embeddings")
         self._create_table_collections(conn)
         self._create_table_embeddings(conn)
 
         self.reset_indexes()
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/duckdb.py` & `chromadb-client-0.3.28.dev0/chromadb/db/duckdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
     @override
     def raw_sql(self, raw_sql):
         return self._conn.execute(raw_sql).df()
 
     # TODO: This method should share logic with clickhouse impl
     @override
-    def reset(self):
+    def reset_state(self):
         self._conn.execute("DROP TABLE collections")
         self._conn.execute("DROP TABLE embeddings")
         self._create_table_collections(self._conn)
         self._create_table_embeddings(self._conn)
 
         self.reset_indexes()
 
@@ -520,15 +520,15 @@
             )
 
     def __del__(self):
         # No-op for duckdb with persistence since the base class will delete the indexes
         pass
 
     @override
-    def reset(self):
-        super().reset()
+    def reset_state(self):
+        super().reset_state()
         # empty the save folder
         import shutil
         import os
 
         shutil.rmtree(self._save_folder)
         os.mkdir(self._save_folder)
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/impl/sqlite.py` & `chromadb-client-0.3.28.dev0/chromadb/db/impl/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     @override
     def start(self) -> None:
         super().start()
         self._conn = sqlite3.connect(self._db_file)
         self._conn.isolation_level = None  # Handle commits explicitly
         with self.tx() as cur:
             cur.execute("PRAGMA foreign_keys = ON")
+            cur.execute("PRAGMA case_sensitive_like = ON")
         self.initialize_migrations()
 
     @override
     def stop(self) -> None:
         super().stop()
         self._conn.close()
 
@@ -96,25 +97,25 @@
     @override
     def tx(self) -> TxWrapper:
         if not hasattr(self._tx_stack, "stack"):
             self._tx_stack.stack = []
         return TxWrapper(self._conn, stack=self._tx_stack)
 
     @override
-    def reset(self) -> None:
+    def reset_state(self) -> None:
         if not self._settings.require("allow_reset"):
             raise ValueError(
                 "Resetting the database is not allowed. Set `allow_reset` to true in the config in tests or other non-production environments where reset should be permitted."
             )
         self._conn.close()
         db_file = self._settings.require("sqlite_database")
         if db_file != ":memory:":
             os.remove(db_file)
         self.start()
-        super().reset()
+        super().reset_state()
 
     @override
     def setup_migrations(self) -> None:
         with self.tx() as cur:
             cur.execute(
                 """
                  CREATE TABLE IF NOT EXISTS migrations (
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/index/hnswlib.py` & `chromadb-client-0.3.28.dev0/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/migrations.py` & `chromadb-client-0.3.28.dev0/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/mixins/embeddings_queue.py` & `chromadb-client-0.3.28.dev0/chromadb/db/mixins/embeddings_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     _subscriptions: Dict[str, Set[Subscription]]
 
     def __init__(self, system: System):
         self._subscriptions = defaultdict(set)
         super().__init__(system)
 
     @override
-    def reset(self) -> None:
-        super().reset()
+    def reset_state(self) -> None:
+        super().reset_state()
         self._subscriptions = defaultdict(set)
 
     @override
     def create_topic(self, topic_name: str) -> None:
         # Topic creation is implicit for this impl
         pass
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/mixins/sysdb.py` & `chromadb-client-0.3.28.dev0/chromadb/db/mixins/sysdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,19 +72,25 @@
     def create_collection(self, collection: Collection) -> None:
         """Create a new collection"""
         with self.tx() as cur:
             collections = Table("collections")
             insert_collection = (
                 self.querybuilder()
                 .into(collections)
-                .columns(collections.id, collections.topic, collections.name)
+                .columns(
+                    collections.id,
+                    collections.topic,
+                    collections.name,
+                    collections.dimension,
+                )
                 .insert(
                     ParameterValue(self.uuid_to_db(collection["id"])),
                     ParameterValue(collection["topic"]),
                     ParameterValue(collection["name"]),
+                    ParameterValue(collection["dimension"]),
                 )
             )
             sql, params = get_sql(insert_collection, self.parameter_format())
             try:
                 cur.execute(sql, params)
             except self.unique_constraint_error() as e:
                 raise UniqueConstraintError(
@@ -181,14 +187,15 @@
         q = (
             self.querybuilder()
             .from_(collections_t)
             .select(
                 collections_t.id,
                 collections_t.name,
                 collections_t.topic,
+                collections_t.dimension,
                 metadata_t.key,
                 metadata_t.str_value,
                 metadata_t.int_value,
                 metadata_t.float_value,
             )
             .left_join(metadata_t)
             .on(collections_t.id == metadata_t.collection_id)
@@ -207,21 +214,23 @@
             by_collection = groupby(rows, lambda r: cast(object, r[0]))
             collections = []
             for collection_id, collection_rows in by_collection:
                 id = self.uuid_from_db(str(collection_id))
                 rows = list(collection_rows)
                 name = str(rows[0][1])
                 topic = str(rows[0][2])
+                dimension = int(rows[0][3]) if rows[0][3] else None
                 metadata = self._metadata_from_rows(rows)
                 collections.append(
                     Collection(
                         id=cast(UUID, id),
                         topic=topic,
                         name=name,
                         metadata=metadata,
+                        dimension=dimension,
                     )
                 )
 
             return collections
 
     @override
     def delete_segment(self, id: UUID) -> None:
@@ -313,14 +322,15 @@
 
     @override
     def update_collection(
         self,
         id: UUID,
         topic: OptionalArgument[Optional[str]] = Unspecified(),
         name: OptionalArgument[str] = Unspecified(),
+        dimension: OptionalArgument[Optional[int]] = Unspecified(),
         metadata: OptionalArgument[Optional[UpdateMetadata]] = Unspecified(),
     ) -> None:
         collections_t = Table("collections")
         metadata_t = Table("collection_metadata")
 
         q = (
             self.querybuilder()
@@ -330,54 +340,61 @@
 
         if not topic == Unspecified():
             q = q.set(collections_t.topic, ParameterValue(topic))
 
         if not name == Unspecified():
             q = q.set(collections_t.name, ParameterValue(name))
 
+        if not dimension == Unspecified():
+            q = q.set(collections_t.dimension, ParameterValue(dimension))
+
         with self.tx() as cur:
             sql, params = get_sql(q, self.parameter_format())
             if sql:  # pypika emits a blank string if nothing to do
                 cur.execute(sql, params)
 
-            if metadata is None:
+            # TODO: Update to use better semantics where it's possible to update
+            # individual keys without wiping all the existing metadata.
+
+            # For now, follow current legancy semantics where metadata is fully reset
+            if metadata != Unspecified():
                 q = (
                     self.querybuilder()
                     .from_(metadata_t)
                     .where(
                         metadata_t.collection_id == ParameterValue(self.uuid_to_db(id))
                     )
                     .delete()
                 )
                 sql, params = get_sql(q, self.parameter_format())
                 cur.execute(sql, params)
-            elif metadata != Unspecified():
-                metadata = cast(UpdateMetadata, metadata)
-                self._insert_metadata(
-                    cur,
-                    metadata_t,
-                    metadata_t.collection_id,
-                    id,
-                    metadata,
-                    set(metadata.keys()),
-                )
+                if metadata is not None:
+                    metadata = cast(UpdateMetadata, metadata)
+                    self._insert_metadata(
+                        cur,
+                        metadata_t,
+                        metadata_t.collection_id,
+                        id,
+                        metadata,
+                        set(metadata.keys()),
+                    )
 
     def _metadata_from_rows(
         self, rows: Sequence[Tuple[Any, ...]]
     ) -> Optional[Metadata]:
         """Given SQL rows, return a metadata map (assuming that the last four columns
         are the key, str_value, int_value & float_value)"""
         metadata: Dict[str, Union[str, int, float]] = {}
         for row in rows:
             key = str(row[-4])
-            if row[-3]:
+            if row[-3] is not None:
                 metadata[key] = str(row[-3])
-            elif row[-2]:
+            elif row[-2] is not None:
                 metadata[key] = int(row[-2])
-            elif row[-1]:
+            elif row[-1] is not None:
                 metadata[key] = float(row[-1])
         return metadata or None
 
     def _insert_metadata(
         self,
         cur: Cursor,
         table: Table,
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/db/system.py` & `chromadb-client-0.3.28.dev0/chromadb/db/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,13 +73,14 @@
 
     @abstractmethod
     def update_collection(
         self,
         id: UUID,
         topic: OptionalArgument[str] = Unspecified(),
         name: OptionalArgument[str] = Unspecified(),
+        dimension: OptionalArgument[Optional[int]] = Unspecified(),
         metadata: OptionalArgument[Optional[UpdateMetadata]] = Unspecified(),
     ) -> None:
         """Update a collection. Unspecified fields will be left unchanged. For metadata,
         keys with None values will be removed and keys not present in the UpdateMetadata
         dict will be left unchanged."""
         pass
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/errors.py` & `chromadb-client-0.3.28.dev0/chromadb/errors.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 class InvalidDimensionException(ChromaError):
     @classmethod
     @overrides
     def name(cls) -> str:
         return "InvalidDimension"
 
 
+class InvalidCollectionException(ChromaError):
+    @classmethod
+    @overrides
+    def name(cls) -> str:
+        return "InvalidCollection"
+
+
 class IDAlreadyExistsError(ChromaError):
     @overrides
     def code(self) -> int:
         return 409  # Conflict
 
     @classmethod
     @overrides
@@ -48,11 +55,12 @@
     @overrides
     def name(cls) -> str:
         return "InvalidUUID"
 
 
 error_types: Dict[str, Type[ChromaError]] = {
     "InvalidDimension": InvalidDimensionException,
+    "InvalidCollection": InvalidCollectionException,
     "IDAlreadyExists": IDAlreadyExistsError,
     "DuplicateID": DuplicateIDError,
     "InvalidUUID": InvalidUUIDError,
 }
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/ingest/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/ingest/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     SeqId,
     Vector,
     ScalarEncoding,
 )
 from chromadb.config import Component
 from uuid import UUID
 import array
-from overrides import override
 
 
 def encode_vector(vector: Vector, encoding: ScalarEncoding) -> bytes:
     """Encode a vector into a byte array."""
 
     if encoding == ScalarEncoding.FLOAT32:
         return array.array("f", vector).tobytes()
@@ -49,21 +48,14 @@
     @abstractmethod
     def submit_embedding(
         self, topic_name: str, embedding: SubmitEmbeddingRecord
     ) -> SeqId:
         """Add an embedding record to the given topic. Returns the SeqID of the record."""
         pass
 
-    @abstractmethod
-    @override
-    def reset(self) -> None:
-        """Delete all topics and data. For testing only, implementations intended for
-        production may throw an exception instead of implementing this method."""
-        pass
-
 
 ConsumerCallbackFn = Callable[[Sequence[EmbeddingRecord]], None]
 
 
 class Consumer(Component):
     """Interface for reading embeddings off an ingest stream"""
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/segment/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/segment/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-from typing import Optional, Sequence, Set, TypeVar, Type
-from abc import ABC, abstractmethod
+from typing import Optional, Sequence, TypeVar, Type
+from abc import abstractmethod
 from chromadb.types import (
     Collection,
     MetadataEmbeddingRecord,
     VectorEmbeddingRecord,
     Where,
     WhereDocument,
     VectorQuery,
     VectorQueryResult,
     Segment,
     SeqId,
+    Metadata,
 )
 from chromadb.config import Component, System
-from overrides import EnforceOverrides
 from uuid import UUID
 
 
-class SegmentImplementation(ABC, EnforceOverrides):
+class SegmentImplementation(Component):
     @abstractmethod
     def __init__(self, sytstem: System, segment: Segment):
         pass
 
     @abstractmethod
     def count(self) -> int:
         """Get the number of embeddings in this segment"""
         pass
 
     @abstractmethod
     def max_seqid(self) -> SeqId:
         """Get the maximum SeqID currently indexed by this segment"""
         pass
 
+    @staticmethod
+    def propagate_collection_metadata(metadata: Metadata) -> Optional[Metadata]:
+        """Given an arbitrary metadata map (e.g, from a collection), validate it and
+        return metadata (if any) that is applicable and should be applied to the
+        segment. Validation errors will be reported to the user."""
+        return None
+
+
+S = TypeVar("S", bound=SegmentImplementation)
+
 
 class MetadataReader(SegmentImplementation):
     """Embedding Metadata segment interface"""
 
     @abstractmethod
     def get_metadata(
         self,
@@ -69,29 +79,29 @@
 
 
 class SegmentManager(Component):
     """Interface for a pluggable strategy for creating, retrieving and instantiating
     segments as required"""
 
     @abstractmethod
-    def create_segments(self, collection: Collection) -> Set[Segment]:
-        """Create the segments required for a new collection."""
+    def create_segments(self, collection: Collection) -> Sequence[Segment]:
+        """Return the segments required for a new collection. Returns only segment data,
+        does not persist to the SysDB"""
         pass
 
     @abstractmethod
-    def delete_segments(self, collection_id: UUID) -> None:
-        """Delete all the segments associated with a collection"""
+    def delete_segments(self, collection_id: UUID) -> Sequence[UUID]:
+        """Delete any local state for all the segments associated with a collection, and
+        returns a sequence of their IDs. Does not update the SysDB."""
         pass
 
-    T = TypeVar("T", bound="SegmentImplementation")
-
     # Future Note: To support time travel, add optional parameters to this method to
     # retrieve Segment instances that are bounded to events from a specific range of
     # time
     @abstractmethod
-    def get_segment(self, collection_id: UUID, type: Type[T]) -> SegmentImplementation:
+    def get_segment(self, collection_id: UUID, type: Type[S]) -> S:
         """Return the segment that should be used for servicing queries to a collection.
         Implementations should cache appropriately; clients are intended to call this
         method repeatedly rather than storing the result (thereby giving this
         implementation full control over which segment impls are in or out of memory at
         a given time.)"""
         pass
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/segment/impl/manager/local.py` & `chromadb-client-0.3.28.dev0/chromadb/segment/impl/manager/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,130 @@
 from chromadb.segment import (
     SegmentImplementation,
     SegmentManager,
     MetadataReader,
     VectorReader,
+    S,
 )
 from chromadb.config import System, get_class
 from chromadb.db.system import SysDB
 from overrides import override
 from enum import Enum
-from chromadb.types import Collection, Segment, SegmentScope
-from typing import Dict, Set, Type, TypeVar
+from chromadb.types import Collection, Segment, SegmentScope, Metadata
+from typing import Dict, Type, Sequence, Optional, cast
 from uuid import UUID, uuid4
 from collections import defaultdict
-import re
 
 
 class SegmentType(Enum):
     SQLITE = "urn:chroma:segment/metadata/sqlite"
     HNSW_LOCAL_MEMORY = "urn:chroma:segment/vector/hnsw-local-memory"
 
 
 SEGMENT_TYPE_IMPLS = {
-    SegmentType.SQLITE: "chromadb.segment.impl.sqlite.SqliteMetadataReader",
+    SegmentType.SQLITE: "chromadb.segment.impl.metadata.sqlite.SqliteMetadataSegment",
     SegmentType.HNSW_LOCAL_MEMORY: "chromadb.segment.impl.vector.local_hnsw.LocalHnswSegment",
 }
 
-PROPAGATE_METADATA = {
-    SegmentType.HNSW_LOCAL_MEMORY: [r"^hnsw:.*"],
-}
-
 
 class LocalSegmentManager(SegmentManager):
     _sysdb: SysDB
     _system: System
     _instances: Dict[UUID, SegmentImplementation]
     _segment_cache: Dict[UUID, Dict[SegmentScope, Segment]]
 
     def __init__(self, system: System):
+        super().__init__(system)
         self._sysdb = self.require(SysDB)
         self._system = system
         self._instances = {}
         self._segment_cache = defaultdict(dict)
-        super().__init__(system)
 
     @override
     def start(self) -> None:
+        for instance in self._instances.values():
+            instance.start()
         super().start()
 
     @override
     def stop(self) -> None:
+        for instance in self._instances.values():
+            instance.stop()
         super().stop()
 
     @override
-    def reset(self) -> None:
+    def reset_state(self) -> None:
+        for instance in self._instances.values():
+            instance.stop()
         self._instances = {}
         self._segment_cache = defaultdict(dict)
-        super().reset()
+        super().reset_state()
 
     @override
-    def create_segments(self, collection: Collection) -> Set[Segment]:
+    def create_segments(self, collection: Collection) -> Sequence[Segment]:
         vector_segment = _segment(
             SegmentType.HNSW_LOCAL_MEMORY, SegmentScope.VECTOR, collection
         )
         metadata_segment = _segment(
             SegmentType.SQLITE, SegmentScope.METADATA, collection
         )
-        self._sysdb.create_segment(vector_segment)
-        self._sysdb.create_segment(metadata_segment)
-        return {vector_segment, metadata_segment}
+        return [vector_segment, metadata_segment]
 
     @override
-    def delete_segments(self, collection_id: UUID) -> None:
+    def delete_segments(self, collection_id: UUID) -> Sequence[UUID]:
         segments = self._sysdb.get_segments(collection=collection_id)
         for segment in segments:
-            self._sysdb.delete_segment(segment["id"])
-            del self._instances[segment["id"]]
-            del self._segment_cache[collection_id][segment["scope"]]
-            del self._segment_cache[collection_id]
-
-    T = TypeVar("T", bound="SegmentImplementation")
+            if segment["id"] in self._instances:
+                del self._instances[segment["id"]]
+            if collection_id in self._segment_cache:
+                if segment["scope"] in self._segment_cache[collection_id]:
+                    del self._segment_cache[collection_id][segment["scope"]]
+                del self._segment_cache[collection_id]
+        return [s["id"] for s in segments]
 
     @override
-    def get_segment(self, collection_id: UUID, type: Type[T]) -> SegmentImplementation:
-        if type == Type[MetadataReader]:
+    def get_segment(self, collection_id: UUID, type: Type[S]) -> S:
+        if type == MetadataReader:
             scope = SegmentScope.METADATA
-        elif type == Type[VectorReader]:
+        elif type == VectorReader:
             scope = SegmentScope.VECTOR
         else:
             raise ValueError(f"Invalid segment type: {type}")
 
         if scope not in self._segment_cache[collection_id]:
             segments = self._sysdb.get_segments(collection=collection_id, scope=scope)
             known_types = set([k.value for k in SEGMENT_TYPE_IMPLS.keys()])
             # Get the first segment of a known type
             segment = next(filter(lambda s: s["type"] in known_types, segments))
             self._segment_cache[collection_id][scope] = segment
 
-        return self._instance(self._segment_cache[collection_id][scope])
+        instance = self._instance(self._segment_cache[collection_id][scope])
+        return cast(S, instance)
+
+    def _cls(self, segment: Segment) -> Type[SegmentImplementation]:
+        classname = SEGMENT_TYPE_IMPLS[SegmentType(segment["type"])]
+        cls = get_class(classname, SegmentImplementation)
+        return cls
 
     def _instance(self, segment: Segment) -> SegmentImplementation:
         if segment["id"] not in self._instances:
-            classname = SEGMENT_TYPE_IMPLS[SegmentType(segment["type"])]
-            cls = get_class(classname, SegmentImplementation)
-            self._instances[segment["id"]] = cls(self._system, segment)
+            cls = self._cls(segment)
+            instance = cls(self._system, segment)
+            instance.start()
+            self._instances[segment["id"]] = instance
         return self._instances[segment["id"]]
 
 
 def _segment(type: SegmentType, scope: SegmentScope, collection: Collection) -> Segment:
     """Create a metadata dict, propagating metadata correctly for the given segment type."""
-    metadata = {}
-    regexes = PROPAGATE_METADATA.get(type, [])
-    if collection["metadata"]:
-        for key, value in collection["metadata"].items():
-            for regex in regexes:
-                if re.match(regex, key):
-                    metadata[key] = value
-                    break
+    cls = get_class(SEGMENT_TYPE_IMPLS[type], SegmentImplementation)
+    collection_metadata = collection.get("metadata", None)
+    metadata: Optional[Metadata] = None
+    if collection_metadata:
+        metadata = cls.propagate_collection_metadata(collection_metadata)
 
     return Segment(
         id=uuid4(),
         type=type.value,
         scope=scope,
         topic=collection["topic"],
         collection=collection["id"],
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/segment/impl/metadata/sqlite.py` & `chromadb-client-0.3.28.dev0/chromadb/segment/impl/metadata/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,25 @@
     LiteralValue,
     WhereOperator,
 )
 from uuid import UUID
 from pypika import Table, Tables
 from pypika.queries import QueryBuilder
 import pypika.functions as fn
-from pypika.terms import Criterion
+from pypika.terms import Criterion, Function
 from itertools import islice, groupby
-from chromadb.config import Component
 from functools import reduce
 import sqlite3
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-class SqliteMetadataSegment(Component, MetadataReader):
+class SqliteMetadataSegment(MetadataReader):
     _consumer: Consumer
     _db: SqliteDB
     _id: UUID
     _topic: Optional[str]
     _subscription: Optional[UUID]
 
     def __init__(self, system: System, segment: Segment):
@@ -210,14 +209,17 @@
             id = cur.execute(sql, params).fetchone()[0]
         except sqlite3.IntegrityError:
             # Can't use INSERT OR REPLACE here because it changes the primary key.
             if upsert:
                 return self._update_record(cur, record)
             else:
                 logger.warning(f"Insert of existing embedding ID: {record['id']}")
+                # We are trying to add for a record that already exists. Fail the call.
+                # We don't throw an exception since this is in principal an async path
+                return
 
         if record["metadata"]:
             self._update_metadata(cur, id, record["metadata"])
 
     def _update_metadata(self, cur: Cursor, id: int, metadata: UpdateMetadata) -> None:
         """Update the metadata for a single EmbeddingRecord"""
         t = Table("embedding_metadata")
@@ -229,15 +231,15 @@
                 .where(t.id == ParameterValue(id))
                 .where(t.key.isin(ParameterValue(to_delete)))
                 .delete()
             )
             sql, params = get_sql(q)
             cur.execute(sql, params)
 
-        if "document" in metadata:
+        if "chroma:document" in metadata:
             t = Table("embedding_fulltext")
             q = (
                 self._db.querybuilder()
                 .from_(t)
                 .where(t.id == ParameterValue(id))
                 .delete()
             )
@@ -281,21 +283,21 @@
                 )
 
         sql, params = get_sql(q)
         sql = sql.replace("INSERT", "INSERT OR REPLACE")
         if sql:
             cur.execute(sql, params)
 
-        if "document" in metadata:
+        if "chroma:document" in metadata:
             t = Table("embedding_fulltext")
             q = (
                 self._db.querybuilder()
                 .into(t)
                 .columns(t.id, t.string_value)
-                .insert(ParameterValue(id), ParameterValue(metadata["document"]))
+                .insert(ParameterValue(id), ParameterValue(metadata["chroma:document"]))
             )
             sql, params = get_sql(q)
             cur.execute(sql, params)
 
     def _delete_record(self, cur: Cursor, record: EmbeddingRecord) -> None:
         """Delete a single EmbeddingRecord from the DB"""
         t = Table("embeddings")
@@ -399,14 +401,24 @@
                     .select(metadata_t.id)
                     .where(metadata_t.key == ParameterValue(k))
                     .where(_where_clause(expr, metadata_t))
                 )
                 clause.append(embeddings_t.id.isin(sq))
         return reduce(lambda x, y: x & y, clause)
 
+    class EscapedLike(Function):  # type: ignore
+        def __init__(self, column_name: str, search_term: str, escape_char: str = "\\"):
+            self.column_name = column_name
+            self.search_term = search_term
+            self.escape_char = escape_char
+            super().__init__("LIKE", column_name, search_term)
+
+        def get_function_sql(self, **kwargs: Any) -> str:
+            return f"{self.column_name} LIKE {self.search_term} ESCAPE '{self.escape_char}'"
+
     def _where_doc_criterion(
         self,
         q: QueryBuilder,
         where: WhereDocument,
         embeddings_t: Table,
         fulltext_t: Table,
     ) -> Criterion:
@@ -420,27 +432,45 @@
             elif k == "$or":
                 criteria = [
                     self._where_doc_criterion(q, w, embeddings_t, fulltext_t)
                     for w in cast(Sequence[WhereDocument], v)
                 ]
                 return reduce(lambda x, y: x | y, criteria)
             elif k == "$contains":
-                search_term = f"%{v}%"
+                v = cast(str, v)
+                search_term = f"%{_escape_characters(v)}%"
+
                 sq = (
                     self._db.querybuilder()
                     .from_(fulltext_t)
                     .select(fulltext_t.id)
-                    .where(fulltext_t.string_value.like(ParameterValue(search_term)))
+                    .where(
+                        self.EscapedLike(
+                            fulltext_t.string_value,
+                            ParameterValue(search_term),
+                        )
+                    )
                 )
                 return embeddings_t.id.isin(sq)
             else:
                 raise ValueError(f"Unknown where_doc operator {k}")
         raise ValueError("Empty where_doc")
 
 
+def _escape_characters(string: str) -> str:
+    """Escape % and _ characters in a string with a backslash as they are reserved in
+    LIKE clauses"""
+    escaped_string = ""
+    for char in string:
+        if char == "%" or char == "_":
+            escaped_string += "\\"
+        escaped_string += char
+    return escaped_string
+
+
 def _encode_seq_id(seq_id: SeqId) -> bytes:
     """Encode a SeqID into a byte array"""
     if seq_id.bit_length() < 64:
         return int.to_bytes(seq_id, 8, "big")
     elif seq_id.bit_length() < 192:
         return int.to_bytes(seq_id, 24, "big")
     else:
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/segment/impl/vector/local_hnsw.py` & `chromadb-client-0.3.28.dev0/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from overrides import override
 from typing import Optional, Sequence, Dict, Set, List, Callable, Union, cast
 from uuid import UUID
 from chromadb.segment import VectorReader
 from chromadb.ingest import Consumer
-from chromadb.config import Component, System, Settings
+from chromadb.config import System, Settings
 from chromadb.types import (
     EmbeddingRecord,
     VectorEmbeddingRecord,
     VectorQuery,
     VectorQueryResult,
     SeqId,
     Segment,
@@ -44,24 +44,14 @@
     search_ef: int
     M: int
     num_threads: int
     resize_factor: float
 
     def __init__(self, metadata: Metadata):
         metadata = metadata or {}
-
-        for param, value in metadata.items():
-            if param.startswith("hnsw:"):
-                if param not in param_validators:
-                    raise ValueError(f"Unknown HNSW parameter: {param}")
-                if not param_validators[param](value):
-                    raise ValueError(
-                        f"Invalid value for HNSW parameter: {param} = {value}"
-                    )
-
         self.space = str(metadata.get("hnsw:space", "l2"))
         self.construction_ef = int(metadata.get("hnsw:construction_ef", 100))
         self.search_ef = int(metadata.get("hnsw:search_ef", 10))
         self.M = int(metadata.get("hnsw:M", 16))
         self.num_threads = int(
             metadata.get("hnsw:num_threads", multiprocessing.cpu_count())
         )
@@ -100,15 +90,15 @@
 
     def delete(self, label: int, id: str) -> None:
         self.delete_labels.append(label)
         self.delete_ids.append(id)
         self.delete_count += 1
 
 
-class LocalHnswSegment(Component, VectorReader):
+class LocalHnswSegment(VectorReader):
     _id: UUID
     _consumer: Consumer
     _topic: Optional[str]
     _subscription: UUID
     _settings: Settings
     _params: HnswParams
 
@@ -136,15 +126,33 @@
         self._max_seq_id = self._consumer.min_seqid()
 
         self._id_to_seq_id = {}
         self._id_to_label = {}
         self._label_to_id = {}
 
         self._lock = Lock()
-        super().__init__(system)
+        super().__init__(system, segment)
+
+    @staticmethod
+    @override
+    def propagate_collection_metadata(metadata: Metadata) -> Optional[Metadata]:
+        # Extract relevant metadata
+        segment_metadata = {}
+        for param, value in metadata.items():
+            if param.startswith("hnsw:"):
+                segment_metadata[param] = value
+
+        # Validate it
+        for param, value in segment_metadata.items():
+            if param not in param_validators:
+                raise ValueError(f"Unknown HNSW parameter: {param}")
+            if not param_validators[param](value):
+                raise ValueError(f"Invalid value for HNSW parameter: {param} = {value}")
+
+        return segment_metadata
 
     @override
     def start(self) -> None:
         super().start()
         if self._topic:
             seq_id = self.max_seqid()
             self._subscription = self._consumer.subscribe(
@@ -219,16 +227,22 @@
 
         all_results: List[List[VectorQueryResult]] = []
         for result_i in range(len(result_labels)):
             results: List[VectorQueryResult] = []
             for label, distance in zip(result_labels[result_i], distances[result_i]):
                 id = self._label_to_id[label]
                 seq_id = self._id_to_seq_id[id]
+                if query["include_embeddings"]:
+                    embedding = self._index.get_items([label])[0]
+                else:
+                    embedding = None
                 results.append(
-                    VectorQueryResult(id=id, seq_id=seq_id, distance=distance)
+                    VectorQueryResult(
+                        id=id, seq_id=seq_id, distance=distance, embedding=embedding
+                    )
                 )
             all_results.append(results)
 
         return all_results
 
     @override
     def max_seqid(self) -> SeqId:
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/server/fastapi/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/server/fastapi/types.py` & `chromadb-client-0.3.28.dev0/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/telemetry/__init__.py` & `chromadb-client-0.3.28.dev0/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/telemetry/events.py` & `chromadb-client-0.3.28.dev0/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/telemetry/posthog.py` & `chromadb-client-0.3.28.dev0/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/conftest.py` & `chromadb-client-0.3.28.dev0/chromadb/test/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,27 @@
 import pytest
 from typing import Generator, List, Callable
 import shutil
 import logging
 import socket
 import multiprocessing
 
+root_logger = logging.getLogger()
+root_logger.setLevel(logging.DEBUG)  # This will only run when testing
+
+
 logger = logging.getLogger(__name__)
 
 hypothesis.settings.register_profile(
     "dev",
     deadline=30000,
     suppress_health_check=[
         hypothesis.HealthCheck.data_too_large,
         hypothesis.HealthCheck.large_base_example,
+        hypothesis.HealthCheck.function_scoped_fixture,
     ],
 )
 hypothesis.settings.load_profile(os.getenv("HYPOTHESIS_PROFILE", "dev"))
 
 
 def find_free_port() -> int:
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
@@ -54,85 +59,109 @@
             raise e
         else:
             logger.info("Waiting for server to start...")
             time.sleep(4)
             _await_server(api, attempts + 1)
 
 
-def fastapi() -> Generator[API, None, None]:
+def fastapi() -> Generator[System, None, None]:
     """Fixture generator that launches a server in a separate process, and yields a
     fastapi client connect to it"""
     port = find_free_port()
     logger.info(f"Running test FastAPI server on port {port}")
     ctx = multiprocessing.get_context("spawn")
     proc = ctx.Process(target=_run_server, args=(port,), daemon=True)
     proc.start()
     settings = Settings(
         chroma_api_impl="rest",
         chroma_server_host="localhost",
         chroma_server_http_port=str(port),
+        allow_reset=True,
     )
     system = System(settings)
     api = system.instance(API)
-    _await_server(api)
     system.start()
-    yield api
+    _await_server(api)
+    yield system
     system.stop()
     proc.kill()
 
 
-def duckdb() -> Generator[API, None, None]:
+def duckdb() -> Generator[System, None, None]:
     """Fixture generator for duckdb"""
     settings = Settings(
         chroma_api_impl="local",
         chroma_db_impl="duckdb",
         persist_directory=tempfile.gettempdir(),
+        allow_reset=True,
     )
     system = System(settings)
-    api = system.instance(API)
     system.start()
-    yield api
+    yield system
     system.stop()
 
 
-def duckdb_parquet() -> Generator[API, None, None]:
+def duckdb_parquet() -> Generator[System, None, None]:
     """Fixture generator for duckdb+parquet"""
 
     save_path = tempfile.gettempdir() + "/tests"
     settings = Settings(
         chroma_api_impl="local",
         chroma_db_impl="duckdb+parquet",
         persist_directory=save_path,
+        allow_reset=True,
     )
     system = System(settings)
-    api = system.instance(API)
     system.start()
-    yield api
+    yield system
     system.stop()
     if os.path.exists(save_path):
         shutil.rmtree(save_path)
 
 
-def integration_api() -> Generator[API, None, None]:
+def integration() -> Generator[System, None, None]:
     """Fixture generator for returning a client configured via environmenet
     variables, intended for externally configured integration tests
     """
-    settings = Settings()
+    settings = Settings(allow_reset=True)
     system = System(settings)
-    api = system.instance(API)
     system.start()
-    yield api
+    yield system
     system.stop()
 
 
-def fixtures() -> List[Callable[[], Generator[API, None, None]]]:
-    api_fixtures = [duckdb, duckdb_parquet, fastapi]
+def sqlite() -> Generator[System, None, None]:
+    """Fixture generator for segment-based API using in-memory Sqlite"""
+    settings = Settings(
+        chroma_api_impl="chromadb.api.segment.SegmentAPI",
+        chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+        chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
+        chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
+        chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
+        sqlite_database=":memory:",
+        allow_reset=True,
+    )
+    system = System(settings)
+    system.start()
+    yield system
+    system.stop()
+
+
+def system_fixtures() -> List[Callable[[], Generator[System, None, None]]]:
+    fixtures = [duckdb, duckdb_parquet, fastapi, sqlite]
     if "CHROMA_INTEGRATION_TEST" in os.environ:
-        api_fixtures.append(integration_api)
+        fixtures.append(integration)
     if "CHROMA_INTEGRATION_TEST_ONLY" in os.environ:
-        api_fixtures = [integration_api]
-    return api_fixtures
+        fixtures = [integration]
+    return fixtures
 
 
-@pytest.fixture(scope="module", params=fixtures())
-def api(request: pytest.FixtureRequest) -> Generator[API, None, None]:
+@pytest.fixture(scope="module", params=system_fixtures())
+def system(request: pytest.FixtureRequest) -> Generator[API, None, None]:
     yield next(request.param())
+
+
+@pytest.fixture(scope="function")
+def api(system: System) -> Generator[API, None, None]:
+    system.reset_state()
+    api = system.instance(API)
+    yield api
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/db/test_base.py` & `chromadb-client-0.3.28.dev0/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/db/test_migrations.py` & `chromadb-client-0.3.28.dev0/chromadb/test/db/test_migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def test_exception_propagation(db: migrations.MigratableDB) -> None:
     with pytest.raises(Exception):
         with db.tx():
             raise (Exception("test exception"))
 
 
 def test_setup_migrations(db: migrations.MigratableDB) -> None:
-    db.reset()
+    db.reset_state()
     db.setup_migrations()
     db.setup_migrations()  # idempotent
 
     with db.tx() as cursor:
         rows = cursor.execute("SELECT * FROM migrations").fetchall()
         assert len(rows) == 0
 
@@ -94,15 +94,15 @@
 
     with db.tx() as cur:
         assert len(cur.execute("SELECT * FROM migrations").fetchall()) == 3
         assert len(cur.execute("SELECT * FROM table3").fetchall()) == 0
 
 
 def test_tampered_migration(db: migrations.MigratableDB) -> None:
-    db.reset()
+    db.reset_state()
 
     db.setup_migrations()
 
     source_migrations = migrations.find_migrations(
         "chromadb/test/db/migrations", db.migration_scope()
     )
 
@@ -138,15 +138,15 @@
             db_migrations, inconsistent_hash_migrations
         )
 
 
 def test_initialization(
     monkeypatch: pytest.MonkeyPatch, db: migrations.MigratableDB
 ) -> None:
-    db.reset()
+    db.reset_state()
     monkeypatch.setattr(db, "migration_dirs", lambda: ["chromadb/test/db/migrations"])
 
     assert not db.migrations_initialized()
 
     with pytest.raises(migrations.UninitializedMigrationsError):
         db.validate_migrations()
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/db/test_system.py` & `chromadb-client-0.3.28.dev0/chromadb/test/db/test_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,32 +28,35 @@
 
 sample_collections = [
     Collection(
         id=uuid.uuid4(),
         name="test_collection_1",
         topic="test_topic_1",
         metadata={"test_str": "str1", "test_int": 1, "test_float": 1.3},
+        dimension=128,
     ),
     Collection(
         id=uuid.uuid4(),
         name="test_collection_2",
         topic="test_topic_2",
         metadata={"test_str": "str2", "test_int": 2, "test_float": 2.3},
+        dimension=None,
     ),
     Collection(
         id=uuid.uuid4(),
         name="test_collection_3",
         topic="test_topic_3",
         metadata={"test_str": "str3", "test_int": 3, "test_float": 3.3},
+        dimension=None,
     ),
 ]
 
 
 def test_create_get_delete_collections(sysdb: SysDB) -> None:
-    sysdb.reset()
+    sysdb.reset_state()
 
     for collection in sample_collections:
         sysdb.create_collection(collection)
 
     results = sysdb.get_collections()
     results = sorted(results, key=lambda c: c["name"])
 
@@ -112,17 +115,18 @@
         "test_float": 1.3,
     }
     coll = Collection(
         id=uuid.uuid4(),
         name="test_collection_1",
         topic="test_topic_1",
         metadata=metadata,
+        dimension=None,
     )
 
-    sysdb.reset()
+    sysdb.reset_state()
 
     sysdb.create_collection(coll)
 
     # Update name
     coll["name"] = "new_name"
     sysdb.update_collection(coll["id"], name=coll["name"])
     result = sysdb.get_collections(name=coll["name"])
@@ -130,29 +134,23 @@
 
     # Update topic
     coll["topic"] = "new_topic"
     sysdb.update_collection(coll["id"], topic=coll["topic"])
     result = sysdb.get_collections(topic=coll["topic"])
     assert result == [coll]
 
-    # Add a new metadata key
-    metadata["test_str2"] = "str2"
-    sysdb.update_collection(coll["id"], metadata={"test_str2": "str2"})
+    # Update dimension
+    coll["dimension"] = 128
+    sysdb.update_collection(coll["id"], dimension=coll["dimension"])
     result = sysdb.get_collections(id=coll["id"])
     assert result == [coll]
 
-    # Update a metadata key
-    metadata["test_str"] = "str3"
-    sysdb.update_collection(coll["id"], metadata={"test_str": "str3"})
-    result = sysdb.get_collections(id=coll["id"])
-    assert result == [coll]
-
-    # Delete a metadata key
-    del metadata["test_str"]
-    sysdb.update_collection(coll["id"], metadata={"test_str": None})
+    # Reset the metadata
+    coll["metadata"] = {"test_str2": "str2"}
+    sysdb.update_collection(coll["id"], metadata=coll["metadata"])
     result = sysdb.get_collections(id=coll["id"])
     assert result == [coll]
 
     # Delete all metadata keys
     coll["metadata"] = None
     sysdb.update_collection(coll["id"], metadata=None)
     result = sysdb.get_collections(id=coll["id"])
@@ -184,15 +182,15 @@
         collection=None,
         metadata={"test_str": "str3", "test_int": 3, "test_float": 3.3},
     ),
 ]
 
 
 def test_create_get_delete_segments(sysdb: SysDB) -> None:
-    sysdb.reset()
+    sysdb.reset_state()
 
     for collection in sample_collections:
         sysdb.create_collection(collection)
 
     for segment in sample_segments:
         sysdb.create_segment(segment)
 
@@ -258,15 +256,15 @@
         type="test_type_a",
         scope=SegmentScope.VECTOR,
         topic="test_topic_a",
         collection=sample_collections[0]["id"],
         metadata=metadata,
     )
 
-    sysdb.reset()
+    sysdb.reset_state()
     for c in sample_collections:
         sysdb.create_collection(c)
 
     sysdb.create_segment(segment)
 
     # Update topic to new value
     segment["topic"] = "new_topic"
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/hnswlib/test_hnswlib.py` & `chromadb-client-0.3.28.dev0/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/ingest/test_producer_consumer.py` & `chromadb-client-0.3.28.dev0/chromadb/test/ingest/test_producer_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 @pytest.mark.asyncio
 async def test_backfill(
     producer_consumer: Tuple[Producer, Consumer],
     sample_embeddings: Iterator[SubmitEmbeddingRecord],
 ) -> None:
     producer, consumer = producer_consumer
-    producer.reset()
+    producer.reset_state()
 
     embeddings = [next(sample_embeddings) for _ in range(3)]
 
     producer.create_topic("test_topic")
     for e in embeddings:
         producer.submit_embedding("test_topic", e)
 
@@ -137,15 +137,15 @@
 
 @pytest.mark.asyncio
 async def test_notifications(
     producer_consumer: Tuple[Producer, Consumer],
     sample_embeddings: Iterator[SubmitEmbeddingRecord],
 ) -> None:
     producer, consumer = producer_consumer
-    producer.reset()
+    producer.reset_state()
     producer.create_topic("test_topic")
 
     embeddings: List[SubmitEmbeddingRecord] = []
 
     consume_fn = CapturingConsumeFn()
 
     consumer.subscribe("test_topic", consume_fn, start=consumer.min_seqid())
@@ -160,15 +160,15 @@
 
 @pytest.mark.asyncio
 async def test_multiple_topics(
     producer_consumer: Tuple[Producer, Consumer],
     sample_embeddings: Iterator[SubmitEmbeddingRecord],
 ) -> None:
     producer, consumer = producer_consumer
-    producer.reset()
+    producer.reset_state()
     producer.create_topic("test_topic_1")
     producer.create_topic("test_topic_2")
 
     embeddings_1: List[SubmitEmbeddingRecord] = []
     embeddings_2: List[SubmitEmbeddingRecord] = []
 
     consume_fn_1 = CapturingConsumeFn()
@@ -193,15 +193,15 @@
 
 @pytest.mark.asyncio
 async def test_start_seq_id(
     producer_consumer: Tuple[Producer, Consumer],
     sample_embeddings: Iterator[SubmitEmbeddingRecord],
 ) -> None:
     producer, consumer = producer_consumer
-    producer.reset()
+    producer.reset_state()
     producer.create_topic("test_topic")
 
     consume_fn_1 = CapturingConsumeFn()
     consume_fn_2 = CapturingConsumeFn()
 
     consumer.subscribe("test_topic", consume_fn_1, start=consumer.min_seqid())
 
@@ -227,15 +227,15 @@
 
 @pytest.mark.asyncio
 async def test_end_seq_id(
     producer_consumer: Tuple[Producer, Consumer],
     sample_embeddings: Iterator[SubmitEmbeddingRecord],
 ) -> None:
     producer, consumer = producer_consumer
-    producer.reset()
+    producer.reset_state()
     producer.create_topic("test_topic")
 
     consume_fn_1 = CapturingConsumeFn()
     consume_fn_2 = CapturingConsumeFn()
 
     consumer.subscribe("test_topic", consume_fn_1, start=consumer.min_seqid())
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/invariants.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/invariants.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,20 @@
         1,
         np_query,
     )
     # Sort the distances and return the indices
     return np.argsort(distances).tolist(), distances.tolist()
 
 
+def is_metadata_valid(normalized_record_set: NormalizedRecordSet) -> bool:
+    if normalized_record_set["metadatas"] is None:
+        return True
+    return not any([len(m) == 0 for m in normalized_record_set["metadatas"]])
+
+
 def ann_accuracy(
     collection: Collection,
     record_set: RecordSet,
     n_results: int = 1,
     min_recall: float = 0.99,
     embedding_function: Optional[types.EmbeddingFunction] = None,
 ) -> None:
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/strategies.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,20 +305,28 @@
     return metadata
 
 
 @st.composite
 def document(draw: st.DrawFn, collection: Collection) -> types.Document:
     """Strategy for generating documents that could be a part of the given collection"""
 
+    # Blacklist certain unicode characters that affect sqlite processing.
+    # For example, the null (/x00) character makes sqlite stop processing a string.
+    blacklist_categories = ("Cc", "Cs")
     if collection.known_document_keywords:
         known_words_st = st.sampled_from(collection.known_document_keywords)
     else:
-        known_words_st = st.text(min_size=1)
-
-    random_words_st = st.text(min_size=1)
+        known_words_st = st.text(
+            min_size=1,
+            alphabet=st.characters(blacklist_categories=blacklist_categories),
+        )
+
+    random_words_st = st.text(
+        min_size=1, alphabet=st.characters(blacklist_categories=blacklist_categories)
+    )
     words = draw(st.lists(st.one_of(known_words_st, random_words_st), min_size=1))
     return " ".join(words)
 
 
 @st.composite
 def recordsets(
     draw: st.DrawFn,
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/test_add.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/test_add.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,23 @@
 
     # TODO: Generative embedding functions
     coll = api.create_collection(
         name=collection.name,
         metadata=collection.metadata,
         embedding_function=collection.embedding_function,
     )
+    normalized_record_set = invariants.wrap_all(record_set)
+
+    if not invariants.is_metadata_valid(normalized_record_set):
+        with pytest.raises(Exception):
+            collection.add(**normalized_record_set)
+        return
+
     coll.add(**record_set)
 
-    normalized_record_set = invariants.wrap_all(record_set)
     invariants.count(coll, cast(strategies.RecordSet, normalized_record_set))
     n_results = max(1, (len(normalized_record_set["ids"]) // 10))
     invariants.ann_accuracy(
         coll,
         cast(strategies.RecordSet, normalized_record_set),
         n_results=n_results,
         embedding_function=collection.embedding_function,
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/test_collections.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/test_collections.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,18 @@
         self.api.reset()
         self.model = {}
 
     @rule(target=collections, coll=strategies.collections())
     def create_coll(
         self, coll: strategies.Collection
     ) -> MultipleResults[strategies.Collection]:
-        if coll.name in self.model:
+        # Metadata can either be None or a non-empty dict
+        if coll.name in self.model or (
+            coll.metadata is not None and len(coll.metadata) == 0
+        ):
             with pytest.raises(Exception):
                 c = self.api.create_collection(
                     name=coll.name,
                     metadata=coll.metadata,
                     embedding_function=coll.embedding_function,
                 )
             return multiple()
@@ -115,14 +118,23 @@
         # new_metadata is not none, coll is a new collection
         # get_or_create should create a new collection with the new metadata, ignoring
         # the metdata of in the input coll.
 
         # The fact that we ignore the metadata of the generated collections is a
         # bit weird, but it is the easiest way to excercise all cases
 
+        if new_metadata is not None and len(new_metadata) == 0:
+            with pytest.raises(Exception):
+                c = self.api.get_or_create_collection(
+                    name=coll.name,
+                    metadata=new_metadata,
+                    embedding_function=coll.embedding_function,
+                )
+            return multiple()
+
         # Update model
         if coll.name not in self.model:
             # Handles case 1 and 3
             coll.metadata = new_metadata
         else:
             # Handles case 0 and 2
             coll.metadata = (
@@ -158,14 +170,22 @@
             with pytest.raises(Exception):
                 c = self.api.get_collection(name=coll.name)
             return multiple()
 
         c = self.api.get_collection(name=coll.name)
 
         if new_metadata is not None:
+            if len(new_metadata) == 0:
+                with pytest.raises(Exception):
+                    c = self.api.get_or_create_collection(
+                        name=coll.name,
+                        metadata=new_metadata,
+                        embedding_function=coll.embedding_function,
+                    )
+                return multiple()
             coll.metadata = new_metadata
             self.model[coll.name] = coll.metadata
 
         if new_name is not None:
             if new_name in self.model and new_name != coll.name:
                 with pytest.raises(Exception):
                     c.modify(metadata=new_metadata, name=new_name)
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/test_cross_version_persist.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/test_cross_version_persist.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,17 @@
     embeddings_strategy=strategies.recordsets(collection_st),
 )
 @pytest.mark.skipif(
     sys.version_info.major < 3
     or (sys.version_info.major == 3 and sys.version_info.minor <= 7),
     reason="The mininum supported versions of chroma do not work with python <= 3.7",
 )
+@pytest.mark.xfail(
+    reason="As we migrate to sqlite, we will not support old versions of chromadb and instead require manual migration. The minimum version will be increased to 0.4.0 and this test will be expected to pass."
+)
 @settings(deadline=None)
 def test_cycle_versions(
     version_settings: Tuple[str, Settings],
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
 ) -> None:
     # # Test backwards compatibility
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/test_embeddings.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/test_embeddings.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import hypothesis.strategies as st
 from typing import Set, cast, Union, DefaultDict
 from dataclasses import dataclass
 from chromadb.api.types import ID, Include, IDs
 import chromadb.errors as errors
 from chromadb.api import API
 from chromadb.api.models.Collection import Collection
+from chromadb.db.impl.sqlite import SqliteDB
 import chromadb.test.property.strategies as strategies
 from hypothesis.stateful import (
     Bundle,
     RuleBasedStateMachine,
     MultipleResults,
     rule,
     initialize,
@@ -93,20 +94,42 @@
         normalized_record_set: strategies.NormalizedRecordSet = invariants.wrap_all(
             record_set
         )
 
         if len(normalized_record_set["ids"]) > 0:
             trace("add_more_embeddings")
 
-        if set(normalized_record_set["ids"]).intersection(
-            set(self.record_set_state["ids"])
-        ):
-            with pytest.raises(errors.IDAlreadyExistsError):
+        if not invariants.is_metadata_valid(normalized_record_set):
+            with pytest.raises(Exception):
                 self.collection.add(**normalized_record_set)
             return multiple()
+
+        intersection = set(normalized_record_set["ids"]).intersection(
+            self.record_set_state["ids"]
+        )
+        if len(intersection) > 0:
+            # Partially apply the non-duplicative records to the state
+            new_ids = list(set(normalized_record_set["ids"]).difference(intersection))
+            indices = [normalized_record_set["ids"].index(id) for id in new_ids]
+            filtered_record_set: strategies.NormalizedRecordSet = {
+                "ids": [normalized_record_set["ids"][i] for i in indices],
+                "metadatas": [normalized_record_set["metadatas"][i] for i in indices]
+                if normalized_record_set["metadatas"]
+                else None,
+                "documents": [normalized_record_set["documents"][i] for i in indices]
+                if normalized_record_set["documents"]
+                else None,
+                "embeddings": [normalized_record_set["embeddings"][i] for i in indices]
+                if normalized_record_set["embeddings"]
+                else None,
+            }
+            self.collection.add(**normalized_record_set)
+            self._upsert_embeddings(cast(strategies.RecordSet, filtered_record_set))
+            return multiple(*filtered_record_set["ids"])
+
         else:
             self.collection.add(**normalized_record_set)
             self._upsert_embeddings(cast(strategies.RecordSet, normalized_record_set))
             return multiple(*normalized_record_set["ids"])
 
     @precondition(lambda self: len(self.record_set_state["ids"]) > 20)
     @rule(ids=st.lists(consumes(embedding_ids), min_size=1, max_size=20))
@@ -128,14 +151,23 @@
             min_size=1,
             max_size=5,
         )
     )
     def update_embeddings(self, record_set: strategies.RecordSet) -> None:
         trace("update embeddings")
         self.on_state_change(EmbeddingStateMachineStates.update_embeddings)
+
+        normalized_record_set: strategies.NormalizedRecordSet = invariants.wrap_all(
+            record_set
+        )
+        if not invariants.is_metadata_valid(normalized_record_set):
+            with pytest.raises(Exception):
+                self.collection.update(**normalized_record_set)
+            return
+
         self.collection.update(**record_set)
         self._upsert_embeddings(record_set)
 
     # Using a value < 3 causes more retries and lowers the number of valid samples
     @precondition(lambda self: len(self.record_set_state["ids"]) >= 3)
     @rule(
         record_set=strategies.recordsets(
@@ -144,14 +176,23 @@
             min_size=1,
             max_size=5,
         )
     )
     def upsert_embeddings(self, record_set: strategies.RecordSet) -> None:
         trace("upsert embeddings")
         self.on_state_change(EmbeddingStateMachineStates.upsert_embeddings)
+
+        normalized_record_set: strategies.NormalizedRecordSet = invariants.wrap_all(
+            record_set
+        )
+        if not invariants.is_metadata_valid(normalized_record_set):
+            with pytest.raises(Exception):
+                self.collection.upsert(**normalized_record_set)
+            return
+
         self.collection.upsert(**record_set)
         self._upsert_embeddings(record_set)
 
     @invariant()
     def count(self) -> None:
         invariants.count(
             self.collection, cast(strategies.RecordSet, self.record_set_state)
@@ -189,17 +230,27 @@
                         target_idx
                     ] = self.embedding_function(
                         [normalized_record_set["documents"][idx]]
                     )[
                         0
                     ]
                 if normalized_record_set["metadatas"] is not None:
-                    self.record_set_state["metadatas"][
-                        target_idx
-                    ] = normalized_record_set["metadatas"][idx]
+                    # Sqlite merges the metadata, as opposed to old
+                    # implementations which overwrites it
+                    record_set_state = self.record_set_state["metadatas"][target_idx]
+                    if (
+                        hasattr(self.api, "_sysdb")
+                        and type(self.api._sysdb) == SqliteDB
+                        and record_set_state is not None
+                    ):
+                        record_set_state.update(normalized_record_set["metadatas"][idx])
+                    else:
+                        self.record_set_state["metadatas"][
+                            target_idx
+                        ] = normalized_record_set["metadatas"][idx]
                 if normalized_record_set["documents"] is not None:
                     self.record_set_state["documents"][
                         target_idx
                     ] = normalized_record_set["documents"][idx]
             else:
                 # Add path
                 self.record_set_state["ids"].append(id)
@@ -250,16 +301,17 @@
 
 def test_multi_add(api: API) -> None:
     api.reset()
     coll = api.create_collection(name="foo")
     coll.add(ids=["a"], embeddings=[[0.0]])
     assert coll.count() == 1
 
-    with pytest.raises(errors.IDAlreadyExistsError):
-        coll.add(ids=["a"], embeddings=[[0.0]])
+    # after the sqlite refactor - add silently ignores duplicates, no exception is raised
+    # partial adds are supported - i.e we will add whatever we can in the request
+    coll.add(ids=["a"], embeddings=[[0.0]])
 
     assert coll.count() == 1
 
     results = coll.get()
     assert results["ids"] == ["a"]
 
     coll.delete(ids=["a"])
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/test_filtering.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/test_filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,24 +142,30 @@
 )  # type: ignore
 @given(
     collection=collection_st,
     record_set=recordset_st,
     filters=st.lists(strategies.filters(collection_st, recordset_st), min_size=1),
 )
 def test_filterable_metadata_get(
-    caplog, api: API, collection, record_set, filters
+    caplog, api: API, collection: strategies.Collection, record_set, filters
 ) -> None:
     caplog.set_level(logging.ERROR)
 
     api.reset()
     coll = api.create_collection(
         name=collection.name,
         metadata=collection.metadata,
         embedding_function=collection.embedding_function,
     )
+
+    if not invariants.is_metadata_valid(invariants.wrap_all(record_set)):
+        with pytest.raises(Exception):
+            coll.add(**record_set)
+        return
+
     coll.add(**record_set)
 
     for filter in filters:
         result_ids = coll.get(**filter)["ids"]
         expected_ids = _filter_embedding_set(record_set, filter)
         assert sorted(result_ids) == sorted(expected_ids)
 
@@ -186,19 +192,25 @@
     filters: List[strategies.Filter],
 ) -> None:
     caplog.set_level(logging.ERROR)
 
     api.reset()
     coll = api.create_collection(
         name=collection.name,
-        metadata=collection.metadata,
+        metadata=collection.metadata,  # type: ignore
         embedding_function=collection.embedding_function,
     )
-    coll.add(**record_set)
     normalized_record_set = invariants.wrap_all(record_set)
+
+    if not invariants.is_metadata_valid(normalized_record_set):
+        with pytest.raises(Exception):
+            coll.add(**record_set)
+        return
+
+    coll.add(**record_set)
     total_count = len(normalized_record_set["ids"])
     # Pick a random vector
     random_query: Embedding
     if collection.has_embeddings:
         assert normalized_record_set["embeddings"] is not None
         assert all(isinstance(e, list) for e in normalized_record_set["embeddings"])
         random_query = normalized_record_set["embeddings"][
@@ -255,7 +267,24 @@
         where={"test": "yes"},
         n_results=3,
     )
     assert res["ids"] == [[], []]
     assert res["embeddings"] is None
     assert res["distances"] == [[], []]
     assert res["metadatas"] == [[], []]
+
+
+@pytest.mark.xfail(reason="Boolean metadata is not supported yet")
+def test_boolean_metadata(api: API) -> None:
+    """Test that metadata with boolean values is correctly filtered"""
+    api.reset()
+    coll = api.create_collection(name="test")
+
+    test_ids: IDs = ["1", "2", "3"]
+    test_embeddings: Embeddings = [[1, 1], [2, 2], [3, 3]]
+    test_metadatas: Metadatas = [{"test": True}, {"test": False}, {"test": True}]
+
+    coll.add(ids=test_ids, embeddings=test_embeddings, metadatas=test_metadatas)
+
+    res = coll.get(where={"test": True})
+
+    assert res["ids"] == ["1", "3"]
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/property/test_persist.py` & `chromadb-client-0.3.28.dev0/chromadb/test/property/test_persist.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,19 @@
     api_1.reset()
     coll = api_1.create_collection(
         name=collection_strategy.name,
         metadata=collection_strategy.metadata,
         embedding_function=collection_strategy.embedding_function,
     )
 
+    if not invariants.is_metadata_valid(invariants.wrap_all(embeddings_strategy)):
+        with pytest.raises(Exception):
+            coll.add(**embeddings_strategy)
+        return
+
     coll.add(**embeddings_strategy)
 
     invariants.count(coll, embeddings_strategy)
     invariants.metadatas_match(coll, embeddings_strategy)
     invariants.documents_match(coll, embeddings_strategy)
     invariants.ids_match(coll, embeddings_strategy)
     invariants.ann_accuracy(
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/segment/test_metadata.py` & `chromadb-client-0.3.28.dev0/chromadb/test/segment/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         metadata: Optional[Dict[str, Union[str, int, float]]]
         if i == 0:
             metadata = None
         else:
             metadata = {"str_key": f"value_{i}", "int_key": i, "float_key": i + i * 0.1}
             if i % 3 == 0:
                 metadata["div_by_three"] = "true"
-            metadata["document"] = _build_document(i)
+            metadata["chroma:document"] = _build_document(i)
 
         record = SubmitEmbeddingRecord(
             id=f"embedding_{i}",
             embedding=vector,
             encoding=ScalarEncoding.FLOAT32,
             metadata=metadata,
             operation=Operation.ADD,
@@ -102,15 +102,15 @@
         time.sleep(0.25)
     raise TimeoutError(f"Timed out waiting for seq_id {seq_id}")
 
 
 def test_insert_and_count(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     max_id = 0
     for i in range(3):
         max_id = producer.submit_embedding(topic, next(sample_embeddings))
@@ -140,15 +140,15 @@
         assert e["id"] == a["id"]
         assert e["metadata"] == a["metadata"]
 
 
 def test_get(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
 
     producer = system.instance(Producer)
     topic = str(segment_definition["topic"])
 
     embeddings = [next(sample_embeddings) for i in range(10)]
 
     seq_ids = []
@@ -238,29 +238,29 @@
     )
     assert len(result) == 1
 
 
 def test_fulltext(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
 
     producer = system.instance(Producer)
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
     max_id = 0
     for i in range(100):
         max_id = producer.submit_embedding(topic, next(sample_embeddings))
 
     sync(segment, max_id)
 
-    result = segment.get_metadata(where={"document": "four two"})
+    result = segment.get_metadata(where={"chroma:document": "four two"})
     result2 = segment.get_metadata(ids=["embedding_42"])
     assert result == result2
 
     # Test single result
     result = segment.get_metadata(where_document={"$contains": "four two"})
     assert len(result) == 1
 
@@ -300,15 +300,15 @@
     result = segment.get_metadata(where_document={"$contains": "zer"})
     assert len(result) == 9
 
 
 def test_delete(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
 
     producer = system.instance(Producer)
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
@@ -363,15 +363,15 @@
     assert segment.count() == 10
     results = segment.get_metadata(ids=["embedding_0"])
 
 
 def test_update(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
 
     producer = system.instance(Producer)
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
@@ -391,15 +391,15 @@
     assert len(results) == 0
     assert segment.count() == 3
 
 
 def test_upsert(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
 
     producer = system.instance(Producer)
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
@@ -438,60 +438,60 @@
 
     results = segment.get_metadata(ids=["embedding_0"])
     assert_equiv_records(embeddings[:1], results)
 
     # Update embedding with no metadata
     update_record = SubmitEmbeddingRecord(
         id="embedding_0",
-        metadata={"document": "foo bar"},
+        metadata={"chroma:document": "foo bar"},
         embedding=None,
         encoding=None,
         operation=op,
     )
     max_id = producer.submit_embedding(topic, update_record)
     sync(segment, max_id)
     results = segment.get_metadata(ids=["embedding_0"])
-    assert results[0]["metadata"] == {"document": "foo bar"}
+    assert results[0]["metadata"] == {"chroma:document": "foo bar"}
     results = segment.get_metadata(where_document={"$contains": "foo"})
-    assert results[0]["metadata"] == {"document": "foo bar"}
+    assert results[0]["metadata"] == {"chroma:document": "foo bar"}
 
     # Update and overrwrite key
     update_record = SubmitEmbeddingRecord(
         id="embedding_0",
-        metadata={"document": "biz buz"},
+        metadata={"chroma:document": "biz buz"},
         embedding=None,
         encoding=None,
         operation=op,
     )
     max_id = producer.submit_embedding(topic, update_record)
     sync(segment, max_id)
     results = segment.get_metadata(ids=["embedding_0"])
-    assert results[0]["metadata"] == {"document": "biz buz"}
+    assert results[0]["metadata"] == {"chroma:document": "biz buz"}
     results = segment.get_metadata(where_document={"$contains": "biz"})
-    assert results[0]["metadata"] == {"document": "biz buz"}
+    assert results[0]["metadata"] == {"chroma:document": "biz buz"}
     results = segment.get_metadata(where_document={"$contains": "foo"})
     assert len(results) == 0
 
     # Update and add key
     update_record = SubmitEmbeddingRecord(
         id="embedding_0",
         metadata={"baz": 42},
         embedding=None,
         encoding=None,
         operation=op,
     )
     max_id = producer.submit_embedding(topic, update_record)
     sync(segment, max_id)
     results = segment.get_metadata(ids=["embedding_0"])
-    assert results[0]["metadata"] == {"document": "biz buz", "baz": 42}
+    assert results[0]["metadata"] == {"chroma:document": "biz buz", "baz": 42}
 
     # Update and delete key
     update_record = SubmitEmbeddingRecord(
         id="embedding_0",
-        metadata={"document": None},
+        metadata={"chroma:document": None},
         embedding=None,
         encoding=None,
         operation=op,
     )
     max_id = producer.submit_embedding(topic, update_record)
     sync(segment, max_id)
     results = segment.get_metadata(ids=["embedding_0"])
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/segment/test_vector.py` & `chromadb-client-0.3.28.dev0/chromadb/test/segment/test_vector.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         time.sleep(0.25)
     raise TimeoutError(f"Timed out waiting for seq_id {seq_id}")
 
 
 def test_insert_and_count(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     max_id = 0
     for i in range(3):
         max_id = producer.submit_embedding(topic, next(sample_embeddings))
@@ -112,15 +112,15 @@
 def approx_equal_vector(a: Vector, b: Vector, epsilon: float = 0.0001) -> bool:
     return all(approx_equal(x, y, epsilon) for x, y in zip(a, b))
 
 
 def test_get_vectors(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     segment = LocalHnswSegment(system, segment_definition)
     segment.start()
 
@@ -155,15 +155,15 @@
         )
         assert actual["seq_id"] == seq_id
 
 
 def test_ann_query(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     segment = LocalHnswSegment(system, segment_definition)
     segment.start()
 
@@ -174,47 +174,59 @@
         seq_ids.append(producer.submit_embedding(topic, e))
 
     sync(segment, seq_ids[-1])
 
     # Each item is its own nearest neighbor (one at a time)
     for e in embeddings:
         vector = cast(Vector, e["embedding"])
-        query = VectorQuery(vectors=[vector], k=1, allowed_ids=None, options=None)
+        query = VectorQuery(
+            vectors=[vector],
+            k=1,
+            allowed_ids=None,
+            options=None,
+            include_embeddings=True,
+        )
         results = segment.query_vectors(query)
         assert len(results) == 1
         assert len(results[0]) == 1
         assert results[0][0]["id"] == e["id"]
+        assert results[0][0]["embedding"] is not None
+        assert approx_equal_vector(results[0][0]["embedding"], vector)
 
     # Each item is its own nearest neighbor (all at once)
     vectors = [cast(Vector, e["embedding"]) for e in embeddings]
-    query = VectorQuery(vectors=vectors, k=1, allowed_ids=None, options=None)
+    query = VectorQuery(
+        vectors=vectors, k=1, allowed_ids=None, options=None, include_embeddings=False
+    )
     results = segment.query_vectors(query)
     assert len(results) == len(embeddings)
     for r, e in zip(results, embeddings):
         assert len(r) == 1
         assert r[0]["id"] == e["id"]
 
     # Each item's 3 nearest neighbors are itself and the item before and after
     test_embeddings = embeddings[1:-1]
     vectors = [cast(Vector, e["embedding"]) for e in test_embeddings]
-    query = VectorQuery(vectors=vectors, k=3, allowed_ids=None, options=None)
+    query = VectorQuery(
+        vectors=vectors, k=3, allowed_ids=None, options=None, include_embeddings=False
+    )
     results = segment.query_vectors(query)
     assert len(results) == len(test_embeddings)
 
     for r, e, i in zip(results, test_embeddings, range(1, len(test_embeddings))):
         assert len(r) == 3
         assert r[0]["id"] == embeddings[i]["id"]
         assert r[1]["id"] == embeddings[i - 1]["id"]
         assert r[2]["id"] == embeddings[i + 1]["id"]
 
 
 def test_delete(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     segment = LocalHnswSegment(system, segment_definition)
     segment.start()
 
@@ -253,15 +265,17 @@
         assert actual["id"] == expected["id"]
         assert approx_equal_vector(
             actual["embedding"], cast(Vector, expected["embedding"])
         )
 
     # Assert that the record is gone from KNN search
     vector = cast(Vector, embeddings[0]["embedding"])
-    query = VectorQuery(vectors=[vector], k=10, allowed_ids=None, options=None)
+    query = VectorQuery(
+        vectors=[vector], k=10, allowed_ids=None, options=None, include_embeddings=False
+    )
     knn_results = segment.query_vectors(query)
     assert len(results) == 4
     assert set(r["id"] for r in knn_results[0]) == set(e["id"] for e in embeddings[1:])
 
     # Delete is idempotent
     seq_ids.append(
         producer.submit_embedding(
@@ -319,33 +333,37 @@
     results = segment.get_vectors()
     assert len(results) == 3
     results = segment.get_vectors(ids=[embeddings[0]["id"]])
     assert results[0]["embedding"] == [10.0, 10.0]
 
     # Test querying at the old location
     vector = cast(Vector, embeddings[0]["embedding"])
-    query = VectorQuery(vectors=[vector], k=3, allowed_ids=None, options=None)
+    query = VectorQuery(
+        vectors=[vector], k=3, allowed_ids=None, options=None, include_embeddings=False
+    )
     knn_results = segment.query_vectors(query)[0]
     assert knn_results[0]["id"] == embeddings[1]["id"]
     assert knn_results[1]["id"] == embeddings[2]["id"]
     assert knn_results[2]["id"] == embeddings[0]["id"]
 
     # Test querying at the new location
     vector = [10.0, 10.0]
-    query = VectorQuery(vectors=[vector], k=3, allowed_ids=None, options=None)
+    query = VectorQuery(
+        vectors=[vector], k=3, allowed_ids=None, options=None, include_embeddings=False
+    )
     knn_results = segment.query_vectors(query)[0]
     assert knn_results[0]["id"] == embeddings[0]["id"]
     assert knn_results[1]["id"] == embeddings[2]["id"]
     assert knn_results[2]["id"] == embeddings[1]["id"]
 
 
 def test_update(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     segment = LocalHnswSegment(system, segment_definition)
     segment.start()
 
@@ -368,15 +386,15 @@
     assert segment.count() == 3
     assert segment.get_vectors(ids=["no_such_record"]) == []
 
 
 def test_upsert(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset()
+    system.reset_state()
     producer = system.instance(Producer)
 
     topic = str(segment_definition["topic"])
 
     segment = LocalHnswSegment(system, segment_definition)
     segment.start()
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/test_api.py` & `chromadb-client-0.3.28.dev0/chromadb/test/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import chromadb
 from chromadb.api.types import QueryResult
 from chromadb.config import Settings
 import chromadb.server.fastapi
 import pytest
 import tempfile
 import numpy as np
+from datetime import datetime, timedelta
 from chromadb.utils.embedding_functions import (
     DefaultEmbeddingFunction,
 )
 
 
 @pytest.fixture
 def local_persist_api():
@@ -30,14 +31,24 @@
             chroma_api_impl="local",
             chroma_db_impl="duckdb+parquet",
             persist_directory=tempfile.gettempdir() + "/test_server",
         )
     )
 
 
+def approx_equal(a, b, tolerance=1e-6) -> bool:
+    return abs(a - b) < tolerance
+
+
+def vector_approx_equal(a, b, tolerance: float = 1e-6) -> bool:
+    if len(a) != len(b):
+        return False
+    return all([approx_equal(a, b, tolerance) for a, b in zip(a, b)])
+
+
 @pytest.mark.parametrize("api_fixture", [local_persist_api])
 def test_persist_index_loading(api_fixture, request):
     api = request.getfixturevalue("local_persist_api")
     api.reset()
     collection = api.create_collection("test")
     collection.add(ids="id1", documents="hello")
 
@@ -136,15 +147,20 @@
     del api
 
     api = request.getfixturevalue(api_fixture.__name__)
     assert api.list_collections() == []
 
 
 def test_heartbeat(api):
-    assert isinstance(api.heartbeat(), int)
+    heartbeat_ns = api.heartbeat()
+    assert isinstance(heartbeat_ns, int)
+
+    heartbeat_s = heartbeat_ns // 10**9
+    heartbeat = datetime.fromtimestamp(heartbeat_s)
+    assert heartbeat > datetime.now() - timedelta(seconds=10)
 
 
 batch_records = {
     "embeddings": [[1.1, 2.3, 3.2], [1.2, 2.24, 3.2]],
     "ids": ["https://example.com/1", "https://example.com/2"],
 }
 
@@ -976,15 +992,15 @@
     assert items["ids"][0] == "id1"
     assert items["metadatas"][0]["int_value"] == 1
     assert items["documents"][0] == "this document is first"
 
     items = collection.get(include=["embeddings", "documents"])
     assert items["metadatas"] is None
     assert items["ids"][0] == "id1"
-    assert items["embeddings"][1][0] == 1.2
+    assert approx_equal(items["embeddings"][1][0], 1.2)
 
     items = collection.get(include=[])
     assert items["documents"] is None
     assert items["metadatas"] is None
     assert items["embeddings"] is None
     assert items["ids"][0] == "id1"
 
@@ -1202,15 +1218,17 @@
         n_results=1,
         include=["embeddings", "documents", "metadatas"],
     )
     assert len(results["ids"][0]) == 1
     assert results["ids"][0][0] == updated_records["ids"][0]
     assert results["documents"][0][0] == updated_records["documents"][0]
     assert results["metadatas"][0][0]["foo"] == "bar"
-    assert results["embeddings"][0][0] == updated_records["embeddings"][0]
+    assert vector_approx_equal(
+        results["embeddings"][0][0], updated_records["embeddings"][0]
+    )
 
 
 def test_get_nearest_neighbors_where_n_results_more_than_element(api):
     api.reset()
     collection = api.create_collection("testspace")
     collection.add(**records)
 
@@ -1289,39 +1307,43 @@
 
     collection.upsert(**new_records)
     assert collection.count() == 4
 
     get_result = collection.get(
         include=["embeddings", "metadatas", "documents"], ids=new_records["ids"][0]
     )
-    assert get_result["embeddings"][0] == new_records["embeddings"][0]
+    assert vector_approx_equal(
+        get_result["embeddings"][0], new_records["embeddings"][0]
+    )
     assert get_result["metadatas"][0] == new_records["metadatas"][0]
     assert get_result["documents"][0] == new_records["documents"][0]
 
     query_result = collection.query(
         query_embeddings=get_result["embeddings"],
         n_results=1,
         include=["embeddings", "metadatas", "documents"],
     )
-    assert query_result["embeddings"][0][0] == new_records["embeddings"][0]
+    assert vector_approx_equal(
+        query_result["embeddings"][0][0], new_records["embeddings"][0]
+    )
     assert query_result["metadatas"][0][0] == new_records["metadatas"][0]
     assert query_result["documents"][0][0] == new_records["documents"][0]
 
     collection.delete(ids=initial_records["ids"][2])
     collection.upsert(
         ids=initial_records["ids"][2],
         embeddings=[[1.1, 0.99, 2.21]],
         metadatas=[{"string_value": "a new string value"}],
     )
     assert collection.count() == 4
 
     get_result = collection.get(
         include=["embeddings", "metadatas", "documents"], ids=["id3"]
     )
-    assert get_result["embeddings"][0] == [1.1, 0.99, 2.21]
+    assert vector_approx_equal(get_result["embeddings"][0], [1.1, 0.99, 2.21])
     assert get_result["metadatas"][0] == {"string_value": "a new string value"}
     assert get_result["documents"][0] is None
 
 
 # test to make sure add, query, update, upsert error on invalid embeddings input
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/test_chroma.py` & `chromadb-client-0.3.28.dev0/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/test_config.py` & `chromadb-client-0.3.28.dev0/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/test/utils/test_messagid.py` & `chromadb-client-0.3.28.dev0/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb/types.py` & `chromadb-client-0.3.28.dev0/chromadb/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 class Collection(TypedDict):
     id: UUID
     name: str
     topic: str
     metadata: Optional[Metadata]
+    dimension: Optional[int]
 
 
 class Segment(TypedDict):
     id: UUID
     type: NamespacedName
     scope: SegmentScope
     # If a segment has a topic, it implies that this segment is a consumer of the topic
@@ -93,23 +94,25 @@
 
 class VectorQuery(TypedDict):
     """A KNN/ANN query"""
 
     vectors: Sequence[Vector]
     k: int
     allowed_ids: Optional[Sequence[str]]
+    include_embeddings: bool
     options: Optional[Dict[str, Union[str, int, float]]]
 
 
 class VectorQueryResult(TypedDict):
     """A KNN/ANN query result"""
 
     id: str
     seq_id: SeqId
     distance: float
+    embedding: Optional[Vector]
 
 
 # Metadata Query Grammar
 LiteralValue = Union[str, int, float]
 LogicalOperator = Union[Literal["$and"], Literal["$or"]]
 WhereOperator = Union[
     Literal["$gt"],
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/utils/embedding_functions.py` & `chromadb-client-0.3.28.dev0/chromadb/utils/embedding_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,37 @@
 
 class SentenceTransformerEmbeddingFunction(EmbeddingFunction):
     # Since we do dynamic imports we have to type this as Any
     models: Dict[str, Any] = {}
 
     # If you have a beefier machine, try "gtr-t5-large".
     # for a full list of options: https://huggingface.co/sentence-transformers, https://www.sbert.net/docs/pretrained_models.html
-    def __init__(self, model_name: str = "all-MiniLM-L6-v2", device: str = "cpu"):
+    def __init__(
+        self,
+        model_name: str = "all-MiniLM-L6-v2",
+        device: str = "cpu",
+        normalize_embeddings: bool = False,
+    ):
         if model_name not in self.models:
             try:
                 from sentence_transformers import SentenceTransformer
             except ImportError:
                 raise ValueError(
                     "The sentence_transformers python package is not installed. Please install it with `pip install sentence_transformers`"
                 )
             self.models[model_name] = SentenceTransformer(model_name, device=device)
         self._model = self.models[model_name]
+        self._normalize_embeddings = normalize_embeddings
 
     def __call__(self, texts: Documents) -> Embeddings:
-        return self._model.encode(list(texts), convert_to_numpy=True).tolist()  # type: ignore # noqa E501
+        return self._model.encode(
+            list(texts),
+            convert_to_numpy=True,
+            normalize_embeddings=self._normalize_embeddings,
+        ).tolist()
 
 
 class Text2VecEmbeddingFunction(EmbeddingFunction):
     def __init__(self, model_name: str = "shibing624/text2vec-base-chinese"):
         try:
             from text2vec import SentenceModel
         except ImportError:
@@ -346,14 +356,15 @@
         return [
             self._palm.generate_embeddings(model=self._model_name, text=text)[
                 "embedding"
             ]
             for text in texts
         ]
 
+
 class GoogleVertexEmbeddingFunction(EmbeddingFunction):
     # Follow API Quickstart for Google Vertex AI
     # https://cloud.google.com/vertex-ai/docs/generative-ai/start/quickstarts/api-quickstart
     # Information about the text embedding modules in Google Vertex AI
     # https://cloud.google.com/vertex-ai/docs/generative-ai/embeddings/get-text-embeddings
     def __init__(
         self,
@@ -369,8 +380,8 @@
     def __call__(self, texts: Documents) -> Embeddings:
         response = self._session.post(
             self._api_url, json={"instances": [{"content": texts}]}
         ).json()
 
         if "predictions" in response:
             return response["predictions"]
-        return {}
+        return []
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb/utils/messageid.py` & `chromadb-client-0.3.28.dev0/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/chromadb_client.egg-info/PKG-INFO` & `chromadb-client-0.3.28.dev0/chromadb_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.27.dev0
+Version: 0.3.28.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
 client = chromadb.Client(Settings(chroma_api_impl="rest",
                                   chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+                                  chroma_server_http_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.27.dev0 Summary:
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.28.dev0 Summary:
 Chroma Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
 you can do the following: ```python import chromadb from chromadb.config import
 Settings # Example setup of the client to connect to your chroma server client
 = chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_port=8000)) collection =
+chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
 client.create_collection("all-my-documents") collection.add( documents=["This
 is document1", "This is document2"], metadatas=[{"source": "notion"},
 {"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
 for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
 collection.query( query_texts=["This is a query document"], n_results=2, #
 where={"metadata_field": "is_equal_to_this"}, # optional filter #
 where_document={"$contains":"search_string"} # optional filter ) ``` ## License
```

### Comparing `chromadb-client-0.3.27.dev0/chromadb_client.egg-info/SOURCES.txt` & `chromadb-client-0.3.28.dev0/chromadb_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -42,28 +42,30 @@
 chromadb/config.py
 chromadb/errors.py
 chromadb/is_thin_client.py
 chromadb/types.py
 chromadb/api/__init__.py
 chromadb/api/fastapi.py
 chromadb/api/local.py
+chromadb/api/segment.py
 chromadb/api/types.py
 chromadb/api/models/Collection.py
 chromadb/db/__init__.py
 chromadb/db/base.py
 chromadb/db/clickhouse.py
 chromadb/db/duckdb.py
 chromadb/db/migrations.py
 chromadb/db/system.py
 chromadb/db/impl/__init__.py
 chromadb/db/impl/sqlite.py
 chromadb/db/index/__init__.py
 chromadb/db/index/hnswlib.py
 chromadb/db/mixins/embeddings_queue.py
 chromadb/db/mixins/sysdb.py
+chromadb/experimental/density_relevance.ipynb
 chromadb/ingest/__init__.py
 chromadb/segment/__init__.py
 chromadb/segment/impl/manager/local.py
 chromadb/segment/impl/metadata/sqlite.py
 chromadb/segment/impl/vector/local_hnsw.py
 chromadb/server/__init__.py
 chromadb/server/fastapi/__init__.py
@@ -123,25 +125,25 @@
 clients/js/examples/browser/README.md
 clients/js/examples/browser/app.ts
 clients/js/examples/browser/index.html
 clients/js/examples/browser/package.json
 clients/js/examples/browser/yarn.lock
 clients/js/examples/node/README.md
 clients/js/examples/node/app.js
-clients/js/examples/node/package-lock.json
 clients/js/examples/node/package.json
 clients/js/examples/node/yarn.lock
 clients/js/src/ChromaClient.ts
 clients/js/src/Collection.ts
 clients/js/src/index.ts
 clients/js/src/types.ts
 clients/js/src/utils.ts
 clients/js/src/embeddings/CohereEmbeddingFunction.ts
 clients/js/src/embeddings/IEmbeddingFunction.ts
 clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+clients/js/src/embeddings/TransformersEmbeddingFunction.ts
 clients/js/src/embeddings/WebAIEmbeddingFunction.ts
 clients/js/src/generated/README.md
 clients/js/src/generated/api.ts
 clients/js/src/generated/configuration.ts
 clients/js/src/generated/index.ts
 clients/js/src/generated/models.ts
 clients/js/src/generated/runtime.ts
@@ -160,19 +162,24 @@
 clients/python/README.md
 clients/python/build_python_thin_client.sh
 clients/python/integration-test.sh
 clients/python/is_thin_client.py
 clients/python/pyproject.toml
 config/backup_disk.xml
 config/chroma_users.xml
-examples/alternative_embeddings.ipynb
-examples/local_persistence.ipynb
-examples/where_filtering.ipynb
+examples/README.md
+examples/basic_functionality/alternative_embeddings.ipynb
+examples/basic_functionality/local_persistence.ipynb
+examples/basic_functionality/where_filtering.ipynb
 examples/deployments/google-cloud-compute/README.md
 examples/deployments/google-cloud-compute/chroma.tf
 examples/deployments/google-cloud-compute/main.tf
 examples/deployments/google-cloud-compute/startup.sh
 examples/deployments/google-cloud-compute/variables.tf
+examples/use_with/cohere/cohere_js.js
+examples/use_with/cohere/cohere_python.ipynb
+examples/use_with/cohere/package.json
 migrations/embeddings_queue/00001-embeddings.sqlite.sql
 migrations/metadb/00001-embedding-metadata.sqlite.sql
 migrations/sysdb/00001-collections.sqlite.sql
-migrations/sysdb/00002-segments.sqlite.sql
+migrations/sysdb/00002-segments.sqlite.sql
+migrations/sysdb/00003-collection-dimension.sqlite.sql
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/DEVELOP.md` & `chromadb-client-0.3.28.dev0/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/LICENSE` & `chromadb-client-0.3.28.dev0/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/README.md` & `chromadb-client-0.3.28.dev0/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/examples/browser/app.ts` & `chromadb-client-0.3.28.dev0/clients/js/examples/browser/app.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import { ChromaClient } from '../../src/ChromaClient';
 // import env.ts
 
 window.onload = async () => {
-  const chroma = new ChromaClient("http://localhost:8000");
+  const chroma = new ChromaClient({ path: "http://localhost:8000" });
   await chroma.reset();
 
-  const collection = await chroma.createCollection("test-from-js");
+  const collection = await chroma.createCollection({ name: "test-from-js" });
   console.log("collection", collection);
 
   // first generate some data
   var ids: string[] = [];
   var embeddings: Array<any> = [];
-  var metadata: Array<any> = [];
+  var metadatas: Array<any> = [];
   for (let i = 0; i < 100; i++) {
     ids.push("test-id-" + i.toString());
     embeddings.push([1, 2, 3, 4, 5]);
-    metadata.push({ test: "test" });
+    metadatas.push({ test: "test" });
   }
 
-  let add = await collection.add(ids, embeddings, metadata);
+  let add = await collection.add({ ids, embeddings, metadatas });
   console.log("add", add);
 
   let count = await collection.count();
   console.log("count", count);
 
-  const queryData = await collection.query([1, 2, 3, 4, 5], 5, {
-    test: "test",
+  const queryData = await collection.query({
+    queryEmbeddings: [1, 2, 3, 4, 5],
+    nResults: 5,
+    where: { test: "test" }
   });
 
   console.log("queryData", queryData);
 
   await collection.delete();
 
   let count2 = await collection.count();
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/examples/browser/index.html` & `chromadb-client-0.3.28.dev0/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/examples/browser/yarn.lock` & `chromadb-client-0.3.28.dev0/clients/js/examples/browser/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -743,35 +743,14 @@
 ansi-styles@^4.1.0:
   version "4.3.0"
   resolved "https://registry.yarnpkg.com/ansi-styles/-/ansi-styles-4.3.0.tgz#edd803628ae71c04c85ae7a0906edad34b648937"
   integrity sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==
   dependencies:
     color-convert "^2.0.1"
 
-asynckit@^0.4.0:
-  version "0.4.0"
-  resolved "https://registry.yarnpkg.com/asynckit/-/asynckit-0.4.0.tgz#c79ed97f7f34cb8f2ba1bc9790bcc366474b4b79"
-  integrity sha512-Oei9OH4tRh0YqU3GxhX79dM/mwVgvbZJaSNaRk+bshkj0S5cfHcgYakreBjrHwatXKbz+IoIdYLxrKim2MjW0Q==
-
-axios@^0.26.0:
-  version "0.26.1"
-  resolved "https://registry.yarnpkg.com/axios/-/axios-0.26.1.tgz#1ede41c51fcf51bbbd6fd43669caaa4f0495aaa9"
-  integrity sha512-fPwcX4EvnSHuInCMItEhAGnaSEXRBjtzh9fOtsE6E1G6p7vl7edEeZe11QHf18+6+9gR5PbKV/sGKNaD8YaMeA==
-  dependencies:
-    follow-redirects "^1.14.8"
-
-axios@^1.3.3:
-  version "1.3.3"
-  resolved "https://registry.yarnpkg.com/axios/-/axios-1.3.3.tgz#e7011384ba839b885007c9c9fae1ff23dceb295b"
-  integrity sha512-eYq77dYIFS77AQlhzEL937yUBSepBfPIe8FcgEDN35vMNZKMrs81pgnyrQpwfy4NF4b4XWX1Zgx7yX+25w8QJA==
-  dependencies:
-    follow-redirects "^1.15.0"
-    form-data "^4.0.0"
-    proxy-from-env "^1.1.0"
-
 base-x@^3.0.8:
   version "3.0.9"
   resolved "https://registry.yarnpkg.com/base-x/-/base-x-3.0.9.tgz#6349aaabb58526332de9f60995e548a53fe21320"
   integrity sha512-H7JU6iBHTal1gp56aKoaa//YUxEaAOUiydvrV/pILqIHXTtqxSkATOnDA2u+jZ/61sD+L/412+7kzXRtWukhpQ==
   dependencies:
     safe-buffer "^5.0.1"
 
@@ -825,20 +804,18 @@
   version "4.1.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-4.1.2.tgz#aac4e2b7734a740867aeb16bf02aad556a1e7a01"
   integrity sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==
   dependencies:
     ansi-styles "^4.1.0"
     supports-color "^7.1.0"
 
-chromadb@1.2.1:
-  version "1.2.1"
-  resolved "https://registry.yarnpkg.com/chromadb/-/chromadb-1.2.1.tgz#3883dd20f0b85967341e491ccdd58d1930e5da67"
-  integrity sha512-QGW8H+w72fIS49W5N4RyYNlLLXZIL6Q9mI+zddaDfEr4Dn5FtTTtvkUPef4y34w5qtNp8MMArXwyhzWQhUKleQ==
-  dependencies:
-    axios "^0.26.0"
+chromadb@1.5.0:
+  version "1.5.0"
+  resolved "https://registry.yarnpkg.com/chromadb/-/chromadb-1.5.0.tgz#80d97d9db08fca07a8b2554f1327429de19ed8b9"
+  integrity sha512-uBHbgykL5lYuXXaTst3H9P/539pC8vJNe7pzkyl8oGVWgJJjrgA8XGyFstTjG8EjjxxUpTUh8GcU4LmfgOu9dg==
 
 chrome-trace-event@^1.0.2:
   version "1.0.3"
   resolved "https://registry.yarnpkg.com/chrome-trace-event/-/chrome-trace-event-1.0.3.tgz#1015eced4741e15d06664a957dbbf50d041e26ac"
   integrity sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==
 
 clone@^2.1.1:
@@ -866,21 +843,14 @@
   integrity sha512-72fSenhMw2HZMTVHeCA9KCmpEIbzWiQsjN+BHcBbS9vr1mtt+vJjPdksIBNUmKAW8TFUDPJK5SUU3QhE9NEXDw==
 
 color-name@~1.1.4:
   version "1.1.4"
   resolved "https://registry.yarnpkg.com/color-name/-/color-name-1.1.4.tgz#c2a09a87acbde69543de6f63fa3995c826c536a2"
   integrity sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==
 
-combined-stream@^1.0.8:
-  version "1.0.8"
-  resolved "https://registry.yarnpkg.com/combined-stream/-/combined-stream-1.0.8.tgz#c3d45a8b34fd730631a110a8a2520682b31d5a7f"
-  integrity sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==
-  dependencies:
-    delayed-stream "~1.0.0"
-
 commander@^2.20.0:
   version "2.20.3"
   resolved "https://registry.yarnpkg.com/commander/-/commander-2.20.3.tgz#fd485e84c03eb4881c20722ba48035e8531aeb33"
   integrity sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==
 
 commander@^7.0.0, commander@^7.2.0:
   version "7.2.0"
@@ -925,19 +895,14 @@
 csso@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/csso/-/csso-4.2.0.tgz#ea3a561346e8dc9f546d6febedd50187cf389529"
   integrity sha512-wvlcdIbf6pwKEk7vHj8/Bkc0B4ylXZruLvOgs9doS5eOsOpuodOV2zJChSpkp+pRpYQLQMeF04nr3Z68Sta9jA==
   dependencies:
     css-tree "^1.1.2"
 
-delayed-stream@~1.0.0:
-  version "1.0.0"
-  resolved "https://registry.yarnpkg.com/delayed-stream/-/delayed-stream-1.0.0.tgz#df3ae199acadfb7d440aaae0b29e2272b24ec619"
-  integrity sha512-ZySD7Nf91aLB0RxL4KGrKHBXl7Eds1DAmEdcoVawXnLD7SDhpNgtuII2aAkg7a7QS41jxPSZ17p4VdGnMHk3MQ==
-
 detect-libc@^1.0.3:
   version "1.0.3"
   resolved "https://registry.yarnpkg.com/detect-libc/-/detect-libc-1.0.3.tgz#fa137c4bd698edf55cd5cd02ac559f91a4c4ba9b"
   integrity sha512-pGjwhsmsp4kL2RTz08wcOlGN83otlqHeD/Z5T8GXZB+/YcpQ/dgo+lbU8ZsGxV0HIvqqxo9l7mqYwyYMD9bKDg==
 
 dom-serializer@^1.0.1:
   version "1.4.1"
@@ -1014,28 +979,14 @@
 fill-range@^7.0.1:
   version "7.0.1"
   resolved "https://registry.yarnpkg.com/fill-range/-/fill-range-7.0.1.tgz#1919a6a7c75fe38b2c7c77e5198535da9acdda40"
   integrity sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==
   dependencies:
     to-regex-range "^5.0.1"
 
-follow-redirects@^1.14.8, follow-redirects@^1.15.0:
-  version "1.15.2"
-  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.15.2.tgz#b460864144ba63f2681096f274c4e57026da2c13"
-  integrity sha512-VQLG33o04KaQ8uYi2tVNbdrWp1QWxNNea+nmIB4EVM28v0hmP17z7aG1+wAkNzVq4KeXTq3221ye5qTJP91JwA==
-
-form-data@^4.0.0:
-  version "4.0.0"
-  resolved "https://registry.yarnpkg.com/form-data/-/form-data-4.0.0.tgz#93919daeaf361ee529584b9b31664dc12c9fa452"
-  integrity sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==
-  dependencies:
-    asynckit "^0.4.0"
-    combined-stream "^1.0.8"
-    mime-types "^2.1.12"
-
 get-port@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/get-port/-/get-port-4.2.0.tgz#e37368b1e863b7629c43c5a323625f95cf24b119"
   integrity sha512-/b3jarXkH8KJoOMQc3uVGHASwGLPq3gSFJ7tgJm2diza+bydJPTGOibin2steecKeOylE8oY2JERlVWkAJO6yw==
 
 globals@^13.2.0:
   version "13.20.0"
@@ -1211,26 +1162,14 @@
   version "4.0.5"
   resolved "https://registry.yarnpkg.com/micromatch/-/micromatch-4.0.5.tgz#bc8999a7cbbf77cdc89f132f6e467051b49090c6"
   integrity sha512-DMy+ERcEW2q8Z2Po+WNXuw3c5YaUSFjAO5GsJqfEl7UjvtIuFKO6ZrKvcItdy98dwFI2N1tg3zNIdKaQT+aNdA==
   dependencies:
     braces "^3.0.2"
     picomatch "^2.3.1"
 
-mime-db@1.52.0:
-  version "1.52.0"
-  resolved "https://registry.yarnpkg.com/mime-db/-/mime-db-1.52.0.tgz#bbabcdc02859f4987301c856e3387ce5ec43bf70"
-  integrity sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==
-
-mime-types@^2.1.12:
-  version "2.1.35"
-  resolved "https://registry.yarnpkg.com/mime-types/-/mime-types-2.1.35.tgz#381a871b62a734450660ae3deee44813f70d959a"
-  integrity sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==
-  dependencies:
-    mime-db "1.52.0"
-
 msgpackr-extract@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/msgpackr-extract/-/msgpackr-extract-3.0.0.tgz#5b5c5fbfff25be5ee5b5a82a9cbe02e37f72bed0"
   integrity sha512-oy6KCk1+X4Bn5m6Ycq5N1EWl9npqG/cLrE8ga8NX7ZqfqYUUBS08beCQaGq80fjbKBySur0E6x//yZjzNJDt3A==
   dependencies:
     node-gyp-build-optional-packages "5.0.7"
   optionalDependencies:
@@ -1382,19 +1321,14 @@
     posthtml-render "^3.0.0"
 
 process@^0.11.10:
   version "0.11.10"
   resolved "https://registry.yarnpkg.com/process/-/process-0.11.10.tgz#7332300e840161bda3e69a1d1d91a7d4bc16f182"
   integrity sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==
 
-proxy-from-env@^1.1.0:
-  version "1.1.0"
-  resolved "https://registry.yarnpkg.com/proxy-from-env/-/proxy-from-env-1.1.0.tgz#e102f16ca355424865755d2c9e8ea4f24d58c3e2"
-  integrity sha512-D+zkORCbA9f1tdWRK0RaCR3GPv50cMxcrz4X8k5LTSUD1Dkw47mKJEZQNunItRTkWwgtaUSo1RVFRIG9ZXiFYg==
-
 react-error-overlay@6.0.9:
   version "6.0.9"
   resolved "https://registry.yarnpkg.com/react-error-overlay/-/react-error-overlay-6.0.9.tgz#3c743010c9359608c375ecd6bc76f35d93995b0a"
   integrity sha512-nQTTcUu+ATDbrSD1BZHr5kgSD4oF8OFjxun8uAaL8RwPBacGBNPf/yAuVVdx17N8XNzRDMrZ9XcKZHCjPW+9ew==
 
 react-refresh@^0.9.0:
   version "0.9.0"
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/examples/node/yarn.lock` & `chromadb-client-0.3.28.dev0/clients/js/examples/node/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,17 +55,15 @@
   resolved "https://registry.npmjs.org/call-bind/-/call-bind-1.0.2.tgz"
   integrity sha512-7O+FbCihrB5WGbFYesctwmTKae6rOiIzmz1icreWJ+0aA7LJfuqhEso2T9ncpcFtzMQtzXf2QGGueWJGTYsqrA==
   dependencies:
     function-bind "^1.1.1"
     get-intrinsic "^1.0.2"
 
 "chromadb@file:../..":
-  version "1.2.1"
-  dependencies:
-    axios "^0.26.0"
+  version "1.5.0"
 
 cohere-ai@^5.0.2:
   version "5.0.2"
   resolved "https://registry.npmjs.org/cohere-ai/-/cohere-ai-5.0.2.tgz"
   integrity sha512-Svt8VC20/GgwCBF2kHYZI3JZkfqEoG6wCbTT6tohNK8x/aBFyMxlBUYEF0gRGXH1055vQpBjj5ewHF8LpnSSOA==
 
 combined-stream@^1.0.8:
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/genapi.sh` & `chromadb-client-0.3.28.dev0/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/package-lock.json` & `chromadb-client-0.3.28.dev0/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/package.json` & `chromadb-client-0.3.28.dev0/clients/js/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.5.3'"}*

```diff
@@ -35,9 +35,9 @@
         "release": "run-s build test:run && npm publish",
         "test": "run-s db:clean db:run test:runfull db:clean",
         "test:run": "jest --runInBand",
         "test:runfull": "PORT=8001 jest --runInBand",
         "test:set-port": "cross-env URL=localhost:8001",
         "test:update": "run-s db:clean db:run && jest --runInBand --updateSnapshot && run-s db:clean"
     },
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/ChromaClient.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/ChromaClient.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 import { IEmbeddingFunction } from './embeddings/IEmbeddingFunction';
 import { Configuration, ApiApi as DefaultApi, Api } from "./generated";
 import { handleSuccess, handleError } from "./utils";
 import { Collection } from './Collection';
-import { CollectionMetadata, CollectionType } from './types';
+import { CollectionMetadata, CollectionType, ConfigOptions } from './types';
 
 
 export class ChromaClient {
     /**
      * @ignore
      */
-    private api: DefaultApi;
+    private api: DefaultApi & ConfigOptions;
 
     /**
      * Creates a new ChromaClient instance.
      * @param {Object} params - The parameters for creating a new client
      * @param {string} [params.path] - The base path for the Chroma API.
      * @returns {ChromaClient} A new ChromaClient instance.
      *
      * @example
      * ```typescript
      * const client = new ChromaClient({
      *   path: "http://localhost:8000"
      * });
      * ```
      */
-    constructor({ path }: { path?: string } = {}) {
+    constructor({
+        path,
+        fetchOptions
+    }: {
+        path?: string,
+        fetchOptions?: RequestInit
+    } = {}) {
         if (path === undefined) path = "http://localhost:8000";
         const apiConfig: Configuration = new Configuration({
             basePath: path,
         });
         this.api = new DefaultApi(apiConfig);
+        this.api.options = fetchOptions ?? {};
     }
 
     /**
      * Resets the state of the object by making an API call to the reset endpoint.
      *
      * @returns {Promise<Api.Reset200Response>} A promise that resolves when the reset operation is complete.
      * @throws {Error} If there is an issue resetting the state.
      *
      * @example
      * ```typescript
      * await client.reset();
      * ```
      */
     public async reset(): Promise<Api.Reset200Response> {
-        return await this.api.reset();
+        return await this.api.reset(this.api.options);
     }
 
     /**
      * Returns the version of the Chroma API.
      * @returns {Promise<string>} A promise that resolves to the version of the Chroma API.
      *
      * @example
      * ```typescript
      * const version = await client.version();
      * ```
      */
     public async version(): Promise<string> {
-        const response = await this.api.version();
+        const response = await this.api.version(this.api.options);
         return await handleSuccess(response);
     }
 
     /**
      * Returns a heartbeat from the Chroma API.
      * @returns {Promise<number>} A promise that resolves to the heartbeat from the Chroma API.
      *
      * @example
      * ```typescript
      * const heartbeat = await client.heartbeat();
      * ```
      */
     public async heartbeat(): Promise<number> {
-        const response = await this.api.heartbeat();
+        const response = await this.api.heartbeat(this.api.options);
         let ret = await handleSuccess(response);
         return ret["nanosecond heartbeat"]
     }
 
     /**
      * @ignore
      */
@@ -113,15 +120,15 @@
         metadata?: CollectionMetadata,
         embeddingFunction?: IEmbeddingFunction
     }): Promise<Collection> {
         const newCollection = await this.api
             .createCollection({
                 name,
                 metadata,
-            })
+            }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
 
         if (newCollection.error) {
             throw new Error(newCollection.error);
         }
 
@@ -159,15 +166,15 @@
         embeddingFunction?: IEmbeddingFunction
     }): Promise<Collection> {
         const newCollection = await this.api
             .createCollection({
                 name,
                 metadata,
                 'get_or_create': true
-            })
+            }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
 
         if (newCollection.error) {
             throw new Error(newCollection.error);
         }
 
@@ -188,15 +195,15 @@
      *
      * @example
      * ```typescript
      * const collections = await client.listCollections();
      * ```
      */
     public async listCollections(): Promise<CollectionType[]> {
-        const response = await this.api.listCollections();
+        const response = await this.api.listCollections(this.api.options);
         return handleSuccess(response);
     }
 
     /**
      * Gets a collection with the specified name.
      * @param {Object} params - The parameters for getting a collection.
      * @param {string} params.name - The name of the collection.
@@ -215,29 +222,30 @@
         name,
         embeddingFunction
     }: {
         name: string;
         embeddingFunction?: IEmbeddingFunction
     }): Promise<Collection> {
         const response = await this.api
-            .getCollection(name)
+            .getCollection(name, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
 
         if (response.error) {
             throw new Error(response.error);
         }
 
         return new Collection(
             response.name,
             response.id,
             this.api,
             response.metadata,
             embeddingFunction
         );
+
     }
 
     /**
      * Deletes a collection with the specified name.
      * @param {Object} params - The parameters for deleting a collection.
      * @param {string} params.name - The name of the collection.
      * @returns {Promise<void>} A promise that resolves when the collection is deleted.
@@ -252,13 +260,13 @@
      */
     public async deleteCollection({
         name
     }: {
         name: string
     }): Promise<void> {
         return await this.api
-            .deleteCollection(name)
+            .deleteCollection(name, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
     }
 
 }
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/Collection.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/Collection.ts`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,31 @@
     WhereDocument,
     ID,
     IDs,
     PositiveInteger,
     GetResponse,
     QueryResponse,
     AddResponse,
-    CollectionMetadata
+    CollectionMetadata,
+    ConfigOptions
 } from "./types";
 import { IEmbeddingFunction } from './embeddings/IEmbeddingFunction';
 import { ApiApi as DefaultApi } from "./generated";
 import { handleError, handleSuccess } from "./utils";
 import { toArray, toArrayOfArrays } from "./utils";
 
 
 export class Collection {
     public name: string;
     public id: string;
     public metadata: CollectionMetadata | undefined;
     /**
      * @ignore
      */
-    private api: DefaultApi;
+    private api: DefaultApi & ConfigOptions;
     /**
      * @ignore
      */
     public embeddingFunction: IEmbeddingFunction | undefined;
 
     /**
      * @ignore
@@ -151,15 +152,15 @@
     /**
      * Add items to the collection
      * @param {Object} params - The parameters for the query.
      * @param {ID | IDs} [params.ids] - IDs of the items to add.
      * @param {Embedding | Embeddings} [params.embeddings] - Optional embeddings of the items to add.
      * @param {Metadata | Metadatas} [params.metadatas] - Optional metadata of the items to add.
      * @param {Document | Documents} [params.documents] - Optional documents of the items to add.
-     * @returns {Promise<AddResponse>} - The response from the API. True if successful.
+    * @returns {Promise<AddResponse>} - The response from the API. True if successful.
      *
      * @example
      * ```typescript
      * const response = await collection.add({
      *   ids: ["id1", "id2"],
      *   embeddings: [[1, 2, 3], [4, 5, 6]],
      *   metadatas: [{ "key": "value" }, { "key": "value" }],
@@ -191,15 +192,15 @@
             {
                 // @ts-ignore
                 ids: idsArray,
                 embeddings: embeddingsArray as number[][], // We know this is defined because of the validate function
                 // @ts-ignore
                 documents: documentsArray,
                 metadatas: metadatasArray,
-            })
+            }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
 
         return response
     }
 
     /**
@@ -245,14 +246,15 @@
                 //@ts-ignore
                 ids: idsArray,
                 embeddings: embeddingsArray as number[][], // We know this is defined because of the validate function
                 //@ts-ignore
                 documents: documentsArray,
                 metadatas: metadatasArray,
             },
+            this.api.options
         )
             .then(handleSuccess)
             .catch(handleError);
 
         return response
 
     }
@@ -263,15 +265,15 @@
      *
      * @example
      * ```typescript
      * const response = await collection.count();
      * ```
      */
     public async count(): Promise<number> {
-        const response = await this.api.count(this.id);
+        const response = await this.api.count(this.id, this.api.options);
         return handleSuccess(response);
     }
 
     /**
      * Modify the collection name or metadata
      * @param {Object} params - The parameters for the query.
      * @param {string} [params.name] - Optional new name for the collection.
@@ -296,14 +298,15 @@
         const response = await this.api
             .updateCollection(
                 this.id,
                 {
                     new_name: name,
                     new_metadata: metadata,
                 },
+                this.api.options
             )
             .then(handleSuccess)
             .catch(handleError);
 
         this.setName(name || this.name);
         this.setMetadata(metadata || this.metadata);
 
@@ -356,15 +359,15 @@
             .aGet(this.id, {
                 ids: idsArray,
                 where,
                 limit,
                 offset,
                 include,
                 where_document: whereDocument,
-            })
+            }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
     }
 
     /**
      * Update the embeddings, documents, and/or metadatas of existing items
      * @param {Object} params - The parameters for the query.
@@ -423,14 +426,15 @@
                 this.id,
                 {
                     ids: toArray(ids),
                     embeddings: embeddings ? toArrayOfArrays(embeddings) : undefined,
                     documents: documents,
                     metadatas: metadatas
                 },
+                this.api.options
             )
             .then(handleSuccess)
             .catch(handleError);
 
         return resp;
     }
 
@@ -505,15 +509,15 @@
         return await this.api
             .getNearestNeighbors(this.id, {
                 query_embeddings: query_embeddingsArray,
                 where,
                 n_results: nResults,
                 where_document: whereDocument,
                 include: include,
-            })
+            }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
     }
 
     /**
      * Peek inside the collection
      * @param {Object} params - The parameters for the query.
@@ -528,15 +532,15 @@
      * });
      * ```
      */
     public async peek({ limit }: { limit?: PositiveInteger } = {}): Promise<GetResponse> {
         if (limit === undefined) limit = 10;
         const response = await this.api.aGet(this.id, {
             limit: limit,
-        });
+        }, this.api.options);
         return handleSuccess(response);
     }
 
     /**
      * Deletes items from the collection.
      * @param {Object} params - The parameters for deleting items from the collection.
      * @param {ID | IDs} [params.ids] - Optional ID or array of IDs of items to delete.
@@ -562,12 +566,12 @@
         ids?: ID | IDs,
         where?: Where,
         whereDocument?: WhereDocument
     } = {}): Promise<string[]> {
         let idsArray = undefined;
         if (ids !== undefined) idsArray = toArray(ids);
         return await this.api
-            .aDelete(this.id, { ids: idsArray, where: where, where_document: whereDocument })
+            .aDelete(this.id, { ids: idsArray, where: where, where_document: whereDocument }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
     }
 }
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     private api_key: string;
     private model: string;
 
     constructor({ cohere_api_key, model }: { cohere_api_key: string, model?: string }) {
         try {
             // eslint-disable-next-line global-require,import/no-extraneous-dependencies
             CohereAiApi = require("cohere-ai");
+            CohereAiApi.init(cohere_api_key);
         } catch {
             throw new Error(
                 "Please install the cohere-ai package to use the CohereEmbeddingFunction, `npm install -S cohere-ai`"
             );
         }
         this.api_key = cohere_api_key;
         this.model = model || "large";
@@ -22,8 +23,8 @@
     public async generate(texts: string[]) {
         const response = await CohereAiApi.embed({
             texts: texts,
             model: this.model,
         });
         return response.body.embeddings;
     }
-}
+}
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
         });
         const data = response.data["data"];
         for (let i = 0; i < data.length; i += 1) {
             embeddings.push(data[i]["embedding"]);
         }
         return embeddings;
     }
-}
+}
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/generated/README.md` & `chromadb-client-0.3.28.dev0/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/generated/api.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/generated/configuration.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/generated/models.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/generated/runtime.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/types.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/types.ts`

 * *Files 23% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   [key: string]: LiteralValue | OperatorExpression;
 };
 
 type LogicalWhere = {
   [key in LogicalOperator]?: Where[];
 };
 
-export type Where = BaseWhere & LogicalWhere;
+export type Where = BaseWhere | LogicalWhere;
 
 type WhereDocumentOperator = "$contains" | LogicalOperator;
 
 export type WhereDocument = {
   [key in WhereDocumentOperator]?: LiteralValue | LiteralNumber | WhereDocument[];
 };
 
@@ -68,7 +68,13 @@
 }
 
 export type AddResponse = {
   error: string;
 }
 
 export type CollectionMetadata = Record<string, unknown>;
+
+// RequestInit can be used to set Authorization headers and more
+// see all options here: https://www.jsdocs.io/package/@types/node-fetch#RequestInit
+export type ConfigOptions = {
+  options?: RequestInit;
+};
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/src/utils.ts` & `chromadb-client-0.3.28.dev0/clients/js/src/utils.ts`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         }
     } else {
         return value;
     }
 }
 
 export async function handleError(error: unknown) {
+
     if (error instanceof Response) {
         try {
             const res = await error.json();
             if ("error" in res) {
                 return { error: res.error };
             }
         } catch (e: unknown) {
@@ -58,8 +59,8 @@
         case response instanceof Response:
             return repack(await (response as Response).json());
         case typeof response === "string":
             return repack((response as string)); // currently version is the only thing that return non-JSON
         default:
             return repack(response);
     }
-}
+}
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/add.collections.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/add.collections.test.ts`

 * *Files 11% similar despite different names*

```diff
@@ -40,23 +40,14 @@
   const collection = await chroma.createCollection({ name: "test" });
   let resp = await collection.add({ ids: IDS, embeddings: EMBEDDINGS, documents: DOCUMENTS });
   expect(resp).toBe(true)
   const results = await collection.get({ ids: ["test1"] });
   expect(results.documents[0]).toBe("This is a test");
 });
 
-test('it should return an error when inserting an ID that alreay exists in the Collection', async () => {
-  await chroma.reset()
-  const collection = await chroma.createCollection({ name: "test" });
-  await collection.add({ ids: IDS, embeddings: EMBEDDINGS, metadatas: METADATAS })
-  const results = await collection.add({ ids: IDS, embeddings: EMBEDDINGS, metadatas: METADATAS });
-  expect(results.error).toBeDefined()
-  expect(results.error).toContain("IDAlreadyExists")
-})
-
 test('It should return an error when inserting duplicate IDs in the same batch', async () => {
   await chroma.reset()
   const collection = await chroma.createCollection({ name: "test" });
   const ids = IDS.concat(["test1"])
   const embeddings = EMBEDDINGS.concat([[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]])
   const metadatas = METADATAS.concat([{ test: 'test1', 'float_value': 0.1 }])
   try {
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/client.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/collection.client.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/collection.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/delete.collection.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/get.collection.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/peek.collection.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/query.collection.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/query.collection.test.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 import { expect, test } from "@jest/globals";
 import chroma from "./initClient";
 import { IncludeEnum } from "../src/types";
 import { EMBEDDINGS, IDS, METADATAS, DOCUMENTS } from "./data";
 
+import { IEmbeddingFunction } from "../src/embeddings/IEmbeddingFunction";
+
+export class TestEmbeddingFunction implements IEmbeddingFunction {
+
+  constructor() { }
+
+  public async generate(texts: string[]): Promise<number[][]> {
+    let embeddings: number[][] = [];
+    for (let i = 0; i < texts.length; i += 1) {
+      embeddings.push([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
+    }
+    return embeddings;
+  }
+}
+
 test("it should query a collection", async () => {
   await chroma.reset();
   const collection = await chroma.createCollection({ name: "test" });
   await collection.add({ ids: IDS, embeddings: EMBEDDINGS });
   const results = await collection.query({ queryEmbeddings: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], nResults: 2 });
   expect(results).toBeDefined();
   expect(results).toBeInstanceOf(Object);
@@ -43,7 +58,31 @@
     include: [IncludeEnum.Embeddings]
   });
 
   // expect(results2.embeddings[0][0]).toBeInstanceOf(Array);
   expect(results2.embeddings![0].length).toBe(1);
   expect(results2.embeddings![0][0]).toEqual([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
 });
+
+
+// test queryTexts
+test("it should query a collection with text", async () => {
+  await chroma.reset();
+  let embeddingFunction = new TestEmbeddingFunction();
+  const collection = await chroma.createCollection({ name: "test", embeddingFunction: embeddingFunction });
+  await collection.add({ ids: IDS, embeddings: EMBEDDINGS, metadatas: METADATAS, documents: DOCUMENTS });
+
+  const results = await collection.query({
+    queryTexts: ["test"],
+    nResults: 3,
+    whereDocument: { $contains: "This is a test" }
+  });
+
+  expect(results).toBeDefined();
+  expect(results).toBeInstanceOf(Object);
+  expect(results.ids.length).toBe(1);
+  expect(["test1"]).toEqual(expect.arrayContaining(results.ids[0]));
+  expect(["test2"]).not.toEqual(expect.arrayContaining(results.ids[0]));
+  expect(["This is a test"]).toEqual(
+    expect.arrayContaining(results.documents[0])
+  );
+})
```

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/update.collection.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/test/upsert.collections.test.ts` & `chromadb-client-0.3.28.dev0/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/js/yarn.lock` & `chromadb-client-0.3.28.dev0/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/python/README.md` & `chromadb-client-0.3.28.dev0/clients/python/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
 client = chromadb.Client(Settings(chroma_api_impl="rest",
                                   chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+                                  chroma_server_http_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
 you can do the following: ```python import chromadb from chromadb.config import
 Settings # Example setup of the client to connect to your chroma server client
 = chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_port=8000)) collection =
+chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
 client.create_collection("all-my-documents") collection.add( documents=["This
 is document1", "This is document2"], metadatas=[{"source": "notion"},
 {"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
 for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
 collection.query( query_texts=["This is a query document"], n_results=2, #
 where={"metadata_field": "is_equal_to_this"}, # optional filter #
 where_document={"$contains":"search_string"} # optional filter ) ``` ## License
```

### Comparing `chromadb-client-0.3.27.dev0/clients/python/build_python_thin_client.sh` & `chromadb-client-0.3.28.dev0/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/python/integration-test.sh` & `chromadb-client-0.3.28.dev0/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/clients/python/pyproject.toml` & `chromadb-client-0.3.28.dev0/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/docker-compose.server.example.yml` & `chromadb-client-0.3.28.dev0/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/docker-compose.test.yml` & `chromadb-client-0.3.28.dev0/docker-compose.test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
       - test_index_data:/index_data
     command: uvicorn chromadb.app:app --workers 1 --host 0.0.0.0 --port 8000 --log-config log_config.yml
     environment:
       - CHROMA_DB_IMPL=clickhouse
       - CLICKHOUSE_HOST=test_clickhouse
       - CLICKHOUSE_PORT=8123
       - ANONYMIZED_TELEMETRY=False
+      - ALLOW_RESET=True
     ports:
       - ${CHROMA_PORT}:8000
     depends_on:
       - test_clickhouse
     networks:
       - test_net
```

### Comparing `chromadb-client-0.3.27.dev0/docker-compose.yml` & `chromadb-client-0.3.28.dev0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/examples/alternative_embeddings.ipynb` & `chromadb-client-0.3.28.dev0/examples/basic_functionality/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/README.md` & `chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-client-0.3.28.dev0/examples/deployments/google-cloud-compute/startup.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #! /bin/bash
 
+cd ~
+
 apt-get update -y
 apt-get install -y ca-certificates curl gnupg lsb-release
 mkdir -m 0755 -p /etc/apt/keyrings
 curl -fsSL https://download.docker.com/linux/debian/gpg | gpg --dearmor -o /etc/apt/keyrings/docker.gpg
 echo \
   "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian \
   $(lsb_release -cs) stable" | tee /etc/apt/sources.list.d/docker.list > /dev/null
@@ -70,8 +72,8 @@
             <allow_experimental_lightweight_delete>1</allow_experimental_lightweight_delete>
             <mutations_sync>1</mutations_sync>
         </default>
     </profiles>
 </clickhouse>
 EOF
 
-docker compose up -d
+COMPOSE_PROJECT_NAME=chroma docker compose up -d
```

### Comparing `chromadb-client-0.3.27.dev0/examples/local_persistence.ipynb` & `chromadb-client-0.3.28.dev0/examples/basic_functionality/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/examples/where_filtering.ipynb` & `chromadb-client-0.3.28.dev0/examples/basic_functionality/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `chromadb-client-0.3.28.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.27.dev0/pyproject.toml` & `chromadb-client-0.3.28.dev0/pyproject.toml`

 * *Files identical despite different names*

