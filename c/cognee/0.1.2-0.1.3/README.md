# Comparing `tmp/cognee-0.1.2.tar.gz` & `tmp/cognee-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognee-0.1.2.tar", max compression
+gzip compressed data, was "cognee-0.1.3.tar", max compression
```

## Comparing `cognee-0.1.2.tar` & `cognee-0.1.3.tar`

### file list

```diff
@@ -1,147 +1,155 @@
--rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.2/LICENSE
--rw-r--r--   0        0        0     3439 2024-03-30 17:25:42.197086 cognee-0.1.2/README.md
--rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.2/cognee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.2/cognee/api/__init__.py
--rw-r--r--   0        0        0     3242 2024-03-30 16:41:17.062218 cognee-0.1.2/cognee/api/client.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.2/cognee/api/v1/__init__.py
--rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.2/cognee/api/v1/add/__init__.py
--rw-r--r--   0        0        0     4671 2024-03-30 13:51:31.701448 cognee-0.1.2/cognee/api/v1/add/add.py
--rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.2/cognee/api/v1/add/add_standalone.py
--rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.2/cognee/api/v1/add/remember.py
--rw-r--r--   0        0        0     7259 2024-03-29 16:53:50.083510 cognee-0.1.2/cognee/api/v1/cognify/cognify.py
--rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.2/cognee/api/v1/config/__init__.py
--rw-r--r--   0        0        0      446 2024-03-29 19:28:33.373763 cognee-0.1.2/cognee/api/v1/config/config.py
--rw-r--r--   0        0        0      598 2024-03-30 12:05:41.189310 cognee-0.1.2/cognee/api/v1/datasets/datasets.py
--rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.2/cognee/api/v1/prune/__init__.py
--rw-r--r--   0        0        0      643 2024-03-30 12:50:34.627648 cognee-0.1.2/cognee/api/v1/prune/prune.py
--rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.2/cognee/api/v1/search/__init__.py
--rw-r--r--   0        0        0     3581 2024-03-30 16:39:36.408528 cognee-0.1.2/cognee/api/v1/search/search.py
--rw-r--r--   0        0        0     5660 2024-03-29 20:13:16.651948 cognee-0.1.2/cognee/config.py
--rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.2/cognee/fetch_secret.py
--rw-r--r--   0        0        0     3315 2024-03-29 19:46:31.747251 cognee-0.1.2/cognee/infrastructure/InfrastructureConfig.py
--rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.2/cognee/infrastructure/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.2/cognee/infrastructure/data/__init__.py
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.2/cognee/infrastructure/data/models/Data.py
--rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.2/cognee/infrastructure/data/models/Dataset.py
--rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.2/cognee/infrastructure/data/models/DatasetData.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.2/cognee/infrastructure/data/models/__init__.py
--rw-r--r--   0        0        0      763 2024-03-29 12:58:54.563831 cognee-0.1.2/cognee/infrastructure/data/utils/extract_keywords.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.2/cognee/infrastructure/databases/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.2/cognee/infrastructure/databases/graph/__init__.py
--rw-r--r--   0        0        0     1128 2024-03-29 20:07:32.328042 cognee-0.1.2/cognee/infrastructure/databases/graph/get_graph_client.py
--rw-r--r--   0        0        0     2210 2024-03-13 17:10:40.344532 cognee-0.1.2/cognee/infrastructure/databases/graph/graph_db_interface.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344605 cognee-0.1.2/cognee/infrastructure/databases/graph/neo4j/__init__.py
--rw-r--r--   0        0        0      109 2024-03-13 17:10:40.344858 cognee-0.1.2/cognee/infrastructure/databases/graph/neo4j/adapter.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.2/cognee/infrastructure/databases/graph/networkx/__init__.py
--rw-r--r--   0        0        0     8493 2024-03-13 17:10:40.345060 cognee-0.1.2/cognee/infrastructure/databases/graph/networkx/adapter.py
--rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.2/cognee/infrastructure/databases/relational/DatabaseEngine.py
--rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.2/cognee/infrastructure/databases/relational/ModelBase.py
--rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.2/cognee/infrastructure/databases/relational/__init__.py
--rw-r--r--   0        0        0      725 2024-03-30 12:05:04.946747 cognee-0.1.2/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
--rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.2/cognee/infrastructure/databases/relational/relational_db_interface.py
--rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.2/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.2/cognee/infrastructure/databases/relational/sqlite/__init__.py
--rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.2/cognee/infrastructure/databases/relational/utils/__init__.py
--rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.2/cognee/infrastructure/databases/relational/utils/with_rollback.py
--rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.2/cognee/infrastructure/databases/vector/__init__.py
--rw-r--r--   0        0        0      674 2024-03-29 17:00:23.517351 cognee-0.1.2/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
--rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.2/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.347884 cognee-0.1.2/cognee/infrastructure/databases/vector/lancedb/__init__.py
--rw-r--r--   0        0        0     3310 2024-03-13 17:10:40.348274 cognee-0.1.2/cognee/infrastructure/databases/vector/lancedb/adapter.py
--rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.2/cognee/infrastructure/databases/vector/models/CollectionConfig.py
--rw-r--r--   0        0        0      227 2024-03-22 15:50:27.358090 cognee-0.1.2/cognee/infrastructure/databases/vector/models/DataPoint.py
--rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.2/cognee/infrastructure/databases/vector/models/ScoredResult.py
--rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.2/cognee/infrastructure/databases/vector/models/VectorConfig.py
--rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.2/cognee/infrastructure/databases/vector/pinecone/adapter.py
--rw-r--r--   0        0        0     6069 2024-03-29 14:27:35.243935 cognee-0.1.2/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
--rw-r--r--   0        0        0       59 2024-03-13 17:10:40.349378 cognee-0.1.2/cognee/infrastructure/databases/vector/qdrant/__init__.py
--rw-r--r--   0        0        0     2195 2024-03-29 12:58:54.565755 cognee-0.1.2/cognee/infrastructure/databases/vector/vector_db_interface.py
--rw-r--r--   0        0        0     3637 2024-03-30 12:48:44.298101 cognee-0.1.2/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
--rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.2/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
--rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.2/cognee/infrastructure/files/__init__.py
--rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.2/cognee/infrastructure/files/add_file_to_storage.py
--rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.2/cognee/infrastructure/files/remove_file_from_storage.py
--rw-r--r--   0        0        0     1418 2024-03-29 19:59:15.459545 cognee-0.1.2/cognee/infrastructure/files/storage/LocalStorage.py
--rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.2/cognee/infrastructure/files/storage/StorageManager.py
--rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.2/cognee/infrastructure/files/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.2/cognee/infrastructure/files/utils/__init__.py
--rw-r--r--   0        0        0      392 2024-03-29 13:33:11.690414 cognee-0.1.2/cognee/infrastructure/files/utils/extract_text_from_file.py
--rw-r--r--   0        0        0      835 2024-03-29 12:58:54.566704 cognee-0.1.2/cognee/infrastructure/files/utils/get_file_metadata.py
--rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.2/cognee/infrastructure/files/utils/get_file_size.py
--rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.2/cognee/infrastructure/files/utils/guess_file_type.py
--rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.2/cognee/infrastructure/files/utils/is_text_content.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.2/cognee/infrastructure/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.2/cognee/infrastructure/llm/anthropic/__init__.py
--rw-r--r--   0        0        0     1879 2024-03-30 12:39:21.599895 cognee-0.1.2/cognee/infrastructure/llm/anthropic/adapter.py
--rw-r--r--   0        0        0     4310 2024-03-29 12:58:54.567478 cognee-0.1.2/cognee/infrastructure/llm/generic_llm_api/adapter.py
--rw-r--r--   0        0        0     1299 2024-03-30 12:30:01.413157 cognee-0.1.2/cognee/infrastructure/llm/get_llm_client.py
--rw-r--r--   0        0        0     1599 2024-03-29 12:58:54.567907 cognee-0.1.2/cognee/infrastructure/llm/llm_interface.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.2/cognee/infrastructure/llm/openai/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-29 12:58:54.568258 cognee-0.1.2/cognee/infrastructure/llm/openai/adapter.py
--rw-r--r--   0        0        0     2487 2024-03-13 17:10:40.352918 cognee-0.1.2/cognee/infrastructure/llm/openai/openai_tools.py
--rw-r--r--   0        0        0     2715 2024-03-22 15:50:27.359964 cognee-0.1.2/cognee/infrastructure/llm/openai/queries.py
--rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.2/cognee/infrastructure/llm/prompts/__init__.py
--rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.2/cognee/infrastructure/llm/prompts/classify_content.txt
--rw-r--r--   0        0        0     1314 2024-03-13 17:10:40.353468 cognee-0.1.2/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
--rw-r--r--   0        0        0     2187 2024-03-13 17:10:40.353554 cognee-0.1.2/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
--rw-r--r--   0        0        0       68 2024-03-22 15:50:27.360445 cognee-0.1.2/cognee/infrastructure/llm/prompts/label_content.txt
--rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.2/cognee/infrastructure/llm/prompts/read_query_prompt.py
--rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.2/cognee/infrastructure/llm/prompts/render_prompt.py
--rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.2/cognee/infrastructure/llm/prompts/summarize_content.txt
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.2/cognee/infrastructure/pipeline/models/Operation.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353900 cognee-0.1.2/cognee/infrastructure/pipeline/models/_init_.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.2/cognee/modules/__init__.py
--rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354071 cognee-0.1.2/cognee/modules/cognify/__init__.py
--rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.2/cognee/modules/cognify/graph/__init__.py
--rw-r--r--   0        0        0     1443 2024-03-22 15:50:27.361219 cognee-0.1.2/cognee/modules/cognify/graph/add_classification_nodes.py
--rw-r--r--   0        0        0     1161 2024-03-13 17:10:40.354569 cognee-0.1.2/cognee/modules/cognify/graph/add_document_node.py
--rw-r--r--   0        0        0     1288 2024-03-22 15:50:27.361428 cognee-0.1.2/cognee/modules/cognify/graph/add_label_nodes.py
--rw-r--r--   0        0        0     7022 2024-03-29 14:10:33.422446 cognee-0.1.2/cognee/modules/cognify/graph/add_node_connections.py
--rw-r--r--   0        0        0     5638 2024-03-22 15:50:27.361998 cognee-0.1.2/cognee/modules/cognify/graph/add_propositions.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355009 cognee-0.1.2/cognee/modules/cognify/graph/add_semantic_search_connection.py
--rw-r--r--   0        0        0     1295 2024-03-22 15:50:27.362124 cognee-0.1.2/cognee/modules/cognify/graph/add_summary_nodes.py
--rw-r--r--   0        0        0     8625 2024-03-22 15:50:27.362421 cognee-0.1.2/cognee/modules/cognify/graph/create.py
--rw-r--r--   0        0        0     1006 2024-03-22 15:50:27.362656 cognee-0.1.2/cognee/modules/cognify/graph/initialize_graph.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.2/cognee/modules/cognify/llm/__init__.py
--rw-r--r--   0        0        0     2119 2024-03-29 12:58:54.568821 cognee-0.1.2/cognee/modules/cognify/llm/classify_content.py
--rw-r--r--   0        0        0      579 2024-03-22 15:50:27.363257 cognee-0.1.2/cognee/modules/cognify/llm/content_to_cog_layers.py
--rw-r--r--   0        0        0     1033 2024-03-22 15:50:27.363567 cognee-0.1.2/cognee/modules/cognify/llm/generate_graph.py
--rw-r--r--   0        0        0      614 2024-03-29 12:58:54.569126 cognee-0.1.2/cognee/modules/cognify/llm/label_content.py
--rw-r--r--   0        0        0     1215 2024-03-29 12:58:54.569332 cognee-0.1.2/cognee/modules/cognify/llm/resolve_cross_graph_references.py
--rw-r--r--   0        0        0      618 2024-03-29 12:58:54.569749 cognee-0.1.2/cognee/modules/cognify/llm/summarize_content.py
--rw-r--r--   0        0        0      784 2024-03-22 15:50:27.364528 cognee-0.1.2/cognee/modules/cognify/vector/add_propositions.py
--rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.2/cognee/modules/discovery/__init__.py
--rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.2/cognee/modules/discovery/discover_directory_datasets.py
--rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.2/cognee/modules/ingestion/__init__.py
--rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.2/cognee/modules/ingestion/add_data_to_dataset.py
--rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.2/cognee/modules/ingestion/classify.py
--rw-r--r--   0        0        0      692 2024-03-29 12:58:54.570789 cognee-0.1.2/cognee/modules/ingestion/data_types/BinaryData.py
--rw-r--r--   0        0        0      230 2024-03-29 12:58:54.571011 cognee-0.1.2/cognee/modules/ingestion/data_types/IngestionData.py
--rw-r--r--   0        0        0      511 2024-03-29 12:58:54.571210 cognee-0.1.2/cognee/modules/ingestion/data_types/TextData.py
--rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.2/cognee/modules/ingestion/data_types/__init__.py
--rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.2/cognee/modules/ingestion/exceptions.py
--rw-r--r--   0        0        0      254 2024-03-13 17:10:40.360037 cognee-0.1.2/cognee/modules/ingestion/identify.py
--rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.2/cognee/modules/ingestion/save.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.360307 cognee-0.1.2/cognee/modules/memory/__init__.py
--rw-r--r--   0        0        0       55 2024-03-13 17:10:40.361059 cognee-0.1.2/cognee/modules/memory/vector/__init__.py
--rw-r--r--   0        0        0      378 2024-03-13 17:10:40.361283 cognee-0.1.2/cognee/modules/memory/vector/create_vector_memory.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.2/cognee/modules/search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.2/cognee/modules/search/graph/__init__.py
--rw-r--r--   0        0        0      913 2024-03-22 15:50:27.364872 cognee-0.1.2/cognee/modules/search/graph/search_adjacent.py
--rw-r--r--   0        0        0      557 2024-03-22 15:50:27.365088 cognee-0.1.2/cognee/modules/search/graph/search_categories.py
--rw-r--r--   0        0        0     1010 2024-03-22 15:50:27.365311 cognee-0.1.2/cognee/modules/search/graph/search_neighbour.py
--rw-r--r--   0        0        0      544 2024-03-22 15:50:27.365587 cognee-0.1.2/cognee/modules/search/graph/search_summary.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.2/cognee/modules/search/vector/__init__.py
--rw-r--r--   0        0        0     1507 2024-03-30 16:18:14.250229 cognee-0.1.2/cognee/modules/search/vector/search_similarity.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.2/cognee/modules/users/__init__.py
--rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.2/cognee/modules/users/memory/__init__.py
--rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.2/cognee/modules/users/memory/create_information_points.py
--rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.2/cognee/modules/users/memory/is_existing_memory.py
--rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.2/cognee/modules/users/memory/register_memory_for_user.py
--rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.2/cognee/root_dir.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.2/cognee/shared/__init__.py
--rw-r--r--   0        0        0     8575 2024-03-30 12:42:21.249458 cognee-0.1.2/cognee/shared/data_models.py
--rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.2/cognee/shared/encode_uuid.py
--rw-r--r--   0        0        0     4345 2024-03-30 11:04:30.643974 cognee-0.1.2/cognee/utils.py
--rw-r--r--   0        0        0     3324 2024-03-30 17:30:48.945773 cognee-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 cognee-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3449 2024-04-21 20:11:09.838701 cognee-0.1.3/README.md
+-rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.3/cognee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.3/cognee/api/__init__.py
+-rw-r--r--   0        0        0     3242 2024-03-30 16:41:17.062218 cognee-0.1.3/cognee/api/client.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.3/cognee/api/v1/__init__.py
+-rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.3/cognee/api/v1/add/__init__.py
+-rw-r--r--   0        0        0     4642 2024-04-21 19:40:11.051001 cognee-0.1.3/cognee/api/v1/add/add.py
+-rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.3/cognee/api/v1/add/add_standalone.py
+-rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.3/cognee/api/v1/add/remember.py
+-rw-r--r--   0        0        0     6629 2024-04-20 17:06:04.931686 cognee-0.1.3/cognee/api/v1/cognify/cognify.py
+-rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.3/cognee/api/v1/config/__init__.py
+-rw-r--r--   0        0        0     2128 2024-04-20 17:06:04.932458 cognee-0.1.3/cognee/api/v1/config/config.py
+-rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.3/cognee/api/v1/datasets/datasets.py
+-rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.3/cognee/api/v1/prune/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-20 17:06:04.933673 cognee-0.1.3/cognee/api/v1/prune/prune.py
+-rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.3/cognee/api/v1/search/__init__.py
+-rw-r--r--   0        0        0     3534 2024-04-20 17:45:58.021645 cognee-0.1.3/cognee/api/v1/search/search.py
+-rw-r--r--   0        0        0     6290 2024-04-20 17:16:57.816028 cognee-0.1.3/cognee/config.py
+-rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.3/cognee/fetch_secret.py
+-rw-r--r--   0        0        0     7242 2024-04-20 17:28:06.014788 cognee-0.1.3/cognee/infrastructure/InfrastructureConfig.py
+-rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.3/cognee/infrastructure/__init__.py
+-rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.3/cognee/infrastructure/data/__init__.py
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.3/cognee/infrastructure/data/models/Data.py
+-rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.3/cognee/infrastructure/data/models/Dataset.py
+-rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.3/cognee/infrastructure/data/models/DatasetData.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.3/cognee/infrastructure/data/models/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.3/cognee/infrastructure/data/utils/extract_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.3/cognee/infrastructure/databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.3/cognee/infrastructure/databases/graph/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-20 17:13:59.861624 cognee-0.1.3/cognee/infrastructure/databases/graph/get_graph_client.py
+-rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.3/cognee/infrastructure/databases/graph/graph_db_interface.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.3/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
+-rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.3/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.3/cognee/infrastructure/databases/graph/networkx/__init__.py
+-rw-r--r--   0        0        0     5212 2024-04-20 17:06:04.936777 cognee-0.1.3/cognee/infrastructure/databases/graph/networkx/adapter.py
+-rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.3/cognee/infrastructure/databases/relational/DatabaseEngine.py
+-rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.3/cognee/infrastructure/databases/relational/ModelBase.py
+-rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.3/cognee/infrastructure/databases/relational/__init__.py
+-rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.3/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
+-rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.3/cognee/infrastructure/databases/relational/relational_db_interface.py
+-rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.3/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.3/cognee/infrastructure/databases/relational/sqlite/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.3/cognee/infrastructure/databases/relational/utils/__init__.py
+-rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.3/cognee/infrastructure/databases/relational/utils/with_rollback.py
+-rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.3/cognee/infrastructure/databases/vector/__init__.py
+-rw-r--r--   0        0        0     1410 2024-04-20 17:06:04.937392 cognee-0.1.3/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
+-rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.3/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
+-rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.3/cognee/infrastructure/databases/vector/models/CollectionConfig.py
+-rw-r--r--   0        0        0      261 2024-04-20 17:06:04.938241 cognee-0.1.3/cognee/infrastructure/databases/vector/models/DataPoint.py
+-rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.3/cognee/infrastructure/databases/vector/models/ScoredResult.py
+-rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.3/cognee/infrastructure/databases/vector/models/VectorConfig.py
+-rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.3/cognee/infrastructure/databases/vector/pinecone/adapter.py
+-rw-r--r--   0        0        0     6114 2024-04-20 17:06:04.938634 cognee-0.1.3/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
+-rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.3/cognee/infrastructure/databases/vector/qdrant/__init__.py
+-rw-r--r--   0        0        0     2195 2024-03-29 12:58:54.565755 cognee-0.1.3/cognee/infrastructure/databases/vector/vector_db_interface.py
+-rw-r--r--   0        0        0     4664 2024-04-20 17:37:59.594359 cognee-0.1.3/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
+-rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.3/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.3/cognee/infrastructure/files/__init__.py
+-rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.3/cognee/infrastructure/files/add_file_to_storage.py
+-rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.3/cognee/infrastructure/files/remove_file_from_storage.py
+-rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.3/cognee/infrastructure/files/storage/LocalStorage.py
+-rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.3/cognee/infrastructure/files/storage/StorageManager.py
+-rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.3/cognee/infrastructure/files/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.3/cognee/infrastructure/files/utils/__init__.py
+-rw-r--r--   0        0        0      392 2024-03-29 13:33:11.690414 cognee-0.1.3/cognee/infrastructure/files/utils/extract_text_from_file.py
+-rw-r--r--   0        0        0      835 2024-03-29 12:58:54.566704 cognee-0.1.3/cognee/infrastructure/files/utils/get_file_metadata.py
+-rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.3/cognee/infrastructure/files/utils/get_file_size.py
+-rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.3/cognee/infrastructure/files/utils/guess_file_type.py
+-rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.3/cognee/infrastructure/files/utils/is_text_content.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.3/cognee/infrastructure/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.3/cognee/infrastructure/llm/anthropic/__init__.py
+-rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.3/cognee/infrastructure/llm/anthropic/adapter.py
+-rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.3/cognee/infrastructure/llm/generic_llm_api/adapter.py
+-rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.3/cognee/infrastructure/llm/get_llm_client.py
+-rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.3/cognee/infrastructure/llm/llm_interface.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.3/cognee/infrastructure/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.3/cognee/infrastructure/llm/openai/adapter.py
+-rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.3/cognee/infrastructure/llm/prompts/__init__.py
+-rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.3/cognee/infrastructure/llm/prompts/classify_content.txt
+-rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
+-rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
+-rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.3/cognee/infrastructure/llm/prompts/read_query_prompt.py
+-rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.3/cognee/infrastructure/llm/prompts/render_prompt.py
+-rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.3/cognee/infrastructure/llm/prompts/summarize_content.txt
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.3/cognee/infrastructure/pipeline/models/Operation.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353900 cognee-0.1.3/cognee/infrastructure/pipeline/models/_init_.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.3/cognee/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.3/cognee/modules/cognify/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.3/cognee/modules/cognify/dataset.py
+-rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.3/cognee/modules/cognify/evaluate.py
+-rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.3/cognee/modules/cognify/graph/__init__.py
+-rw-r--r--   0        0        0     1186 2024-04-20 17:06:04.943347 cognee-0.1.3/cognee/modules/cognify/graph/add_classification_nodes.py
+-rw-r--r--   0        0        0     4928 2024-04-21 19:46:17.929629 cognee-0.1.3/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
+-rw-r--r--   0        0        0      915 2024-04-20 17:06:04.943871 cognee-0.1.3/cognee/modules/cognify/graph/add_cognitive_layers.py
+-rw-r--r--   0        0        0     1265 2024-04-20 17:06:04.944165 cognee-0.1.3/cognee/modules/cognify/graph/add_data_chunks.py
+-rw-r--r--   0        0        0      797 2024-04-20 17:06:04.944492 cognee-0.1.3/cognee/modules/cognify/graph/add_document_node.py
+-rw-r--r--   0        0        0     1948 2024-04-20 17:06:04.944822 cognee-0.1.3/cognee/modules/cognify/graph/add_label_nodes.py
+-rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.3/cognee/modules/cognify/graph/add_node_connections.py
+-rw-r--r--   0        0        0      798 2024-04-20 17:06:04.945404 cognee-0.1.3/cognee/modules/cognify/graph/add_summary_nodes.py
+-rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.3/cognee/modules/cognify/graph/create.py
+-rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.3/cognee/modules/cognify/graph/initialize_graph.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.3/cognee/modules/cognify/llm/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.3/cognee/modules/cognify/llm/resolve_cross_graph_references.py
+-rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.3/cognee/modules/cognify/test.py
+-rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.3/cognee/modules/cognify/train.py
+-rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.3/cognee/modules/data/extraction/extract_categories.py
+-rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.3/cognee/modules/data/extraction/extract_cognitive_layers.py
+-rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.3/cognee/modules/data/extraction/extract_summary.py
+-rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
+-rw-r--r--   0        0        0     1102 2024-04-20 17:06:04.948874 cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
+-rw-r--r--   0        0        0     4726 2024-04-20 18:13:47.472889 cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
+-rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.3/cognee/modules/data/get_cognitive_layers.py
+-rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.3/cognee/modules/data/get_content_categories.py
+-rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.3/cognee/modules/data/get_content_summary.py
+-rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.3/cognee/modules/data/get_layer_graphs.py
+-rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.3/cognee/modules/discovery/__init__.py
+-rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.3/cognee/modules/discovery/discover_directory_datasets.py
+-rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.3/cognee/modules/ingestion/__init__.py
+-rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.3/cognee/modules/ingestion/add_data_to_dataset.py
+-rw-r--r--   0        0        0     8775 2024-04-20 17:06:04.950504 cognee-0.1.3/cognee/modules/ingestion/chunkers.py
+-rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.3/cognee/modules/ingestion/classify.py
+-rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.3/cognee/modules/ingestion/data_types/BinaryData.py
+-rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.3/cognee/modules/ingestion/data_types/IngestionData.py
+-rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.3/cognee/modules/ingestion/data_types/TextData.py
+-rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.3/cognee/modules/ingestion/data_types/__init__.py
+-rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.3/cognee/modules/ingestion/exceptions.py
+-rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.3/cognee/modules/ingestion/identify.py
+-rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.3/cognee/modules/ingestion/save.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.360307 cognee-0.1.3/cognee/modules/memory/__init__.py
+-rw-r--r--   0        0        0       55 2024-03-13 17:10:40.361059 cognee-0.1.3/cognee/modules/memory/vector/__init__.py
+-rw-r--r--   0        0        0      378 2024-03-13 17:10:40.361283 cognee-0.1.3/cognee/modules/memory/vector/create_vector_memory.py
+-rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.3/cognee/modules/search/CogneeSearch.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.3/cognee/modules/search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.3/cognee/modules/search/graph/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.3/cognee/modules/search/graph/search_adjacent.py
+-rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.3/cognee/modules/search/graph/search_categories.py
+-rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.3/cognee/modules/search/graph/search_neighbour.py
+-rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.3/cognee/modules/search/graph/search_summary.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.3/cognee/modules/search/vector/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-20 17:45:36.721313 cognee-0.1.3/cognee/modules/search/vector/search_similarity.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.3/cognee/modules/users/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.3/cognee/modules/users/memory/__init__.py
+-rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.3/cognee/modules/users/memory/create_information_points.py
+-rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.3/cognee/modules/users/memory/is_existing_memory.py
+-rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.3/cognee/modules/users/memory/register_memory_for_user.py
+-rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.3/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
+-rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.3/cognee/root_dir.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.3/cognee/shared/__init__.py
+-rw-r--r--   0        0        0     8681 2024-04-20 17:06:04.953716 cognee-0.1.3/cognee/shared/data_models.py
+-rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.3/cognee/shared/encode_uuid.py
+-rw-r--r--   0        0        0     5635 2024-04-20 17:06:04.953913 cognee-0.1.3/cognee/tests/test_library.py
+-rw-r--r--   0        0        0     8721 2024-04-21 19:46:01.389886 cognee-0.1.3/cognee/utils.py
+-rw-r--r--   0        0        0     3472 2024-04-21 20:10:30.296961 cognee-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6882 1970-01-01 00:00:00.000000 cognee-0.1.3/PKG-INFO
```

### Comparing `cognee-0.1.2/LICENSE` & `cognee-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/README.md` & `cognee-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # cognee
 
-Make data processing for LLMs easy
+Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and vector retrieval
 
 
 <p>
   <a href="https://cognee.ai" target="_blank">
-    <img src="assets/cognee-logo.png" width="160px" alt="Cognee logo" />
+    <img src="https://raw.githubusercontent.com/topoteretes/cognee/main/assets/cognee-logo.png" width="160px" alt="Cognee logo" />
   </a>
 </p>
 
+
 <p>
-  <i>Open-source framework for creating knowledge graphs and data models for LLMs.</i>
+  <i>Open-source framework for creating self-improving deterministic outputs for LLMs.</i>
 </p>
 
 <p>
   <a href="https://github.com/topoteretes/cognee/fork">
     <img src="https://img.shields.io/github/forks/topoteretes/cognee?style=for-the-badge" alt="cognee forks"/>
   </a>
   <a href="https://github.com/topoteretes/cognee/stargazers">
@@ -24,21 +25,17 @@
     <img src="https://img.shields.io/github/issues-pr/topoteretes/cognee?style=for-the-badge" alt="cognee pull-requests"/>
   </a>
   <a href="https://github.com/topoteretes/cognee/releases">
     <img src="https://img.shields.io/github/release/topoteretes/cognee?&label=Latest&style=for-the-badge" alt="cognee releases" />
   </a>
 </p>
 
+![Cognee Demo](assets/cognee_demo.gif)
 
-## 🚀 It's alive
-
-<p>
-Try it yourself on Whatsapp with one of our <a href="https://keepi.ai" target="_blank">partners</a> by typing `/save {content you want to save}` followed by `/query {knowledge you saved previously}`
-For more info here are the <a href="https://topoteretes.github.io/cognee">docs</a>
-</p>
+For more details, have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
 
 
 ## 📦 Installation
 
 With pip:
 
 ```bash
@@ -60,14 +57,15 @@
 
 os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
 os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY"
 
 os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
 
 ```
+You can also use Ollama or Anyscale as your LLM provider. For more info on local models check our [docs](https://topoteretes.github.io/cognee)
 
 ### Run
 
 ```
 import cognee
 
 text = """Natural language processing (NLP) is an interdisciplinary
@@ -107,23 +105,29 @@
 Read more [here](docs/index.md#run).
 
 ## Demo
 
 Check out our demo notebook [here](https://github.com/topoteretes/cognee/blob/main/notebooks/cognee%20-%20Get%20Started.ipynb)
 
 
-## Architecture
 
-[<img src="https://i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg" width="100%">](https://youtu.be/-ARUfIzhzC4 "Learn about cognee: 55")
+[<img src="https://i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg" width="100%">](https://www.youtube.com/watch?v=BDFt4xVPmro "Learn about cognee: 55")
+
+
 
 
-### How Cognee Enhances Your Contextual Memory
 
-Our framework for the OpenAI, Graph (Neo4j) and Vector (Weaviate) databases introduces three key enhancements:
+## How it works
+
+
 
-- Query Classifiers: Navigate information graph using Pydantic OpenAI classifiers.
-- Document Topology: Structure and store documents in public and private domains.
-- Personalized Context: Provide a context object to the LLM for a better response.
 
 
 ![Image](assets/architecture.png)
 
+
+## 🚀 It's alive
+
+<p>
+Try it yourself on Whatsapp with one of our <a href="https://keepi.ai" target="_blank">partners</a> by typing `/save {content you want to save}` followed by `/query {knowledge you saved previously}`
+For more info here are the <a href="https://topoteretes.github.io/cognee">docs</a>
+</p>
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-# cognee Make data processing for LLMs easy
+# cognee Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and
+vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
-Open-source framework for creating knowledge graphs and data models for LLMs.
+Open-source framework for creating self-improving deterministic outputs for
+LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
-## ð It's alive
-Try it yourself on Whatsapp with one of our _p_a_r_t_n_e_r_s by typing `/save {content
-you want to save}` followed by `/query {knowledge you saved previously}` For
-more info here are the _d_o_c_s
-## ð¦ Installation With pip: ```bash pip install "cognee[weaviate]" ``` With
-poetry: ```bash poetry add "cognee[weaviate]" ``` ## ð» Usage ### Setup ```
-import os os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ
-["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] =
-"YOUR_OPENAI_API_KEY" ``` ### Run ``` import cognee text = """Natural language
-processing (NLP) is an interdisciplinary subfield of computer science and
-information retrieval""" cognee.add(text) # Add a new piece of information
-cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
-cognee.search("SIMILARITY", "computer science") # Query cognee for the
-knowledge for result_text in search_results[0]: print(result_text) ``` Add
-alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
+![Cognee Demo](assets/cognee_demo.gif) For more details, have a look at our
+_d_o_c_u_m_e_n_t_a_t_i_o_n ## ð¦ Installation With pip: ```bash pip install "cognee
+[weaviate]" ``` With poetry: ```bash poetry add "cognee[weaviate]" ``` ## ð»
+Usage ### Setup ``` import os os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
+os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY" os.environ
+["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY" ``` You can also use Ollama or
+Anyscale as your LLM provider. For more info on local models check our [docs]
+(https://topoteretes.github.io/cognee) ### Run ``` import cognee text =
+"""Natural language processing (NLP) is an interdisciplinary subfield of
+computer science and information retrieval""" cognee.add(text) # Add a new
+piece of information cognee.cognify() # Use LLMs and cognee to create knowledge
+search_results = cognee.search("SIMILARITY", "computer science") # Query cognee
+for the knowledge for result_text in search_results[0]: print(result_text) ```
+Add alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
 dataset_name) ``` Or ``` cognee.add("data://{absolute_path_to_directory}",
 dataset_name) # This is useful if you have a directory with files organized in
 subdirectories. # You can target which directory to add by providing
 dataset_name. # Example: # root # / \ # reports bills # / \ # 2024 2023 # #
 cognee.add("data://{absolute_path_to_root}", "reports.2024") # This will add
 just directory 2024 under reports. ``` Read more [here](docs/index.md#run). ##
 Demo Check out our demo notebook [here](https://github.com/topoteretes/cognee/
-blob/main/notebooks/cognee%20-%20Get%20Started.ipynb) ## Architecture [[https:/
-/i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg]](https://youtu.be/-ARUfIzhzC4
-"Learn about cognee: 55") ### How Cognee Enhances Your Contextual Memory Our
-framework for the OpenAI, Graph (Neo4j) and Vector (Weaviate) databases
-introduces three key enhancements: - Query Classifiers: Navigate information
-graph using Pydantic OpenAI classifiers. - Document Topology: Structure and
-store documents in public and private domains. - Personalized Context: Provide
-a context object to the LLM for a better response. ![Image](assets/
-architecture.png)
+blob/main/notebooks/cognee%20-%20Get%20Started.ipynb) [[https://i3.ytimg.com/
+vi/-ARUfIzhzC4/maxresdefault.jpg]](https://www.youtube.com/watch?v=BDFt4xVPmro
+"Learn about cognee: 55") ## How it works ![Image](assets/architecture.png) ##
+ð It's alive
+Try it yourself on Whatsapp with one of our _p_a_r_t_n_e_r_s by typing `/save {content
+you want to save}` followed by `/query {knowledge you saved previously}` For
+more info here are the _d_o_c_s
```

### Comparing `cognee-0.1.2/cognee/api/client.py` & `cognee-0.1.3/cognee/api/client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/api/v1/add/add.py` & `cognee-0.1.3/cognee/api/v1/add/add.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import List, Union
 from os import path
 import asyncio
 import dlt
 import duckdb
 import cognee.modules.ingestion as ingestion
 from cognee.infrastructure import infrastructure_config
-from cognee.infrastructure.files import get_file_metadata
 from cognee.infrastructure.files.storage import LocalStorage
 from cognee.modules.discovery import discover_directory_datasets
 
 async def add(data_path: Union[str, List[str]], dataset_name: str = None):
     if isinstance(data_path, str):
         # data_path is a data directory path
         if "data://" in data_path:
             return await add_data_directory(data_path.replace("data://", ""), dataset_name)
         # data_path is a file path
         if "file://" in data_path:
             return await add([data_path], dataset_name)
         # data_path is a text
         else:
-            return await add_text(data_path, dataset_name)
+            file_path = save_text_to_file(data_path, dataset_name)
+            return await add([file_path], dataset_name)
 
     # data_path is a list of file paths or texts
     file_paths = []
     texts = []
 
     for file_path in data_path:
         if file_path.startswith("/") or file_path.startswith("file://"):
             file_paths.append(file_path)
         else:
             texts.append(file_path)
 
     awaitables = []
 
-    if len(file_paths) > 0:
-        awaitables.append(add_files(file_paths, dataset_name))
-
     if len(texts) > 0:
         for text in texts:
-            awaitables.append(add_text(text, dataset_name))
+            file_paths.append(save_text_to_file(text, dataset_name))
+
+    if len(file_paths) > 0:
+        awaitables.append(add_files(file_paths, dataset_name))
 
     return await asyncio.gather(*awaitables)
 
 async def add_files(file_paths: List[str], dataset_name: str):
     infra_config = infrastructure_config.get_config()
     data_directory_path = infra_config["data_root_directory"]
 
@@ -80,15 +80,15 @@
     def data_resources(file_paths: str):
         for file_path in file_paths:
             with open(file_path.replace("file://", ""), mode = "rb") as file:
                 classified_data = ingestion.classify(file)
 
                 data_id = ingestion.identify(classified_data)
 
-                file_metadata = get_file_metadata(classified_data.get_data())
+                file_metadata = classified_data.get_metadata()
 
                 yield {
                     "id": data_id,
                     "name": file_metadata["name"],
                     "file_path": file_metadata["file_path"],
                     "extension": file_metadata["extension"],
                     "mime_type": file_metadata["mime_type"],
@@ -111,20 +111,20 @@
 
     for key in datasets.keys():
         if dataset_name is None or key.startswith(dataset_name):
             results.append(add(datasets[key], dataset_name = key))
 
     return await asyncio.gather(*results)
 
-async def add_text(text: str, dataset_name: str):
+def save_text_to_file(text: str, dataset_name: str):
     data_directory_path = infrastructure_config.get_config()["data_root_directory"]
 
     classified_data = ingestion.classify(text)
     data_id = ingestion.identify(classified_data)
 
     storage_path = data_directory_path + "/" + dataset_name.replace(".", "/")
     LocalStorage.ensure_directory_exists(storage_path)
 
-    text_file_name = str(data_id) + ".txt"
+    text_file_name = data_id + ".txt"
     LocalStorage(storage_path).store(text_file_name, classified_data.get_data())
 
-    return await add(["file://" + storage_path + "/" + text_file_name], dataset_name)
+    return "file://" + storage_path + "/" + text_file_name
```

### Comparing `cognee-0.1.2/cognee/api/v1/add/add_standalone.py` & `cognee-0.1.3/cognee/api/v1/add/add_standalone.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/api/v1/add/remember.py` & `cognee-0.1.3/cognee/api/v1/add/remember.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/api/v1/cognify/cognify.py` & `cognee-0.1.3/cognee/api/v1/cognify/cognify.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import asyncio
-# import logging
 from typing import List, Union
+import logging
 import instructor
 from openai import OpenAI
+from cognee.modules.cognify.graph.add_data_chunks import add_data_chunks
+from cognee.modules.cognify.graph.add_document_node import add_document_node
 from cognee.modules.cognify.graph.add_classification_nodes import add_classification_nodes
-from cognee.modules.cognify.llm.label_content import label_content
-from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
-from cognee.modules.cognify.llm.summarize_content import summarize_content
+from cognee.modules.cognify.graph.add_cognitive_layer_graphs import add_cognitive_layer_graphs
 from cognee.modules.cognify.graph.add_summary_nodes import add_summary_nodes
-from cognee.modules.cognify.graph.add_node_connections import group_nodes_by_layer, graph_ready_output, \
-    connect_nodes_in_graph, extract_node_descriptions
-from cognee.modules.cognify.graph.add_propositions import append_to_graph
+from cognee.modules.cognify.graph.add_node_connections import group_nodes_by_layer, \
+    graph_ready_output, connect_nodes_in_graph
 from cognee.modules.cognify.llm.resolve_cross_graph_references import resolve_cross_graph_references
-from cognee.modules.cognify.vector.add_propositions import add_propositions
 
 from cognee.config import Config
-from cognee.modules.cognify.llm.classify_content import classify_into_categories
-from cognee.modules.cognify.llm.content_to_cog_layers import content_to_cog_layers
-from cognee.modules.cognify.llm.generate_graph import generate_graph
-from cognee.shared.data_models import DefaultContentPrediction, KnowledgeGraph, DefaultCognitiveLayer, \
-    SummarizedContent, LabeledContent
+
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
-from cognee.shared.data_models import GraphDBType
-from cognee.modules.cognify.graph.add_document_node import add_document_node
-from cognee.modules.cognify.graph.initialize_graph import initialize_graph
-from cognee.infrastructure.files.utils.guess_file_type import guess_file_type
+from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
+from cognee.modules.cognify.graph.add_cognitive_layers import add_cognitive_layers
+# from cognee.modules.cognify.graph.initialize_graph import initialize_graph
+from cognee.infrastructure.files.utils.guess_file_type import guess_file_type, FileTypeException
 from cognee.infrastructure.files.utils.extract_text_from_file import extract_text_from_file
 from cognee.infrastructure import infrastructure_config
+from cognee.modules.data.get_content_categories import get_content_categories
+from cognee.modules.data.get_content_summary import get_content_summary
+from cognee.modules.data.get_cognitive_layers import get_cognitive_layers
+from cognee.modules.data.get_layer_graphs import get_layer_graphs
 
 config = Config()
 config.load()
 
 aclient = instructor.patch(OpenAI())
 
 USER_ID = "default_user"
 
-async def cognify(datasets: Union[str, List[str]] = None, graph_data_model: object = None):
+logger = logging.getLogger(__name__)
+
+async def cognify(datasets: Union[str, List[str]] = None):
     """This function is responsible for the cognitive processing of the content."""
 
     db_engine = infrastructure_config.get_config()["database_engine"]
 
     if datasets is None or len(datasets) == 0:
         datasets = db_engine.get_datasets()
 
@@ -52,153 +52,112 @@
 
         graphs = await asyncio.gather(*awaitables)
         return graphs[0]
 
     # datasets is a dataset name string
     added_datasets = db_engine.get_datasets()
 
-    files_metadata = []
+    dataset_files = []
     dataset_name = datasets.replace(".", "_").replace(" ", "_")
 
     for added_dataset in added_datasets:
         if dataset_name in added_dataset:
-            files_metadata.extend(db_engine.get_files_metadata(added_dataset))
+            dataset_files.append((added_dataset, db_engine.get_files_metadata(added_dataset)))
 
     awaitables = []
 
-    await initialize_graph(USER_ID, graph_data_model)
-
-    for file_metadata in files_metadata:
-        with open(file_metadata["file_path"], "rb") as file:
-            file_type = guess_file_type(file)
-            text = extract_text_from_file(file, file_type)
-
-            awaitables.append(process_text(text, file_metadata))
-
-    graphs = await asyncio.gather(*awaitables)
-
-    return graphs[0]
-
-async def process_text(input_text: str, file_metadata: dict):
-    print(f"Processing document ({file_metadata['id']})")
-
-    classified_categories = []
+    graph_db_type = infrastructure_config.get_config()["graph_engine"]
 
-    try:
-        # Classify the content into categories
-        classified_categories = await classify_into_categories(
-            input_text,
-            "classify_content.txt",
-            DefaultContentPrediction
-        )
-        file_metadata["categories"] = list(map(lambda category: category["layer_name"], classified_categories))
-    except Exception as e:
-        print(e)
-        raise e
-
-    try:
-        # Classify the content into categories
-        content_summary = await summarize_content(
-            input_text,
-            "summarize_content.txt",
-            SummarizedContent
-        )
-        file_metadata["summary"] = content_summary["summary"]
-    except Exception as e:
-        print(e)
-        raise e
-
-    try:
-        # Classify the content into categories
-        content_labels = await label_content(
-            input_text,
-            "label_content.txt",
-            LabeledContent
-        )
-        file_metadata["content_labels"] = content_labels["content_labels"]
-    except Exception as e:
-        print(e)
-        raise e
-
-    await add_document_node(f"DefaultGraphModel:{USER_ID}", file_metadata)
-    print(f"Document ({file_metadata['id']}) categorized: {file_metadata['categories']}")
-
-    cognitive_layers = await content_to_cog_layers(
-        classified_categories[0],
-        response_model = DefaultCognitiveLayer
-    )
-
-    cognitive_layers = [layer_subgroup.name for layer_subgroup in cognitive_layers.cognitive_layers]
-
-    async def generate_graph_per_layer(text_input: str, layers: List[str], response_model: KnowledgeGraph = KnowledgeGraph):
-        generate_graphs_awaitables = [generate_graph(text_input, "generate_graph_prompt.txt", {"layer": layer}, response_model) for layer in
-                layers]
+    graph_client = await get_graph_client(graph_db_type)
 
-        return await asyncio.gather(*generate_graphs_awaitables)
+    # await initialize_graph(USER_ID, graph_data_model, graph_client)
 
-    # Run the async function for each set of cognitive layers
-    layer_graphs = await generate_graph_per_layer(input_text, cognitive_layers)
+    data_chunks = {}
 
-    print(f"Document ({file_metadata['id']}) layer graphs created")
+    for (dataset_name, files) in dataset_files:
+        for file_metadata in files[:3]:
+            with open(file_metadata["file_path"], "rb") as file:
+                try:
+                    file_type = guess_file_type(file)
+                    text = extract_text_from_file(file, file_type)
 
-    await add_classification_nodes(f"DOCUMENT:{file_metadata['id']}", classified_categories[0])
+                    if dataset_name not in data_chunks:
+                        data_chunks[dataset_name] = []
 
-    await add_summary_nodes(f"DOCUMENT:{file_metadata['id']}", {"summary": file_metadata["summary"]})
+                    data_chunks[dataset_name].append(dict(text = text, file_metadata = file_metadata))
+                except FileTypeException:
+                    logger.warning("File (%s) has an unknown file type. We are skipping it.", file_metadata["id"])
 
-    await add_label_nodes(f"DOCUMENT:{file_metadata['id']}", {"content_labels": file_metadata["content_labels"]})
+    added_chunks: list[tuple[str, str, dict]] = await add_data_chunks(data_chunks)
 
-    await append_to_graph(layer_graphs, classified_categories[0])
-
-    print(f"Document ({file_metadata['id']}) layers connected")
-
-    print("Document categories, summaries and metadata are: ", str(classified_categories))
+    await asyncio.gather(
+        *[process_text(chunk["collection"], chunk["id"], chunk["text"], chunk["file_metadata"]) for chunk in added_chunks]
+    )
 
-    print("Document metadata is: ", str(file_metadata))
+    return graph_client.graph
 
-    graph_client = get_graph_client(GraphDBType.NETWORKX)
+async def process_text(chunk_collection: str, chunk_id: str, input_text: str, file_metadata: dict):
+    print(f"Processing document ({file_metadata['id']}).")
 
-    await graph_client.load_graph_from_file()
+    graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
 
-    graph = graph_client.graph
+    document_id = await add_document_node(
+        graph_client,
+        parent_node_id = f"DefaultGraphModel__{USER_ID}", #make a param of defaultgraph model to make sure when user passes his stuff, it doesn't break pipeline
+        document_metadata = file_metadata,
+    )
 
-    node_descriptions = await extract_node_descriptions(graph.nodes(data = True))
+    await add_label_nodes(graph_client, document_id, chunk_id, file_metadata["keywords"].split("|"))
 
-    nodes_by_layer = await group_nodes_by_layer(node_descriptions)
+    classified_categories = await get_content_categories(input_text)
+    await add_classification_nodes(
+        graph_client,
+        parent_node_id = document_id,
+        categories = classified_categories,
+    )
 
-    unique_layers = nodes_by_layer.keys()
+    print(f"Document ({document_id}) classified.")
 
-    try:
-        vector_engine = infrastructure_config.get_config()["vector_engine"]
+    content_summary = await get_content_summary(input_text)
+    await add_summary_nodes(graph_client, document_id, content_summary)
 
-        for layer in unique_layers:
-            await vector_engine.create_collection(layer)
-    except Exception as e:
-        print(e)
+    print(f"Document ({document_id}) summarized.")
 
-    await add_propositions(nodes_by_layer)
+    cognitive_layers = await get_cognitive_layers(input_text, classified_categories)
+    cognitive_layers = (await add_cognitive_layers(graph_client, document_id, cognitive_layers))[:2]
 
-    results = await resolve_cross_graph_references(nodes_by_layer)
+    layer_graphs = await get_layer_graphs(input_text, cognitive_layers)
+    await add_cognitive_layer_graphs(graph_client, chunk_collection, chunk_id, layer_graphs)
 
-    relationships = graph_ready_output(results)
-    # print(relationships)
-    await graph_client.load_graph_from_file()
+    if infrastructure_config.get_config()["connect_documents"] is True:
+        db_engine = infrastructure_config.get_config()["database_engine"]
+        relevant_documents_to_connect = db_engine.fetch_cognify_data(excluded_document_id = file_metadata["id"])
 
-    graph = graph_client.graph
+        print("Relevant documents to connect are: ", relevant_documents_to_connect)
 
-    connect_nodes_in_graph(graph, relationships)
+        list_of_nodes = []
 
-    print(f"Document ({file_metadata['id']}) processed")
+        relevant_documents_to_connect.append({
+            "layer_id": document_id,
+        })
 
-    return graph
+        for document in relevant_documents_to_connect:
+            node_descriptions_to_match = await graph_client.extract_node_description(document["layer_id"])
+            list_of_nodes.extend(node_descriptions_to_match)
 
+        print("List of nodes are: ", len(list_of_nodes))
 
+        nodes_by_layer = await group_nodes_by_layer(list_of_nodes)
+        print("Nodes by layer are: ", str(nodes_by_layer)[:5000])
 
-if __name__ == "__main__":
+        results = await resolve_cross_graph_references(nodes_by_layer)
+        print("Results are: ", str(results)[:3000])
 
-    async def main():
-        graph = await cognify(datasets=['izmene'])
-        from cognee.utils import render_graph
-        graph_url = await render_graph(graph)
-        print(graph_url)
+        relationships = graph_ready_output(results)
 
+        await connect_nodes_in_graph(
+            graph_client,
+            relationships,
+            score_threshold = infrastructure_config.get_config()["intra_layer_score_treshold"]
+        )
 
-    asyncio.run(main())
+        print(f"Document ({document_id}) cognified.")
```

### Comparing `cognee-0.1.2/cognee/api/v1/datasets/datasets.py` & `cognee-0.1.3/cognee/api/v1/datasets/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from cognee.modules.discovery import discover_directory_datasets
 from cognee.infrastructure import infrastructure_config
 
 class datasets():
     @staticmethod
     def list_datasets():
-        db = infrastructure_config.get_config()["database_engine"]
+        db = infrastructure_config.get_config("database_engine")
         return db.get_datasets()
 
     @staticmethod
     def discover_datasets(directory_path: str):
         return list(discover_directory_datasets(directory_path).keys())
 
     @staticmethod
     def query_data(dataset_name: str):
-        db = infrastructure_config.get_config()["database_engine"]
+        db = infrastructure_config.get_config("database_engine")
         return db.get_files_metadata(dataset_name)
```

### Comparing `cognee-0.1.2/cognee/api/v1/search/search.py` & `cognee-0.1.3/cognee/api/v1/search/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Dict, Any, Callable, List
 from pydantic import BaseModel, field_validator
 from cognee.modules.search.graph.search_adjacent import search_adjacent
 from cognee.modules.search.vector.search_similarity import search_similarity
 from cognee.modules.search.graph.search_categories import search_categories
 from cognee.modules.search.graph.search_neighbour import search_neighbour
 from cognee.modules.search.graph.search_summary import search_summary
-from cognee.shared.data_models import GraphDBType
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
+from cognee.infrastructure import infrastructure_config
 
 class SearchType(Enum):
     ADJACENT = 'ADJACENT'
     SIMILARITY = 'SIMILARITY'
     CATEGORIES = 'CATEGORIES'
     NEIGHBOR = 'NEIGHBOR'
     SUMMARY = 'SUMMARY'
@@ -38,16 +38,15 @@
 
 async def search(search_type: str, params: Dict[str, Any]) -> List:
     search_params = SearchParameters(search_type = search_type, params = params)
     return await specific_search([search_params])
 
 
 async def specific_search(query_params: List[SearchParameters]) -> List:
-    graph_client = get_graph_client(GraphDBType.NETWORKX)
-    await graph_client.load_graph_from_file()
+    graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
     graph = graph_client.graph
 
     search_functions: Dict[SearchType, Callable] = {
         SearchType.ADJACENT: search_adjacent,
         SearchType.SIMILARITY: search_similarity,
         SearchType.CATEGORIES: search_categories,
         SearchType.NEIGHBOR: search_neighbour,
@@ -57,16 +56,15 @@
     results = []
     search_tasks = []
 
     for search_param in query_params:
         search_func = search_functions.get(search_param.search_type)
         if search_func:
             # Schedule the coroutine for execution and store the task
-            full_params = {**search_param.params, 'graph': graph}
-            task = search_func(**full_params)
+            task = search_func(**search_param.params, graph = graph)
             search_tasks.append(task)
 
     # Use asyncio.gather to run all scheduled tasks concurrently
     search_results = await asyncio.gather(*search_tasks)
 
     # Update the results set with the results from all tasks
     results.extend(search_results)
```

### Comparing `cognee-0.1.2/cognee/config.py` & `cognee-0.1.3/cognee/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,63 +34,68 @@
 
     vectordb: str = os.getenv("VECTORDB", "weaviate")
 
     qdrant_path: str = os.getenv("QDRANT_PATH")
     qdrant_url: str = os.getenv("QDRANT_URL")
     qdrant_api_key: str = os.getenv("QDRANT_API_KEY")
 
-    db_path = str = os.getenv("COGNEE_DB_PATH", "cognee")
+    db_path = str = os.getenv("COGNEE_DB_PATH", "databases")
     db_name: str = os.getenv("DB_NAME", "cognee.db")
     db_host: str = os.getenv("DB_HOST", "localhost")
     db_port: str = os.getenv("DB_PORT", "5432")
     db_user: str = os.getenv("DB_USER", "cognee")
     db_password: str = os.getenv("DB_PASSWORD", "cognee")
 
     sqlalchemy_logging: bool = os.getenv("SQLALCHEMY_LOGGING", True)
 
     graph_filename = os.getenv("GRAPH_NAME", "cognee_graph.pkl")
 
     # Model parameters
-    llm_provider: str = "openai" #openai, or custom or ollama
-    custom_model: str = "mistralai/Mixtral-8x7B-Instruct-v0.1"
-    custom_endpoint: str = "https://api.endpoints.anyscale.com/v1" # pass claude endpoint
-    custom_key: Optional[str] = os.getenv("ANYSCALE_API_KEY")
-    ollama_endpoint: str = "http://localhost:11434/v1"
+    llm_provider: str = os.getenv("LLM_PROVIDER","openai") #openai, or custom or ollama
+    custom_model: str = os.getenv("CUSTOM_LLM_MODEL", "mistralai/Mixtral-8x7B-Instruct-v0.1") #"mistralai/Mixtral-8x7B-Instruct-v0.1"
+    custom_endpoint: str = os.getenv("CUSTOM_ENDPOINT", "https://api.endpoints.anyscale.com/v1") #"https://api.endpoints.anyscale.com/v1" # pass claude endpoint
+    custom_key: Optional[str] = os.getenv("CUSTOM_LLM_API_KEY")
+    ollama_endpoint: str = os.getenv("CUSTOM_OLLAMA_ENDPOINT", "http://localhost:11434/v1") #"http://localhost:11434/v1"
     ollama_key: Optional[str] = "ollama"
-    ollama_model: str = "mistral:instruct"
-    model: str = "gpt-4-1106-preview"
-    # model: str = "gpt-3.5-turbo"
+    ollama_model: str = os.getenv("CUSTOM_OLLAMA_MODEL", "mistral:instruct") #"mistral:instruct"
+    openai_model: str = os.getenv("OPENAI_MODEL", "gpt-4-1106-preview" ) #"gpt-4-1106-preview"
     model_endpoint: str = "openai"
     openai_key: Optional[str] = os.getenv("OPENAI_API_KEY")
     openai_temperature: float = float(os.getenv("OPENAI_TEMPERATURE", 0.0))
+    openai_embedding_model = "text-embedding-3-large"
+    openai_embedding_dimensions = 3072
 
     graphistry_username = os.getenv("GRAPHISTRY_USERNAME")
     graphistry_password = os.getenv("GRAPHISTRY_PASSWORD")
 
     # Embedding parameters
     embedding_model: str = "BAAI/bge-large-en-v1.5"
     embedding_dimensions: int = 1024
+    connect_documents: bool = False
 
     # Database parameters
+    graph_database_provider: str = os.getenv("GRAPH_DB_PROVIDER", "NETWORKX")
+
     if (
         os.getenv("ENV") == "prod"
         or os.getenv("ENV") == "dev"
         or os.getenv("AWS_ENV") == "dev"
         or os.getenv("AWS_ENV") == "prd"
     ):
         load_dotenv()
         logging.info("graph_db_url: %s", os.getenv("GRAPH_DB_URL_PROD"))
         graph_database_url: str = os.getenv("GRAPH_DB_URL_PROD")
         graph_database_username: str = os.getenv("GRAPH_DB_USER")
         graph_database_password: str = os.getenv("GRAPH_DB_PW")
     else:
-        logging.info("graph_db_urlvvv: %s", os.getenv("GRAPH_DB_URL"))
+        logging.info("graph_db_url: %s", os.getenv("GRAPH_DB_URL"))
         graph_database_url: str = os.getenv("GRAPH_DB_URL")
         graph_database_username: str = os.getenv("GRAPH_DB_USER")
         graph_database_password: str = os.getenv("GRAPH_DB_PW")
+
     weaviate_url: str = os.getenv("WEAVIATE_URL")
     weaviate_api_key: str = os.getenv("WEAVIATE_API_KEY")
 
     if (
         os.getenv("ENV") == "prod"
         or os.getenv("ENV") == "dev"
         or os.getenv("AWS_ENV") == "dev"
@@ -100,14 +105,17 @@
 
         db_host: str = os.getenv("POSTGRES_HOST")
         logging.info("db_host: %s", db_host)
         db_user: str = os.getenv("POSTGRES_USER")
         db_password: str = os.getenv("POSTGRES_PASSWORD")
         db_name: str = os.getenv("POSTGRES_DB")
 
+    # Model parameters and configuration for interlayer scoring
+    intra_layer_score_treshold: float = 0.98
+
 
     # Client ID
     anon_clientid: Optional[str] = field(default_factory=lambda: uuid.uuid4().hex)
 
     def load(self):
         """Loads the configuration from a file or environment variables."""
         config = configparser.ConfigParser()
@@ -147,8 +155,8 @@
     @classmethod
     def from_dict(cls, config_dict: Dict[str, Any]) -> "Config":
         """Creates a Config instance from a dictionary."""
         config = cls()
         for attr, value in config_dict.items():
             if hasattr(config, attr):
                 setattr(config, attr, value)
-        return config
+        return config
```

### Comparing `cognee-0.1.2/cognee/fetch_secret.py` & `cognee-0.1.3/cognee/fetch_secret.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/data/models/Data.py` & `cognee-0.1.3/cognee/infrastructure/data/models/Data.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/data/models/Dataset.py` & `cognee-0.1.3/cognee/infrastructure/data/models/Dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/data/models/DatasetData.py` & `cognee-0.1.3/cognee/infrastructure/data/models/DatasetData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/data/utils/extract_keywords.py` & `cognee-0.1.3/cognee/infrastructure/data/utils/extract_keywords.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import nltk
 from sklearn.feature_extraction.text import TfidfVectorizer
+from cognee.utils import extract_pos_tags
 
 def extract_keywords(text: str) -> list[str]:
     if len(text) == 0:
         raise ValueError("extract_keywords cannot extract keywords from empty text.")
 
-    tokens = nltk.word_tokenize(text)
-
-    tags = nltk.pos_tag(tokens)
+    tags = extract_pos_tags(text)
     nouns = [word for (word, tag) in tags if tag == "NN"]
 
     vectorizer = TfidfVectorizer()
     tfidf = vectorizer.fit_transform(nouns)
 
     top_nouns = sorted(
         vectorizer.vocabulary_,
```

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/graph/graph_db_interface.py` & `cognee-0.1.3/cognee/infrastructure/databases/vector/vector_db_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,31 @@
-from typing import List
+from typing import List, Protocol, Optional
 from abc import abstractmethod
-from typing import Protocol
-
-class GraphDBInterface(Protocol):
-
-    """ Save and Load Graphs """
-
-    @abstractmethod
-    async def graph(self):
-        raise NotImplementedError
-
-    @abstractmethod
-    async def save_graph_to_file(
-        self,
-        file_path: str = None
-    ): raise NotImplementedError
-
-    @abstractmethod
-    async def load_graph_from_file(
-        self,
-        file_path: str = None
-    ): raise NotImplementedError
-
-    @abstractmethod
-    async def delete_graph_from_file(
-        self,
-        path: str = None
-    ): raise NotImplementedError
-
-    """ CRUD operations on graph nodes """
+from .models.DataPoint import DataPoint
 
+class VectorDBInterface(Protocol):
+    """ Collections """
     @abstractmethod
-
-    async def add_node(
+    async def create_collection(
         self,
-        id: str,
-        **kwargs
+        collection_name: str
     ): raise NotImplementedError
 
-    @abstractmethod
-    async def delete_node(
-        self,
-        id: str
-    ): raise NotImplementedError
-
-
-    """ CRUD operations on graph edges """
-
-
-    @abstractmethod
-    async def add_edge(
-        self,
-        from_node: str,
-        to_node: str,
-        **kwargs
-    ): raise NotImplementedError
+    # @abstractmethod
+    # async def update_collection(
+    #     self,
+    #     collection_name: str,
+    #     collection_config: object
+    # ): raise NotImplementedError
 
+    # @abstractmethod
+    # async def delete_collection(
+    #     self,
+    #     collection_name: str
+    # ): raise NotImplementedError
 
     # @abstractmethod
     # async def create_vector_index(
     #     self,
     #     collection_name: str,
     #     vector_index_config: object
     # ): raise NotImplementedError
@@ -67,21 +33,21 @@
     # @abstractmethod
     # async def create_data_index(
     #     self,
     #     collection_name: str,
     #     vector_index_config: object
     # ): raise NotImplementedError
 
-    # """ Data points """
-    # @abstractmethod
-    # async def create_data_points(
-    #     self,
-    #     collection_name: str,
-    #     data_points: List[any]
-    # ): raise NotImplementedError
+    """ Data points """
+    @abstractmethod
+    async def create_data_points(
+        self,
+        collection_name: str,
+        data_points: List[DataPoint]
+    ): raise NotImplementedError
 
     # @abstractmethod
     # async def get_data_point(
     #     self,
     #     collection_name: str,
     #     data_point_id: str
     # ): raise NotImplementedError
@@ -96,7 +62,28 @@
 
     # @abstractmethod
     # async def delete_data_point(
     #     self,
     #     collection_name: str,
     #     data_point_id: str
     # ): raise NotImplementedError
+
+    """ Search """
+    @abstractmethod
+    async def search(
+        self,
+        collection_name: str,
+        query_text: Optional[str],
+        query_vector: Optional[List[float]],
+        limit: int,
+        with_vector: bool = False
+
+    ): raise NotImplementedError
+
+    @abstractmethod
+    async def batch_search(
+        self,
+        collection_name: str,
+        query_texts: List[str],
+        limit: int,
+        with_vectors: bool = False
+    ): raise NotImplementedError
```

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/relational/relational_db_interface.py` & `cognee-0.1.3/cognee/infrastructure/databases/relational/relational_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py` & `cognee-0.1.3/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/relational/utils/with_rollback.py` & `cognee-0.1.3/cognee/infrastructure/databases/relational/utils/with_rollback.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py` & `cognee-0.1.3/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 from typing import List
+
+import instructor
+from openai import AsyncOpenAI
+from fastembed import TextEmbedding
 from fastembed import TextEmbedding
+from openai import AsyncOpenAI
+
 from cognee.config import Config
 from cognee.root_dir import get_absolute_path
 from .EmbeddingEngine import EmbeddingEngine
 
 config = Config()
 config.load()
 
@@ -12,7 +18,25 @@
         embedding_model = TextEmbedding(model_name = config.embedding_model, cache_dir = get_absolute_path("cache/embeddings"))
         embeddings_list = list(map(lambda embedding: embedding.tolist(), embedding_model.embed(text)))
 
         return embeddings_list
 
     def get_vector_size(self) -> int:
         return config.embedding_dimensions
+
+
+class OpenAIEmbeddingEngine(EmbeddingEngine):
+    async def embed_text(self, text: List[str]) -> List[float]:
+
+        OPENAI_API_KEY = config.openai_key
+
+        aclient = instructor.patch(AsyncOpenAI())
+        text = text.replace("\n", " ")
+        response = await aclient.embeddings.create(input = text, model = config.openai_embedding_model)
+        embedding = response.data[0].embedding
+        # embeddings_list = list(map(lambda embedding: embedding.tolist(), embedding_model.embed(text)))
+        return embedding
+
+
+    def get_vector_size(self) -> int:
+        return config.openai_embedding_dimensions
+
```

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py` & `cognee-0.1.3/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import asyncio
 from typing import List, Dict, Optional
 from qdrant_client import AsyncQdrantClient, models
 from ..vector_db_interface import VectorDBInterface
 from ..models.DataPoint import DataPoint
-from ..models.CollectionConfig import CollectionConfig
 from ..embeddings.EmbeddingEngine import EmbeddingEngine
 
 # class CollectionConfig(BaseModel, extra = "forbid"):
 #     vector_config: Dict[str, models.VectorParams] = Field(..., description="Vectors configuration" )
 #     hnsw_config: Optional[models.HnswConfig] = Field(default = None, description="HNSW vector index configuration")
 #     optimizers_config: Optional[models.OptimizersConfig] = Field(default = None, description="Optimizers configuration")
 #     quantization_config: Optional[models.QuantizationConfig] = Field(default = None, description="Quantization configuration")
@@ -75,37 +73,36 @@
                 )
             }
         )
 
     async def create_data_points(self, collection_name: str, data_points: List[DataPoint]):
         client = self.get_qdrant_client()
 
-        awaitables = []
+        data_vectors = await self.embed_data([data_point.get_embeddable_data() for data_point in data_points])
 
-        data_vectors = await self.embed_data(list(map(lambda data_point: data_point.get_embeddable_data(), data_points)))
-
-        async def convert_to_qdrant_point(data_point: DataPoint):
+        def convert_to_qdrant_point(data_point: DataPoint):
             return models.PointStruct(
                 id = data_point.id,
                 payload = data_point.payload,
                 vector = {
                     "text": data_vectors[data_points.index(data_point)]
                 }
             )
 
-        for point in data_points:
-            awaitables.append(convert_to_qdrant_point(point))
-
-        points = await asyncio.gather(*awaitables)
+        points = [convert_to_qdrant_point(point) for point in data_points]
 
         return await client.upload_points(
             collection_name = collection_name,
             points = points
         )
 
+    async def retrieve(self, collection_name: str, data_id: str):
+        results = await self.get_qdrant_client().retrieve(collection_name, [data_id], with_payload = True)
+        return results[0] if len(results) > 0 else None
+
     async def search(
         self,
         collection_name: str,
         query_text: Optional[str] = None,
         query_vector: Optional[List[float]] = None,
         limit: int = None,
         with_vector: bool = False
```

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/vector/vector_db_interface.py` & `cognee-0.1.3/cognee/infrastructure/llm/llm_interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,40 @@
-from typing import List, Protocol, Optional
-from abc import abstractmethod
-from .models.DataPoint import DataPoint
-
-class VectorDBInterface(Protocol):
-    """ Collections """
-    @abstractmethod
-    async def create_collection(
-        self,
-        collection_name: str
-    ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def update_collection(
-    #     self,
-    #     collection_name: str,
-    #     collection_config: object
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def delete_collection(
-    #     self,
-    #     collection_name: str
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def create_vector_index(
-    #     self,
-    #     collection_name: str,
-    #     vector_index_config: object
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def create_data_index(
-    #     self,
-    #     collection_name: str,
-    #     vector_index_config: object
-    # ): raise NotImplementedError
+""" LLM Interface """
 
-    """ Data points """
-    @abstractmethod
-    async def create_data_points(
-        self,
-        collection_name: str,
-        data_points: List[DataPoint]
-    ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def get_data_point(
-    #     self,
-    #     collection_name: str,
-    #     data_point_id: str
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def update_data_point(
-    #     self,
-    #     collection_name: str,
-    #     data_point_id: str,
-    #     payload: object
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def delete_data_point(
-    #     self,
-    #     collection_name: str,
-    #     data_point_id: str
-    # ): raise NotImplementedError
-
-    """ Search """
+from typing import Type, Protocol
+from abc import abstractmethod
+from pydantic import BaseModel
+class LLMInterface(Protocol):
+    """ LLM Interface """
+
+    # @abstractmethod
+    # async def async_get_embedding_with_backoff(self, text, model="text-embedding-ada-002"):
+    #     """To get text embeddings, import/call this function"""
+    #     raise NotImplementedError
+    #
+    # @abstractmethod
+    # def get_embedding_with_backoff(self, text: str, model: str = "text-embedding-ada-002"):
+    #     """To get text embeddings, import/call this function"""
+    #     raise NotImplementedError
+    #
+    # @abstractmethod
+    # async def async_get_batch_embeddings_with_backoff(self, texts: List[str], models: List[str]):
+    #     """To get multiple text embeddings in parallel, import/call this function"""
+    #     raise NotImplementedError
+
+    # """ Get completions """
+    # async def acompletions_with_backoff(self, **kwargs):
+    #     raise NotImplementedError
+    #
+    """ Structured output """
     @abstractmethod
-    async def search(
-        self,
-        collection_name: str,
-        query_text: Optional[str],
-        query_vector: Optional[List[float]],
-        limit: int,
-        with_vector: bool = False
-
-    ): raise NotImplementedError
+    async def acreate_structured_output(self,
+                                        text_input: str,
+                                        system_prompt: str,
+                                        response_model: Type[BaseModel]) -> BaseModel:
+        """To get structured output, import/call this function"""
+        raise NotImplementedError
 
     @abstractmethod
-    async def batch_search(
-        self,
-        collection_name: str,
-        query_texts: List[str],
-        limit: int,
-        with_vectors: bool = False
-    ): raise NotImplementedError
+    def show_prompt(self, text_input: str, system_prompt: str) -> str:
+        """To get structured output, import/call this function"""
+        raise NotImplementedError
```

### Comparing `cognee-0.1.2/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py` & `cognee-0.1.3/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import asyncio
+from uuid import UUID
 from typing import List, Optional
 from multiprocessing import Pool
-import weaviate
-import weaviate.classes as wvc
-import weaviate.classes.config as wvcc
-from weaviate.classes.data import DataObject
 from ..vector_db_interface import VectorDBInterface
 from ..models.DataPoint import DataPoint
 from ..models.ScoredResult import ScoredResult
 from ..embeddings.EmbeddingEngine import EmbeddingEngine
 
 
 class WeaviateAdapter(VectorDBInterface):
     async_pool: Pool = None
     embedding_engine: EmbeddingEngine = None
 
     def __init__(self, url: str, api_key: str, embedding_engine: EmbeddingEngine):
+        import weaviate
+        import weaviate.classes as wvc
+      
         self.embedding_engine = embedding_engine
 
         self.client = weaviate.connect_to_wcs(
             cluster_url=url,
             auth_credentials=weaviate.auth.AuthApiKey(api_key),
             # headers = {
             #     "X-OpenAI-Api-Key": openai_api_key
@@ -26,67 +27,105 @@
             additional_config=wvc.init.AdditionalConfig(timeout=wvc.init.Timeout(init=30))
         )
 
     async def embed_data(self, data: List[str]) -> List[float]:
         return await self.embedding_engine.embed_text(data)
 
     async def create_collection(self, collection_name: str):
-        return self.client.collections.create(
-            name=collection_name,
-            properties=[
-                wvcc.Property(
-                    name="text",
-                    data_type=wvcc.DataType.TEXT,
-                    skip_vectorization=True
-                )
-            ]
-        )
+        import weaviate.classes.config as wvcc
+
+        event_loop = asyncio.get_event_loop()
+
+        def sync_create_collection():
+            return self.client.collections.create(
+                name=collection_name,
+                properties=[
+                    wvcc.Property(
+                        name="text",
+                        data_type=wvcc.DataType.TEXT,
+                        skip_vectorization=True
+                    )
+                ]
+            )
+
+        # try:
+        result = await event_loop.run_in_executor(None, sync_create_collection)
+        # finally:
+        #     event_loop.shutdown_executor()
+
+        return result
 
     def get_collection(self, collection_name: str):
         return self.client.collections.get(collection_name)
 
     async def create_data_points(self, collection_name: str, data_points: List[DataPoint]):
+        from weaviate.classes.data import DataObject
+
         data_vectors = await self.embed_data(
             list(map(lambda data_point: data_point.get_embeddable_data(), data_points)))
 
         def convert_to_weaviate_data_points(data_point: DataPoint):
             return DataObject(
                 uuid=data_point.id,
                 properties=data_point.payload,
                 vector=data_vectors[data_points.index(data_point)]
             )
 
         objects = list(map(convert_to_weaviate_data_points, data_points))
 
         return self.get_collection(collection_name).data.insert_many(objects)
 
+    async def retrieve(self, collection_name: str, data_id: str):
+        def sync_retrieve():
+            return self.get_collection(collection_name).query.fetch_object_by_id(UUID(data_id))
+
+        event_loop = asyncio.get_event_loop()
+
+        # try:
+        data_point = await event_loop.run_in_executor(None, sync_retrieve)
+        # finally:
+            # event_loop.shutdown_executor()
+
+        data_point.payload = data_point.properties
+        del data_point.properties
+
+        return data_point
+
     async def search(
             self,
             collection_name: str,
             query_text: Optional[str] = None,
             query_vector: Optional[List[float]] = None,
             limit: int = None,
             with_vector: bool = False
     ):
+        import weaviate.classes as wvc
+
         if query_text is None and query_vector is None:
             raise ValueError("One of query_text or query_vector must be provided!")
 
+        if query_vector is None:
+            query_vector = (await self.embed_data([query_text]))[0]
+
+        # def sync_search():
         search_result = self.get_collection(collection_name).query.hybrid(
-            query=None,
-            vector=query_vector if query_vector is not None else (await self.embed_data([query_text]))[0],
-            limit=limit,
-            include_vector=with_vector,
-            return_metadata=wvc.query.MetadataQuery(score=True),
+            query = None,
+            vector = query_vector,
+            limit = limit,
+            include_vector = with_vector,
+            return_metadata = wvc.query.MetadataQuery(score=True),
         )
 
-        return list(map(lambda result: ScoredResult(
-            id=str(result.uuid),
-            payload=result.properties,
-            score=float(result.metadata.score)
-        ), search_result.objects))
+        return [
+            ScoredResult(
+                id=str(result.uuid),
+                payload=result.properties,
+                score=float(result.metadata.score)
+            ) for result in search_result.objects
+        ]
 
     async def batch_search(self, collection_name: str, query_texts: List[str], limit: int, with_vectors: bool = False):
         def query_search(query_vector):
             return self.search(collection_name, query_vector=query_vector, limit=limit, with_vector=with_vectors)
 
         return [await query_search(query_vector) for query_vector in await self.embed_data(query_texts)]
```

### Comparing `cognee-0.1.2/cognee/infrastructure/files/storage/LocalStorage.py` & `cognee-0.1.3/cognee/infrastructure/files/storage/LocalStorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         with open(
             full_file_path,
             mode = "w" if isinstance(data, str) else "wb",
             encoding = "utf-8" if isinstance(data, str) else None
         ) as f:
             f.write(data if isinstance(data, str) else data.read())
 
-    def retrieve(self, file_path: str):
+    def retrieve(self, file_path: str, mode: str = "rb"):
         full_file_path = self.storage_path + "/" + file_path
 
-        with open(full_file_path, "rb") as f:
+        with open(full_file_path, mode = mode) as f:
             return f.read()
 
     @staticmethod
     def ensure_directory_exists(file_path: str):
         if not os.path.exists(file_path):
             os.makedirs(file_path)
```

### Comparing `cognee-0.1.2/cognee/infrastructure/files/storage/StorageManager.py` & `cognee-0.1.3/cognee/infrastructure/files/storage/StorageManager.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/files/utils/get_file_metadata.py` & `cognee-0.1.3/cognee/infrastructure/files/utils/get_file_metadata.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/files/utils/guess_file_type.py` & `cognee-0.1.3/cognee/infrastructure/files/utils/guess_file_type.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/files/utils/is_text_content.py` & `cognee-0.1.3/cognee/infrastructure/files/utils/is_text_content.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/anthropic/adapter.py` & `cognee-0.1.3/cognee/infrastructure/llm/anthropic/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-import asyncio
-
-import aiohttp
-from typing import List, Type
+from typing import Type
 from pydantic import BaseModel
 import instructor
 from tenacity import retry, stop_after_attempt
-
 import anthropic
-import openai
 from cognee.infrastructure.llm.llm_interface import LLMInterface
 from cognee.infrastructure.llm.prompts import read_query_prompt
 
 
 class AnthropicAdapter(LLMInterface):
     """Adapter for Ollama's API"""
 
-    def __init__(self, ollama_endpoint, api_key: str, model: str):
-
-
-        self.aclient =   instructor.patch(
-            create=anthropic.Anthropic().messages.create,
-            mode=instructor.Mode.ANTHROPIC_TOOLS
+    def __init__(self, model: str = None):
+        self.aclient = instructor.patch(
+            create = anthropic.Anthropic().messages.create,
+            mode = instructor.Mode.ANTHROPIC_TOOLS
         )
         self.model = model
 
-
-
-
-    @retry(stop=stop_after_attempt(5))
-    async def acreate_structured_output(self, text_input: str, system_prompt: str,
-                                        response_model: Type[BaseModel]) -> BaseModel:
+    @retry(stop = stop_after_attempt(5))
+    async def acreate_structured_output(
+        self,
+        text_input: str,
+        system_prompt: str,
+        response_model: Type[BaseModel]
+    ) -> BaseModel:
         """Generate a response from a user query."""
+
         return await self.aclient(
-            model=self.model,
-            max_tokens=4096,
-            max_retries=0,
-            messages=[
-                {
-                    "role": "user",
-                    "content": f"""Use the given format to
-                    extract information from the following input: {text_input}. {system_prompt}""",
-                }
-            ],
-            response_model=response_model,
+            model = self.model,
+            max_tokens = 4096,
+            max_retries = 0,
+            messages = [{
+                "role": "user",
+                "content": f"""Use the given format to extract information
+                from the following input: {text_input}. {system_prompt}""",
+            }],
+            response_model = response_model,
         )
 
     def show_prompt(self, text_input: str, system_prompt: str) -> str:
         """Format and display the prompt for a user query."""
+
         if not text_input:
             text_input = "No user input provided."
         if not system_prompt:
             raise ValueError("No system prompt path provided.")
+
         system_prompt = read_query_prompt(system_prompt)
 
         formatted_prompt = f"""System Prompt:\n{system_prompt}\n\nUser Input:\n{text_input}\n""" if system_prompt else None
+
         return formatted_prompt
```

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/generic_llm_api/adapter.py` & `cognee-0.1.3/cognee/infrastructure/llm/openai/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 import asyncio
-
-import aiohttp
 from typing import List, Type
-from pydantic import BaseModel
+import openai
 import instructor
+from openai import AsyncOpenAI, OpenAI
+from pydantic import BaseModel
 from tenacity import retry, stop_after_attempt
-from openai import AsyncOpenAI
-
-import openai
 from cognee.infrastructure.llm.llm_interface import LLMInterface
 from cognee.infrastructure.llm.prompts import read_query_prompt
 
-
-class GenericAPIAdapter(LLMInterface):
-    """Adapter for Ollama's API"""
-
-    def __init__(self, ollama_endpoint, api_key: str, model: str):
-
-        self.aclient =  instructor.patch(
-            AsyncOpenAI(
-                base_url=ollama_endpoint,
-                api_key=api_key,  # required, but unused
-            ),
-            mode=instructor.Mode.JSON,
-        )
+class OpenAIAdapter(LLMInterface):
+    """Adapter for OpenAI's GPT-3, GPT=4 API"""
+    def __init__(self, api_key: str, model:str):
+        openai.api_key = api_key
+        self.aclient = instructor.from_openai(AsyncOpenAI())
+        self.client = instructor.from_openai(OpenAI())
         self.model = model
 
-    @retry(stop=stop_after_attempt(5))
+    @retry(stop = stop_after_attempt(5))
     def completions_with_backoff(self, **kwargs):
         """Wrapper around ChatCompletion.create w/ backoff"""
-        # Local model
         return openai.chat.completions.create(**kwargs)
 
-    @retry(stop=stop_after_attempt(5))
-    async def acompletions_with_backoff(self, **kwargs):
+    @retry(stop = stop_after_attempt(5))
+    async def acompletions_with_backoff(self,**kwargs):
         """Wrapper around ChatCompletion.acreate w/ backoff"""
         return await openai.chat.completions.acreate(**kwargs)
 
-    @retry(stop=stop_after_attempt(5))
+    @retry(stop = stop_after_attempt(5))
     async def acreate_embedding_with_backoff(self, input: List[str], model: str = "text-embedding-3-large"):
         """Wrapper around Embedding.acreate w/ backoff"""
 
-        return await self.aclient.embeddings.create(input=input, model=model)
+        return await self.aclient.embeddings.create(input = input, model = model)
 
     async def async_get_embedding_with_backoff(self, text, model="text-embedding-3-large"):
         """To get text embeddings, import/call this function
         It specifies defaults + handles rate-limiting + is async"""
         text = text.replace("\n", " ")
-        response = await self.aclient.embeddings.create(input=text, model=model)
+        response = await self.aclient.embeddings.create(input = text, model = model)
         embedding = response.data[0].embedding
         return embedding
 
-    @retry(stop=stop_after_attempt(5))
+    @retry(stop = stop_after_attempt(5))
     def create_embedding_with_backoff(self, **kwargs):
         """Wrapper around Embedding.create w/ backoff"""
         return openai.embeddings.create(**kwargs)
 
     def get_embedding_with_backoff(self, text: str, model: str = "text-embedding-3-large"):
         """To get text embeddings, import/call this function
         It specifies defaults + handles rate-limiting
@@ -68,35 +57,54 @@
         return embedding
 
     async def async_get_batch_embeddings_with_backoff(self, texts: List[str], models: List[str]):
         """To get multiple text embeddings in parallel, import/call this function
         It specifies defaults + handles rate-limiting + is async"""
         # Collect all coroutines
         coroutines = (self.async_get_embedding_with_backoff(text, model)
-                      for text, model in zip(texts, models))
+            for text, model in zip(texts, models))
 
         # Run the coroutines in parallel and gather the results
         embeddings = await asyncio.gather(*coroutines)
 
         return embeddings
 
-    @retry(stop=stop_after_attempt(5))
-    async def acreate_structured_output(self, text_input: str, system_prompt: str,
-                                        response_model: Type[BaseModel]) -> BaseModel:
+    @retry(stop = stop_after_attempt(5))
+    async def acreate_structured_output(self, text_input: str, system_prompt: str, response_model: Type[BaseModel]) -> BaseModel:
         """Generate a response from a user query."""
+
         return await self.aclient.chat.completions.create(
-            model=self.model,
-            messages=[
+            model = self.model,
+            messages = [
+                {
+                    "role": "user",
+                    "content": f"""Use the given format to
+                    extract information from the following input: {text_input}. """,
+                },
+                {"role": "system", "content": system_prompt},
+            ],
+            response_model = response_model,
+        )
+
+
+    @retry(stop = stop_after_attempt(5))
+    def create_structured_output(self, text_input: str, system_prompt: str, response_model: Type[BaseModel]) -> BaseModel:
+        """Generate a response from a user query."""
+
+        return self.client.chat.completions.create(
+            model = self.model,
+            messages = [
                 {
                     "role": "user",
                     "content": f"""Use the given format to
-                    extract information from the following input: {text_input}. {system_prompt} """,
-                }
+                    extract information from the following input: {text_input}. """,
+                },
+                {"role": "system", "content": system_prompt},
             ],
-            response_model=response_model,
+            response_model = response_model,
         )
 
     def show_prompt(self, text_input: str, system_prompt: str) -> str:
         """Format and display the prompt for a user query."""
         if not text_input:
             text_input = "No user input provided."
         if not system_prompt:
```

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/get_llm_client.py` & `cognee-0.1.3/cognee/infrastructure/llm/get_llm_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Get the LLM client."""
 from enum import Enum
 from cognee.config import Config
 from .anthropic.adapter import AnthropicAdapter
 from .openai.adapter import OpenAIAdapter
 from .generic_llm_api.adapter import GenericAPIAdapter
-import logging
-logging.basicConfig(level=logging.INFO)
 
 # Define an Enum for LLM Providers
 class LLMProvider(Enum):
     OPENAI = "openai"
     OLLAMA = "ollama"
     ANTHROPIC = "anthropic"
     CUSTOM = "custom"
@@ -18,20 +16,16 @@
 config.load()
 
 def get_llm_client():
     """Get the LLM client based on the configuration using Enums."""
     provider = LLMProvider(config.llm_provider)
 
     if provider == LLMProvider.OPENAI:
-        return OpenAIAdapter(config.openai_key, config.model)
+        return OpenAIAdapter(config.openai_key, config.openai_model)
     elif provider == LLMProvider.OLLAMA:
         return GenericAPIAdapter(config.ollama_endpoint, config.ollama_key, config.ollama_model)
     elif provider == LLMProvider.ANTHROPIC:
-        return AnthropicAdapter(config.custom_endpoint, config.custom_endpoint, config.custom_model)
+        return AnthropicAdapter(config.custom_model)
     elif provider == LLMProvider.CUSTOM:
         return GenericAPIAdapter(config.custom_endpoint, config.custom_key, config.custom_model)
-        # Add your custom LLM provider here
     else:
         raise ValueError(f"Unsupported LLM provider: {provider}")
-
-# Usage example
-llm_client = get_llm_client()
```

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/openai/adapter.py` & `cognee-0.1.3/cognee/infrastructure/llm/generic_llm_api/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-"""Adapter for OpenAI's GPT-3, GPT=4 API."""
 import asyncio
 from typing import List, Type
-import openai
-import instructor
-from openai import AsyncOpenAI
 from pydantic import BaseModel
+import instructor
 from tenacity import retry, stop_after_attempt
+from openai import AsyncOpenAI
+import openai
 from cognee.infrastructure.llm.llm_interface import LLMInterface
 from cognee.infrastructure.llm.prompts import read_query_prompt
 
-class OpenAIAdapter(LLMInterface):
-    """Adapter for OpenAI's GPT-3, GPT=4 API"""
-    def __init__(self, api_key: str, model:str):
-        openai.api_key = api_key
-        self.aclient = instructor.patch(AsyncOpenAI())
+
+class GenericAPIAdapter(LLMInterface):
+    """Adapter for Ollama's API"""
+
+    def __init__(self, api_endpoint, api_key: str, model: str):
+        self.aclient =  instructor.patch(
+            AsyncOpenAI(
+                base_url = api_endpoint,
+                api_key = api_key,  # required, but unused
+            ),
+            mode = instructor.Mode.JSON,
+        )
         self.model = model
 
     @retry(stop = stop_after_attempt(5))
     def completions_with_backoff(self, **kwargs):
         """Wrapper around ChatCompletion.create w/ backoff"""
         # Local model
         return openai.chat.completions.create(**kwargs)
 
     @retry(stop = stop_after_attempt(5))
-    async def acompletions_with_backoff(self,**kwargs):
+    async def acompletions_with_backoff(self, **kwargs):
         """Wrapper around ChatCompletion.acreate w/ backoff"""
         return await openai.chat.completions.acreate(**kwargs)
 
     @retry(stop = stop_after_attempt(5))
     async def acreate_embedding_with_backoff(self, input: List[str], model: str = "text-embedding-3-large"):
         """Wrapper around Embedding.acreate w/ backoff"""
 
@@ -58,35 +64,35 @@
         return embedding
 
     async def async_get_batch_embeddings_with_backoff(self, texts: List[str], models: List[str]):
         """To get multiple text embeddings in parallel, import/call this function
         It specifies defaults + handles rate-limiting + is async"""
         # Collect all coroutines
         coroutines = (self.async_get_embedding_with_backoff(text, model)
-            for text, model in zip(texts, models))
+                      for text, model in zip(texts, models))
 
         # Run the coroutines in parallel and gather the results
         embeddings = await asyncio.gather(*coroutines)
 
         return embeddings
 
-    @retry(stop = stop_after_attempt(5))
-    async def acreate_structured_output(self, text_input: str, system_prompt: str, response_model: Type[BaseModel]) -> BaseModel:
+    @retry(stop=stop_after_attempt(5))
+    async def acreate_structured_output(self, text_input: str, system_prompt: str,
+                                        response_model: Type[BaseModel]) -> BaseModel:
         """Generate a response from a user query."""
         return await self.aclient.chat.completions.create(
-            model = self.model,
-            messages = [
+            model=self.model,
+            messages=[
                 {
                     "role": "user",
                     "content": f"""Use the given format to
-                    extract information from the following input: {text_input}. """,
-                },
-                {"role": "system", "content": system_prompt},
+                    extract information from the following input: {text_input}. {system_prompt} """,
+                }
             ],
-            response_model = response_model,
+            response_model=response_model,
         )
 
     def show_prompt(self, text_input: str, system_prompt: str) -> str:
         """Format and display the prompt for a user query."""
         if not text_input:
             text_input = "No user input provided."
         if not system_prompt:
```

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/prompts/classify_content.txt` & `cognee-0.1.3/cognee/infrastructure/llm/prompts/classify_content.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/prompts/generate_cog_layers.txt` & `cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_cog_layers.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 
 These layers can help in understanding the content, context, and characteristics of the `{{ data_type }}`.
 
 Your objective is to extract meaningful layers of information that will contribute to constructing a detailed multilayer network or knowledge graph.
 
 Approach this task by considering the unique characteristics and inherent properties of the data at hand.
 
-VERY IMPORTANT: The context you are working in is `{{ layer_name }}` and the specific domain you are extracting data on is `{{ layer_name }}`.
+VERY IMPORTANT: The context you are working in is `{{ category_name }}` and the specific domain you are extracting data on is `{{ category_name }}`.
 
 Guidelines for Layer Extraction:
-Take into account: The content type, in this case, is: `{{ layer_name }}`, should play a major role in how you decompose into layers.
+Take into account: The content type, in this case, is: `{{ category_name }}`, should play a major role in how you decompose into layers.
 
 Based on your analysis, define and describe the layers you've identified, explaining their relevance and contribution to understanding the dataset. Your independent identification of layers will enable a nuanced and multifaceted representation of the data, enhancing applications in knowledge discovery, content analysis, and information retrieval.
```

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt` & `cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 You are a top-tier algorithm
 designed for extracting information in structured formats to build a knowledge graph.
 - **Nodes** represent entities and concepts. They're akin to Wikipedia nodes.
 - **Edges** represent relationships between concepts. They're akin to Wikipedia links.
 - The aim is to achieve simplicity and clarity in the
 knowledge graph, making it accessible for a vast audience.
 YOU ARE ONLY EXTRACTING DATA FOR COGNITIVE LAYER `{{ layer }}`
-## 2. Labeling Nodes
+## 1. Labeling Nodes
 - **Consistency**: Ensure you use basic or elementary types for node labels.
   - For example, when you identify an entity representing a person,
-   always label it as **"person"**.
+   always label it as **"Person"**.
   Avoid using more specific terms like "mathematician" or "scientist".
   - Include event, entity, time, or action nodes to the category.
   - Classify the memory type as episodic or semantic.
 - **Node IDs**: Never utilize integers as node IDs.
     Node IDs should be names or human-readable identifiers found in the text.
-## 3. Handling Numerical Data and Dates
+## 2. Handling Numerical Data and Dates
 - Numerical data, like age or other related information,
 should be incorporated as attributes or properties of the respective nodes.
 - **No Separate Nodes for Dates/Numbers**:
 Do not create separate nodes for dates or numerical values.
  Always attach them as attributes or properties of nodes.
 - **Property Format**: Properties must be in a key-value format.
 - **Quotation Marks**: Never use escaped single or double quotes within property values.
-- **Naming Convention**: Use camelCase for property keys, e.g., `birthDate`.
-## 4. Coreference Resolution
+- **Naming Convention**: Use snake_case for relationship names, e.g., `acted_in`.
+## 3. Coreference Resolution
 - **Maintain Entity Consistency**:
 When extracting entities, it's vital to ensure consistency.
 If an entity, such as "John Doe", is mentioned multiple times
 in the text but is referred to by different names or pronouns (e.g., "Joe", "he"),
 always use the most complete identifier for that entity throughout the knowledge graph.
  In this example, use "John Doe" as the entity ID.
 Remember, the knowledge graph should be coherent and easily understandable,
  so maintaining consistency in entity references is crucial.
-## 5. Strict Compliance
+## 4. Strict Compliance
 Adhere to the rules strictly. Non-compliance will result in termination"""
```

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/prompts/read_query_prompt.py` & `cognee-0.1.3/cognee/infrastructure/llm/prompts/read_query_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/llm/prompts/render_prompt.py` & `cognee-0.1.3/cognee/infrastructure/llm/prompts/render_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/infrastructure/pipeline/models/Operation.py` & `cognee-0.1.3/cognee/infrastructure/pipeline/models/Operation.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/modules/cognify/graph/add_node_connections.py` & `cognee-0.1.3/cognee/modules/cognify/graph/add_node_connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,74 @@
-from networkx import Graph
+import uuid
+
+from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 from cognee.shared.data_models import GraphDBType
 
 
-async def extract_node_descriptions(node):
-    descriptions = []
-
-    for node_id, attributes in node:
-        if "description" in attributes and "unique_id" in attributes:
-            descriptions.append({
-                "node_id": attributes["unique_id"],
-                "description": attributes["description"],
-                "layer_uuid": attributes["layer_uuid"],
-                "layer_decomposition_uuid": attributes["layer_decomposition_uuid"]
-            })
-
-    return descriptions
-
 
 async def group_nodes_by_layer(node_descriptions):
+    """ Group nodes by layer decomposition uuid """
     grouped_data = {}
 
     for item in node_descriptions:
         uuid = item["layer_decomposition_uuid"]
-
         if uuid not in grouped_data:
             grouped_data[uuid] = []
-
         grouped_data[uuid].append(item)
 
+    print("GROUPED DATA", grouped_data)
+
     return grouped_data
 
-def connect_nodes_in_graph(graph: Graph, relationship_dict: dict, score_treshold:float=None) -> Graph:
-    """
-    For each relationship in relationship_dict, check if both nodes exist in the graph based on node attributes.
-    If they do, create a connection (edge) between them.
-
-    :param graph: A NetworkX graph object
-    :param relationship_dict: A dictionary containing relationships between nodes
-    """
-    if score_treshold is None:
-        score_treshold = 0.9
-    for id, relationships in relationship_dict.items():
+
+async def get_node_by_unique_id(graph, unique_id):
+    """ Get a node by its unique_id"""
+    # Iterate through all nodes and their attributes in the graph
+    for node, attrs in graph.nodes(data=True):
+        # Check if the current node's attributes contain the unique_id we're looking for
+        if attrs.get('unique_id') == unique_id:
+            return node  # Return the node (identifier) if found
+    return None
+
+async def connect_nodes_in_graph(graph, relationship_dict, score_threshold=0.9):
+    """ Connect nodes in the graph based on the relationship_dict and score_threshold"""
+    if not graph or not relationship_dict:
+        return graph
+
+    for _, relationships in relationship_dict.items():
         for relationship in relationships:
-            searched_node_attr_id = relationship["searched_node_id"]
-            score_attr_id = relationship["original_id_for_search"]
-            score = relationship["score"]
-
-            if score> score_treshold:
-                # Initialize node keys for both searched_node and score_node
-                searched_node_key, score_node_key = None, None
-
-                # Find nodes in the graph that match the searched_node_id and score_id from their attributes
-                for node, attrs in graph.nodes(data = True):
-                    if "unique_id" in attrs:  # Ensure there is an "id" attribute
-                        if attrs["unique_id"] == searched_node_attr_id:
-                            searched_node_key = node
-                        elif attrs["unique_id"] == score_attr_id:
-                            score_node_key = node
-
-                    # If both nodes are found, no need to continue checking other nodes
-                    if searched_node_key and score_node_key:
-                        break
-
-                # Check if both nodes were found in the graph
-                if searched_node_key is not None and score_node_key is not None:
-                    # print(f"Connecting {searched_node_key} to {score_node_key}")
-                    # If both nodes exist, create an edge between them
-                    # You can customize the edge attributes as needed, here we use "score" as an attribute
-                    graph.add_edge(
-                        searched_node_key,
-                        score_node_key,
-                        weight = score,
-                        score_metadata = relationship.get("score_metadata")
-                    )
-            else:
-                pass
 
-    return graph
+            if relationship['score'] > score_threshold:
+
+                # For NetworkX
+                if infrastructure_config.get_config()["graph_engine"] == GraphDBType.NETWORKX:
+                    searched_node_id_found = await get_node_by_unique_id(graph.graph, relationship['searched_node_id'])
+                    original_id_for_search_found = await get_node_by_unique_id(graph.graph, relationship['original_id_for_search'])
+                    if searched_node_id_found and original_id_for_search_found:
+                        await graph.add_edge(
+                            searched_node_id_found,
+                            original_id_for_search_found,
+                            weight=relationship['score'],
+                            score_metadata=relationship.get('score_metadata', {}),
+                            id = f""" SEMANTIC_CONNECTION_{searched_node_id_found}_{original_id_for_search_found}_{str(uuid.uuid4())}"""
+                        )
+
+                # For Neo4j
+                elif infrastructure_config.get_config()["graph_engine"] == GraphDBType.NEO4J:
+                    # Neo4j specific logic to add an edge
+                    # This is just a placeholder, replace it with actual Neo4j logic
+                    print("query is ", f"""MATCH (a), (b) WHERE a.unique_id = '{relationship['searched_node_id']}' AND b.unique_id = '{relationship['original_id_for_search']}' CREATE (a)-[:CONNECTED {{weight:{relationship['score']}}}]->(b)""")
+                    result = await graph.query(f"""MATCH (a), (b) WHERE a.unique_id = '{relationship['searched_node_id']}' AND b.unique_id = '{relationship['original_id_for_search']}'
+                              CREATE (a)-[:SEMANTIC_CONNECTION {{weight:{relationship['score']}}}]->(b)""")
+                    await graph.close()
 
 
 def graph_ready_output(results):
+    """ Generate a dictionary of relationships from the results of the graph search."""
     relationship_dict = {}
 
     for result in results:
         layer_id = result["layer_id"]
         layer_nodes = result["layer_nodes"]
 
         # Ensure there's a list to collect related items for this uuid
@@ -104,29 +88,25 @@
 
     return relationship_dict
 
 
 if __name__ == "__main__":
 
     async def main():
-        graph_client = get_graph_client(GraphDBType.NETWORKX)
-
-        await graph_client.load_graph_from_file()
-
-
+        graph_client = await get_graph_client(GraphDBType.NEO4J)
         graph = graph_client.graph
 
         # for nodes, attr in graph.nodes(data=True):
         #     if 'd0bd0f6a-09e5-4308-89f6-400d66895126' in nodes:
         #         print(nodes)
 
-
-        relationships = {'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah': [{'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'd0bd0f6a-09e5-4308-89f6-400d66895126', 'score': 1.0, 'score_metadata': {'text': 'Pravilnik o izmenama i dopunama Pravilnika o sadržini, načinu i postupku izrade i način vršenja kontrole tehničke dokumentacije prema klasi i nameni objekata'}, 'original_id_for_search': '2801f7b5-55bf-499b-9843-97d48f8e067a'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'd0bd0f6a-09e5-4308-89f6-400d66895126', 'score': 0.1648828387260437, 'score_metadata': {'text': 'Zakon o planiranju i izgradnji'}, 'original_id_for_search': '57966b55-33e2-4eae-a7fa-2f0237643bbe'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'd0bd0f6a-09e5-4308-89f6-400d66895126', 'score': 0.12986786663532257, 'score_metadata': {'text': 'Službeni glasnik RS, broj 77/2015'}, 'original_id_for_search': '0f626d48-4441-43c1-9060-ea7e54f6d8e2'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'c9b9a460-c64a-4e2e-a4d6-aa5b3769274b', 'score': 1.0, 'score_metadata': {'text': 'Službeni glasnik RS, broj 77/2015'}, 'original_id_for_search': '0f626d48-4441-43c1-9060-ea7e54f6d8e2'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'c9b9a460-c64a-4e2e-a4d6-aa5b3769274b', 'score': 0.07603412866592407, 'score_metadata': {'text': 'Prof. dr Zorana Mihajlović'}, 'original_id_for_search': '5d064a62-3cd6-4895-9f60-1a0d8bc299e8'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'c9b9a460-c64a-4e2e-a4d6-aa5b3769274b', 'score': 0.07226034998893738, 'score_metadata': {'text': 'Ministar građevinarstva, saobraćaja i infrastrukture'}, 'original_id_for_search': 'f5d052ca-c4a0-490e-a3ac-d8ad522dea83'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'bbd6d2d6-e673-4b59-a50c-516972a9d0de', 'score': 0.5, 'score_metadata': {'text': 'Pravilnik o izmenama i dopunama Pravilnika o sadržini, načinu i postupku izrade i način vršenja kontrole tehničke dokumentacije prema klasi i nameni objekata'}, 'original_id_for_search': '2801f7b5-55bf-499b-9843-97d48f8e067a'}]}
-
-        connect_nodes_in_graph(graph, relationships)
+        #
+        # relationships = {'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah': [{'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'd0bd0f6a-09e5-4308-89f6-400d66895126', 'score': 1.0, 'score_metadata': {'text': 'Pravilnik o izmenama i dopunama Pravilnika o sadržini, načinu i postupku izrade i način vršenja kontrole tehničke dokumentacije prema klasi i nameni objekata'}, 'original_id_for_search': '2801f7b5-55bf-499b-9843-97d48f8e067a'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'd0bd0f6a-09e5-4308-89f6-400d66895126', 'score': 0.1648828387260437, 'score_metadata': {'text': 'Zakon o planiranju i izgradnji'}, 'original_id_for_search': '57966b55-33e2-4eae-a7fa-2f0237643bbe'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'd0bd0f6a-09e5-4308-89f6-400d66895126', 'score': 0.12986786663532257, 'score_metadata': {'text': 'Službeni glasnik RS, broj 77/2015'}, 'original_id_for_search': '0f626d48-4441-43c1-9060-ea7e54f6d8e2'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'c9b9a460-c64a-4e2e-a4d6-aa5b3769274b', 'score': 1.0, 'score_metadata': {'text': 'Službeni glasnik RS, broj 77/2015'}, 'original_id_for_search': '0f626d48-4441-43c1-9060-ea7e54f6d8e2'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'c9b9a460-c64a-4e2e-a4d6-aa5b3769274b', 'score': 0.07603412866592407, 'score_metadata': {'text': 'Prof. dr Zorana Mihajlović'}, 'original_id_for_search': '5d064a62-3cd6-4895-9f60-1a0d8bc299e8'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'c9b9a460-c64a-4e2e-a4d6-aa5b3769274b', 'score': 0.07226034998893738, 'score_metadata': {'text': 'Ministar građevinarstva, saobraćaja i infrastrukture'}, 'original_id_for_search': 'f5d052ca-c4a0-490e-a3ac-d8ad522dea83'}, {'collection_id': 'SuaGeKyKWKWyaSeiqWeWaSyuSKqieSamiyah', 'searched_node_id': 'bbd6d2d6-e673-4b59-a50c-516972a9d0de', 'score': 0.5, 'score_metadata': {'text': 'Pravilnik o izmenama i dopunama Pravilnika o sadržini, načinu i postupku izrade i način vršenja kontrole tehničke dokumentacije prema klasi i nameni objekata'}, 'original_id_for_search': '2801f7b5-55bf-499b-9843-97d48f8e067a'}]}
+        #
+        # connect_nodes_in_graph(graph, relationships)
 
         from cognee.utils import render_graph
 
         graph_url = await render_graph(graph)
 
         print(graph_url)
```

### Comparing `cognee-0.1.2/cognee/modules/cognify/llm/label_content.py` & `cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-""" This module contains the code to classify content into categories using the LLM API. """
 from typing import Type
 from pydantic import BaseModel
-from cognee.infrastructure.llm.prompts import read_query_prompt
 from cognee.infrastructure.llm.get_llm_client import get_llm_client
+from cognee.infrastructure.llm.prompts import render_prompt
 
-async def label_content(text_input: str, system_prompt_file: str, response_model: Type[BaseModel]):
+async def extract_content_graph(content: str, cognitive_layer: str, response_model: Type[BaseModel]):
     llm_client = get_llm_client()
 
-    system_prompt = read_query_prompt(system_prompt_file)
+    system_prompt = render_prompt("generate_graph_prompt.txt", { "layer": cognitive_layer })
+    output = await llm_client.acreate_structured_output(content, system_prompt, response_model)
 
-    llm_output = await llm_client.acreate_structured_output(text_input, system_prompt, response_model)
-
-    return llm_output.model_dump()
+    return output.model_dump()
```

### Comparing `cognee-0.1.2/cognee/modules/cognify/llm/resolve_cross_graph_references.py` & `cognee-0.1.3/cognee/modules/cognify/llm/resolve_cross_graph_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     return results
 
 async def get_nodes_by_layer(layer_id: str, layer_nodes: List):
     vector_engine = infrastructure_config.get_config()["vector_engine"]
 
     score_points = await vector_engine.batch_search(
         layer_id,
-        list(map(lambda node: node["description"], layer_nodes)),
-        limit = 3
+        [layer_node["description"] for layer_node in layer_nodes],
+        limit = 2
     )
 
     return {
         "layer_id": layer_id,
         "layer_nodes": connect_score_points_to_node(score_points, layer_nodes)
     }
```

### Comparing `cognee-0.1.2/cognee/modules/discovery/discover_directory_datasets.py` & `cognee-0.1.3/cognee/modules/discovery/discover_directory_datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/modules/ingestion/add_data_to_dataset.py` & `cognee-0.1.3/cognee/modules/ingestion/add_data_to_dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/modules/ingestion/save.py` & `cognee-0.1.3/cognee/modules/ingestion/save.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/modules/users/memory/create_information_points.py` & `cognee-0.1.3/cognee/modules/users/memory/create_information_points.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.2/cognee/shared/data_models.py` & `cognee-0.1.3/cognee/shared/data_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 """Data models for the cognitive architecture."""
+
 from enum import Enum, auto
 from typing import Optional, List, Union, Dict, Any
 from pydantic import BaseModel, Field
 
 class Node(BaseModel):
     """Node in a knowledge graph."""
     id: str
-    description: str
-    category: str
-    color: str = "blue"
-    memory_type: str
-    created_at: Optional[float] = None
-    summarized: Optional[bool] = None
+    entity_name: str
+    entity_type: str
+    entity_description: str
 
 class Edge(BaseModel):
     """Edge in a knowledge graph."""
-    source: str
-    target: str
-    description: str
-    color: str = "blue"
-    created_at: Optional[float] = None
-    summarized: Optional[bool] = None
+    source_node_id: str
+    target_node_id: str
+    relationship_name: str
 
 class KnowledgeGraph(BaseModel):
     """Knowledge graph."""
     nodes: List[Node] = Field(..., default_factory=list)
     edges: List[Edge] = Field(..., default_factory=list)
 
 class GraphQLQuery(BaseModel):
     """GraphQL query."""
     query: str
 
+
+
+class Answer(BaseModel):
+    """Answer."""
+    answer: str
+
+class ChunkStrategy(Enum):
+    EXACT = "exact"
+    PARAGRAPH = "paragraph"
+    SENTENCE = "sentence"
+    VANILLA = "vanilla"
+    SUMMARY = "summary"
+
 class MemorySummary(BaseModel):
     """ Memory summary. """
     nodes: List[Node] = Field(..., default_factory=list)
     edges: List[Edge] = Field(..., default_factory=list)
 
+
 class TextSubclass(str, Enum):
     ARTICLES = "Articles, essays, and reports"
     BOOKS = "Books and manuscripts"
     NEWS_STORIES = "News stories and blog posts"
     RESEARCH_PAPERS = "Research papers and academic publications"
     SOCIAL_MEDIA = "Social media posts and comments"
     WEBSITE_CONTENT = "Website content and product descriptions"
@@ -96,14 +105,15 @@
     PHOTOGRAPHS = "Photographs and digital images"
     ILLUSTRATIONS = "Illustrations, diagrams, and charts"
     INFOGRAPHICS = "Infographics and visual data representations"
     ARTWORK = "Artwork and paintings"
     SCREENSHOTS = "Screenshots and graphical user interfaces"
     OTHER_IMAGES = "Other types of images"
 
+
 class VideoSubclass(str, Enum):
     MOVIES = "Movies and short films"
     DOCUMENTARIES = "Documentaries and educational videos"
     TUTORIALS = "Video tutorials and how-to guides"
     ANIMATED_FEATURES = "Animated features and cartoons"
     LIVE_EVENTS = "Live event recordings and sports broadcasts"
     OTHER_VIDEOS = "Other types of video content"
@@ -132,109 +142,113 @@
     OTHER_PROCEDURAL = "Other types of procedural content"
 
 class ContentType(BaseModel):
     """Base class for different types of content."""
     type: str
 
 class TextContent(ContentType):
-    type:str = "TEXT"
+    type: str = "TEXT"
     subclass: List[TextSubclass]
 
 class AudioContent(ContentType):
-    type:str = "AUDIO"
+    type: str = "AUDIO"
     subclass: List[AudioSubclass]
 
 class ImageContent(ContentType):
-    type:str = "IMAGE"
+    type: str = "IMAGE"
     subclass: List[ImageSubclass]
 
 class VideoContent(ContentType):
-    type:str = "VIDEO"
+    type: str = "VIDEO"
     subclass: List[VideoSubclass]
 
 class MultimediaContent(ContentType):
-    type:str = "MULTIMEDIA"
+    type: str = "MULTIMEDIA"
     subclass: List[MultimediaSubclass]
 
 class Model3DContent(ContentType):
-    type:str = "3D_MODEL"
+    type: str = "3D_MODEL"
     subclass: List[Model3DSubclass]
 
 class ProceduralContent(ContentType):
-    type:str = "PROCEDURAL"
+    type: str = "PROCEDURAL"
     subclass: List[ProceduralSubclass]
 
 class DefaultContentPrediction(BaseModel):
     """Class for a single class label prediction."""
-
-    label: Union[TextContent, AudioContent, ImageContent, VideoContent, MultimediaContent, Model3DContent, ProceduralContent]
-
+    label: Union[
+        TextContent,
+        AudioContent,
+        ImageContent,
+        VideoContent,
+        MultimediaContent,
+        Model3DContent,
+        ProceduralContent,
+    ]
 
 
 class SummarizedContent(BaseModel):
-    """Class for a single class label summary."""
-
+    """Class for a single class label summary and description."""
     summary: str
+    description: str
 
 class LabeledContent(BaseModel):
     """Class for a single class label summary."""
-
     content_labels: str
 
 
 
 class CognitiveLayerSubgroup(BaseModel):
     """ CognitiveLayerSubgroup in a general layer """
     id: int
-    name:str
+    name: str
     description: str
 
 
 class DefaultCognitiveLayer(BaseModel):
     """Cognitive  layer"""
-    category_name:str
+    category_name: str
     cognitive_layers: List[CognitiveLayerSubgroup] = Field(..., default_factory=list)
 
 
 class GraphDBType(Enum):
     NETWORKX = auto()
     NEO4J = auto()
 
 
 # Models for representing different entities
 class Relationship(BaseModel):
     type: str
+    source: Optional[str] = None
+    target: Optional[str] = None
     properties: Optional[Dict[str, Any]] = None
 
 class DocumentType(BaseModel):
     type_id: str
     description: str
     default_relationship: Relationship = Relationship(type = "is_type")
 
 class Category(BaseModel):
     category_id: str
     name: str
     default_relationship: Relationship = Relationship(type = "categorized_as")
 
 class Document(BaseModel):
-    doc_id: str
+    id: str
     title: str
-    summary: Optional[str] = None
-    content_id: Optional[str] = None
-    doc_type: Optional[DocumentType] = None
-    categories: List[Category] = []
-    default_relationship: Relationship = Relationship(type = "has_document")
+    description: Optional[str] = None
 
 class UserLocation(BaseModel):
     location_id: str
     description: str
     default_relationship: Relationship = Relationship(type = "located_in")
 
 class UserProperties(BaseModel):
     custom_properties: Optional[Dict[str, Any]] = None
     location: Optional[UserLocation] = None
 
 class DefaultGraphModel(BaseModel):
-    id: str
+    node_id: str
     user_properties: UserProperties = UserProperties()
     documents: List[Document] = []
     default_fields: Optional[Dict[str, Any]] = {}
+    default_relationship: Relationship = Relationship(type = "has_properties")
```

### Comparing `cognee-0.1.2/pyproject.toml` & `cognee-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "cognee"
-version = "0.1.2"
+version = "0.1.3"
 description = "Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning."
-authors = ["Vasilije Markovic"]
+authors = ["Vasilije Markovic", "Boris Arzentar"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.cognee.ai"
 repository = "https://github.com/topoteretes/cognee"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -14,51 +14,58 @@
     "Topic :: Software Development :: Libraries",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows"
 ]
 
 [tool.poetry.dependencies]
-python = "~3.11"
+python = ">=3.9.0,<3.12"
 openai = "1.14.3"
+pydantic = "^2.5.0"
 python-dotenv = "1.0.1"
 fastapi = "^0.109.2"
 uvicorn = "0.22.0"
 boto3 = "^1.26.125"
 gunicorn = "^20.1.0"
 sqlalchemy = "^2.0.21"
 asyncpg = "^0.28.0"
-instructor = "^0.6.8"
+instructor = "1.2.1"
 networkx = "^3.2.1"
 graphviz = "^0.20.1"
 debugpy = "^1.8.0"
 pyarrow = "^15.0.0"
 pylint = "^3.0.3"
 aiosqlite = "^0.20.0"
 pandas = "^2.2.0"
 greenlet = "^3.0.3"
 ruff = "^0.2.2"
 filetype = "^1.2.0"
 nltk = "^3.8.1"
-dlt = "^0.4.6"
+dlt = "^0.4.7"
 duckdb = {version = "^0.10.0", extras = ["dlt"]}
 overrides = "^7.7.0"
 aiofiles = "^23.2.1"
 qdrant-client = "^1.8.0"
 duckdb-engine = "^0.11.2"
 graphistry = "^0.33.5"
 tenacity = "^8.2.3"
 weaviate-client = "^4.5.4"
 scikit-learn = "^1.4.1.post1"
 fastembed = "^0.2.5"
 pypdf = "^4.1.0"
 anthropic = "^0.21.3"
 xmltodict = "^0.13.0"
+neo4j = "^5.18.0"
 jinja2 = "^3.1.3"
 matplotlib = "^3.8.3"
+nest-asyncio = "^1.6.0"
+structlog = "^24.1.0"
+tiktoken = "^0.6.0"
+dspy-ai = "2.4.3"
+
 
 [tool.poetry.extras]
 dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb", "dbt-snowflake", "dbt-athena-community", "dbt-databricks"]
 gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
 # bigquery is alias on gcp extras
 bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
 postgres = ["psycopg2-binary", "psycopg2cffi"]
```

### Comparing `cognee-0.1.2/PKG-INFO` & `cognee-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: cognee
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning.
 Home-page: https://www.cognee.ai
 License: Apache-2.0
 Author: Vasilije Markovic
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: athena
 Provides-Extra: az
 Provides-Extra: bigquery
 Provides-Extra: cli
 Provides-Extra: databricks
@@ -40,60 +42,67 @@
 Provides-Extra: weaviate
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: asyncpg (>=0.28.0,<0.29.0)
 Requires-Dist: boto3 (>=1.26.125,<2.0.0)
 Requires-Dist: debugpy (>=1.8.0,<2.0.0)
-Requires-Dist: dlt (>=0.4.6,<0.5.0)
+Requires-Dist: dlt (>=0.4.7,<0.5.0)
+Requires-Dist: dspy-ai (==2.4.3)
 Requires-Dist: duckdb-engine (>=0.11.2,<0.12.0)
 Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra == "duckdb" or extra == "motherduck"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fastembed (>=0.2.5,<0.3.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: graphistry (>=0.33.5,<0.34.0)
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: instructor (>=0.6.8,<0.7.0)
+Requires-Dist: instructor (==1.2.1)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
+Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
+Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==1.14.3)
 Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena" or extra == "synapse"
+Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pylint (>=3.0.3,<4.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
 Requires-Dist: qdrant-client (>=1.8.0,<2.0.0)
 Requires-Dist: ruff (>=0.2.2,<0.3.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
+Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: uvicorn (==0.22.0)
 Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate"
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/topoteretes/cognee
 Description-Content-Type: text/markdown
 
 # cognee
 
-Make data processing for LLMs easy
+Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and vector retrieval
 
 
 <p>
   <a href="https://cognee.ai" target="_blank">
-    <img src="assets/cognee-logo.png" width="160px" alt="Cognee logo" />
+    <img src="https://raw.githubusercontent.com/topoteretes/cognee/main/assets/cognee-logo.png" width="160px" alt="Cognee logo" />
   </a>
 </p>
 
+
 <p>
-  <i>Open-source framework for creating knowledge graphs and data models for LLMs.</i>
+  <i>Open-source framework for creating self-improving deterministic outputs for LLMs.</i>
 </p>
 
 <p>
   <a href="https://github.com/topoteretes/cognee/fork">
     <img src="https://img.shields.io/github/forks/topoteretes/cognee?style=for-the-badge" alt="cognee forks"/>
   </a>
   <a href="https://github.com/topoteretes/cognee/stargazers">
@@ -103,21 +112,17 @@
     <img src="https://img.shields.io/github/issues-pr/topoteretes/cognee?style=for-the-badge" alt="cognee pull-requests"/>
   </a>
   <a href="https://github.com/topoteretes/cognee/releases">
     <img src="https://img.shields.io/github/release/topoteretes/cognee?&label=Latest&style=for-the-badge" alt="cognee releases" />
   </a>
 </p>
 
+![Cognee Demo](assets/cognee_demo.gif)
 
-## 🚀 It's alive
-
-<p>
-Try it yourself on Whatsapp with one of our <a href="https://keepi.ai" target="_blank">partners</a> by typing `/save {content you want to save}` followed by `/query {knowledge you saved previously}`
-For more info here are the <a href="https://topoteretes.github.io/cognee">docs</a>
-</p>
+For more details, have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
 
 
 ## 📦 Installation
 
 With pip:
 
 ```bash
@@ -139,14 +144,15 @@
 
 os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
 os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY"
 
 os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
 
 ```
+You can also use Ollama or Anyscale as your LLM provider. For more info on local models check our [docs](https://topoteretes.github.io/cognee)
 
 ### Run
 
 ```
 import cognee
 
 text = """Natural language processing (NLP) is an interdisciplinary
@@ -186,24 +192,30 @@
 Read more [here](docs/index.md#run).
 
 ## Demo
 
 Check out our demo notebook [here](https://github.com/topoteretes/cognee/blob/main/notebooks/cognee%20-%20Get%20Started.ipynb)
 
 
-## Architecture
 
-[<img src="https://i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg" width="100%">](https://youtu.be/-ARUfIzhzC4 "Learn about cognee: 55")
+[<img src="https://i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg" width="100%">](https://www.youtube.com/watch?v=BDFt4xVPmro "Learn about cognee: 55")
+
+
 
 
-### How Cognee Enhances Your Contextual Memory
 
-Our framework for the OpenAI, Graph (Neo4j) and Vector (Weaviate) databases introduces three key enhancements:
+## How it works
+
+
 
-- Query Classifiers: Navigate information graph using Pydantic OpenAI classifiers.
-- Document Topology: Structure and store documents in public and private domains.
-- Personalized Context: Provide a context object to the LLM for a better response.
 
 
 ![Image](assets/architecture.png)
 
 
+## 🚀 It's alive
+
+<p>
+Try it yourself on Whatsapp with one of our <a href="https://keepi.ai" target="_blank">partners</a> by typing `/save {content you want to save}` followed by `/query {knowledge you saved previously}`
+For more info here are the <a href="https://topoteretes.github.io/cognee">docs</a>
+</p>
+
```

#### html2text {}

```diff
@@ -1,76 +1,79 @@
-Metadata-Version: 2.1 Name: cognee Version: 0.1.2 Summary: Cognee - is a
+Metadata-Version: 2.1 Name: cognee Version: 0.1.3 Summary: Cognee - is a
 library for enriching LLM context with a semantic layer for better
 understanding and reasoning. Home-page: https://www.cognee.ai License: Apache-
-2.0 Author: Vasilije Markovic Requires-Python: >=3.11,<3.12 Classifier:
+2.0 Author: Vasilije Markovic Requires-Python: >=3.9.0,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.11 Classifier: Topic :: Software Development :: Libraries Provides-Extra:
-athena Provides-Extra: az Provides-Extra: bigquery Provides-Extra: cli
-Provides-Extra: databricks Provides-Extra: dbt Provides-Extra: duckdb Provides-
-Extra: filesystem Provides-Extra: gcp Provides-Extra: gs Provides-Extra:
-lancedb Provides-Extra: motherduck Provides-Extra: mssql Provides-Extra: neo4j
-Provides-Extra: notebook Provides-Extra: parquet Provides-Extra: pinecone
-Provides-Extra: postgres Provides-Extra: redshift Provides-Extra: s3 Provides-
-Extra: snowflake Provides-Extra: synapse Provides-Extra: weaviate Requires-
-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
-Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist: asyncpg
-(>=0.28.0,<0.29.0) Requires-Dist: boto3 (>=1.26.125,<2.0.0) Requires-Dist:
-debugpy (>=1.8.0,<2.0.0) Requires-Dist: dlt (>=0.4.6,<0.5.0) Requires-Dist:
-duckdb-engine (>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0)
-; extra == "duckdb" or extra == "motherduck" Requires-Dist: fastapi
-(>=0.109.2,<0.110.0) Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist:
-filetype (>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0)
-Requires-Dist: graphviz (>=0.20.1,<0.21.0) Requires-Dist: greenlet
-(>=3.0.3,<4.0.0) Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist:
-instructor (>=0.6.8,<0.7.0) Requires-Dist: jinja2 (>=3.1.3,<4.0.0) Requires-
-Dist: matplotlib (>=3.8.3,<4.0.0) Requires-Dist: networkx (>=3.2.1,<4.0.0)
-Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai (==1.14.3) Requires-
-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook" Requires-Dist: pandas
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Libraries Provides-Extra: athena Provides-Extra: az Provides-
+Extra: bigquery Provides-Extra: cli Provides-Extra: databricks Provides-Extra:
+dbt Provides-Extra: duckdb Provides-Extra: filesystem Provides-Extra: gcp
+Provides-Extra: gs Provides-Extra: lancedb Provides-Extra: motherduck Provides-
+Extra: mssql Provides-Extra: neo4j Provides-Extra: notebook Provides-Extra:
+parquet Provides-Extra: pinecone Provides-Extra: postgres Provides-Extra:
+redshift Provides-Extra: s3 Provides-Extra: snowflake Provides-Extra: synapse
+Provides-Extra: weaviate Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-
+Dist: aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: anthropic (>=0.21.3,<0.22.0)
+Requires-Dist: asyncpg (>=0.28.0,<0.29.0) Requires-Dist: boto3
+(>=1.26.125,<2.0.0) Requires-Dist: debugpy (>=1.8.0,<2.0.0) Requires-Dist: dlt
+(>=0.4.7,<0.5.0) Requires-Dist: dspy-ai (==2.4.3) Requires-Dist: duckdb-engine
+(>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra ==
+"duckdb" or extra == "motherduck" Requires-Dist: fastapi (>=0.109.2,<0.110.0)
+Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist: filetype
+(>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0) Requires-Dist:
+graphviz (>=0.20.1,<0.21.0) Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-
+Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: instructor (==1.2.1) Requires-
+Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
+Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j" Requires-Dist: nest-
+asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx (>=3.2.1,<4.0.0) Requires-
+Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai (==1.14.3) Requires-Dist:
+overrides (>=7.7.0,<8.0.0) ; extra == "notebook" Requires-Dist: pandas
 (>=2.2.0,<3.0.0) Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra ==
 "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena"
-or extra == "synapse" Requires-Dist: pylint (>=3.0.3,<4.0.0) Requires-Dist:
-pypdf (>=4.1.0,<5.0.0) Requires-Dist: python-dotenv (==1.0.1) Requires-Dist:
-qdrant-client (>=1.8.0,<2.0.0) Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-
-Dist: scikit-learn (>=1.4.1.post1,<2.0.0) Requires-Dist: sqlalchemy
-(>=2.0.21,<3.0.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-Dist:
-uvicorn (==0.22.0) Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra ==
-"weaviate" Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository,
-https://github.com/topoteretes/cognee Description-Content-Type: text/markdown #
-cognee Make data processing for LLMs easy
+or extra == "synapse" Requires-Dist: pydantic (>=2.5.0,<3.0.0) Requires-Dist:
+pylint (>=3.0.3,<4.0.0) Requires-Dist: pypdf (>=4.1.0,<5.0.0) Requires-Dist:
+python-dotenv (==1.0.1) Requires-Dist: qdrant-client (>=1.8.0,<2.0.0) Requires-
+Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
+Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0) Requires-Dist: structlog
+(>=24.1.0,<25.0.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-Dist:
+tiktoken (>=0.6.0,<0.7.0) Requires-Dist: uvicorn (==0.22.0) Requires-Dist:
+weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate" Requires-Dist: xmltodict
+(>=0.13.0,<0.14.0) Project-URL: Repository, https://github.com/topoteretes/
+cognee Description-Content-Type: text/markdown # cognee Deterministic LLMs
+Outputs for AI Engineers using graphs, LLMs and vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
-Open-source framework for creating knowledge graphs and data models for LLMs.
+Open-source framework for creating self-improving deterministic outputs for
+LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
-## ð It's alive
-Try it yourself on Whatsapp with one of our _p_a_r_t_n_e_r_s by typing `/save {content
-you want to save}` followed by `/query {knowledge you saved previously}` For
-more info here are the _d_o_c_s
-## ð¦ Installation With pip: ```bash pip install "cognee[weaviate]" ``` With
-poetry: ```bash poetry add "cognee[weaviate]" ``` ## ð» Usage ### Setup ```
-import os os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ
-["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] =
-"YOUR_OPENAI_API_KEY" ``` ### Run ``` import cognee text = """Natural language
-processing (NLP) is an interdisciplinary subfield of computer science and
-information retrieval""" cognee.add(text) # Add a new piece of information
-cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
-cognee.search("SIMILARITY", "computer science") # Query cognee for the
-knowledge for result_text in search_results[0]: print(result_text) ``` Add
-alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
+![Cognee Demo](assets/cognee_demo.gif) For more details, have a look at our
+_d_o_c_u_m_e_n_t_a_t_i_o_n ## ð¦ Installation With pip: ```bash pip install "cognee
+[weaviate]" ``` With poetry: ```bash poetry add "cognee[weaviate]" ``` ## ð»
+Usage ### Setup ``` import os os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
+os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY" os.environ
+["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY" ``` You can also use Ollama or
+Anyscale as your LLM provider. For more info on local models check our [docs]
+(https://topoteretes.github.io/cognee) ### Run ``` import cognee text =
+"""Natural language processing (NLP) is an interdisciplinary subfield of
+computer science and information retrieval""" cognee.add(text) # Add a new
+piece of information cognee.cognify() # Use LLMs and cognee to create knowledge
+search_results = cognee.search("SIMILARITY", "computer science") # Query cognee
+for the knowledge for result_text in search_results[0]: print(result_text) ```
+Add alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
 dataset_name) ``` Or ``` cognee.add("data://{absolute_path_to_directory}",
 dataset_name) # This is useful if you have a directory with files organized in
 subdirectories. # You can target which directory to add by providing
 dataset_name. # Example: # root # / \ # reports bills # / \ # 2024 2023 # #
 cognee.add("data://{absolute_path_to_root}", "reports.2024") # This will add
 just directory 2024 under reports. ``` Read more [here](docs/index.md#run). ##
 Demo Check out our demo notebook [here](https://github.com/topoteretes/cognee/
-blob/main/notebooks/cognee%20-%20Get%20Started.ipynb) ## Architecture [[https:/
-/i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg]](https://youtu.be/-ARUfIzhzC4
-"Learn about cognee: 55") ### How Cognee Enhances Your Contextual Memory Our
-framework for the OpenAI, Graph (Neo4j) and Vector (Weaviate) databases
-introduces three key enhancements: - Query Classifiers: Navigate information
-graph using Pydantic OpenAI classifiers. - Document Topology: Structure and
-store documents in public and private domains. - Personalized Context: Provide
-a context object to the LLM for a better response. ![Image](assets/
-architecture.png)
+blob/main/notebooks/cognee%20-%20Get%20Started.ipynb) [[https://i3.ytimg.com/
+vi/-ARUfIzhzC4/maxresdefault.jpg]](https://www.youtube.com/watch?v=BDFt4xVPmro
+"Learn about cognee: 55") ## How it works ![Image](assets/architecture.png) ##
+ð It's alive
+Try it yourself on Whatsapp with one of our _p_a_r_t_n_e_r_s by typing `/save {content
+you want to save}` followed by `/query {knowledge you saved previously}` For
+more info here are the _d_o_c_s
```

