# Comparing `tmp/graphmemory-0.1.1.tar.gz` & `tmp/graphmemory-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphmemory-0.1.1.tar", last modified: Sat Jun  1 10:46:38 2024, max compression
+gzip compressed data, was "graphmemory-0.1.2.tar", last modified: Sun Jun  2 00:07:00 2024, max compression
```

## Comparing `graphmemory-0.1.1.tar` & `graphmemory-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-01 10:46:38.910670 graphmemory-0.1.1/
--rwxrwxrwx   0 brad      (1000) brad      (1000)     6311 2024-06-01 10:46:38.904822 graphmemory-0.1.1/PKG-INFO
--rwxrwxrwx   0 brad      (1000) brad      (1000)     6103 2024-06-01 10:14:20.000000 graphmemory-0.1.1/README.md
-drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-01 10:46:38.849652 graphmemory-0.1.1/graphmemory.egg-info/
--rwxrwxrwx   0 brad      (1000) brad      (1000)     6311 2024-06-01 10:46:38.000000 graphmemory-0.1.1/graphmemory.egg-info/PKG-INFO
--rwxrwxrwx   0 brad      (1000) brad      (1000)      268 2024-06-01 10:46:38.000000 graphmemory-0.1.1/graphmemory.egg-info/SOURCES.txt
--rwxrwxrwx   0 brad      (1000) brad      (1000)        1 2024-06-01 10:46:38.000000 graphmemory-0.1.1/graphmemory.egg-info/dependency_links.txt
--rwxrwxrwx   0 brad      (1000) brad      (1000)       16 2024-06-01 10:46:38.000000 graphmemory-0.1.1/graphmemory.egg-info/requires.txt
--rwxrwxrwx   0 brad      (1000) brad      (1000)        9 2024-06-01 10:46:38.000000 graphmemory-0.1.1/graphmemory.egg-info/top_level.txt
-drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-01 10:46:38.882159 graphmemory-0.1.1/graphrag/
--rwxrwxrwx   0 brad      (1000) brad      (1000)       76 2024-06-01 09:41:17.000000 graphmemory-0.1.1/graphrag/__init__.py
--rwxrwxrwx   0 brad      (1000) brad      (1000)    10700 2024-06-01 09:35:07.000000 graphmemory-0.1.1/graphrag/database.py
--rwxrwxrwx   0 brad      (1000) brad      (1000)      336 2024-05-31 23:56:06.000000 graphmemory-0.1.1/graphrag/models.py
--rwxrwxrwx   0 brad      (1000) brad      (1000)       38 2024-06-01 10:46:38.910670 graphmemory-0.1.1/setup.cfg
--rwxrwxrwx   0 brad      (1000) brad      (1000)      589 2024-06-01 10:45:50.000000 graphmemory-0.1.1/setup.py
-drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-01 10:46:38.892214 graphmemory-0.1.1/tests/
--rwxrwxrwx   0 brad      (1000) brad      (1000)    10996 2024-06-01 00:29:29.000000 graphmemory-0.1.1/tests/tests.py
+drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-02 00:07:00.287752 graphmemory-0.1.2/
+-rwxrwxrwx   0 brad      (1000) brad      (1000)      344 2024-06-02 00:07:00.281664 graphmemory-0.1.2/PKG-INFO
+-rwxrwxrwx   0 brad      (1000) brad      (1000)     6048 2024-06-01 17:44:07.000000 graphmemory-0.1.2/README.md
+drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-02 00:07:00.210530 graphmemory-0.1.2/graphmemory.egg-info/
+-rwxrwxrwx   0 brad      (1000) brad      (1000)      344 2024-06-02 00:06:59.000000 graphmemory-0.1.2/graphmemory.egg-info/PKG-INFO
+-rwxrwxrwx   0 brad      (1000) brad      (1000)      268 2024-06-02 00:07:00.000000 graphmemory-0.1.2/graphmemory.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brad      (1000) brad      (1000)        1 2024-06-02 00:06:59.000000 graphmemory-0.1.2/graphmemory.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brad      (1000) brad      (1000)       16 2024-06-02 00:06:59.000000 graphmemory-0.1.2/graphmemory.egg-info/requires.txt
+-rwxrwxrwx   0 brad      (1000) brad      (1000)        9 2024-06-02 00:06:59.000000 graphmemory-0.1.2/graphmemory.egg-info/top_level.txt
+drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-02 00:07:00.256214 graphmemory-0.1.2/graphrag/
+-rwxrwxrwx   0 brad      (1000) brad      (1000)       76 2024-06-01 09:41:17.000000 graphmemory-0.1.2/graphrag/__init__.py
+-rwxrwxrwx   0 brad      (1000) brad      (1000)    10700 2024-06-01 09:35:07.000000 graphmemory-0.1.2/graphrag/database.py
+-rwxrwxrwx   0 brad      (1000) brad      (1000)      336 2024-05-31 23:56:06.000000 graphmemory-0.1.2/graphrag/models.py
+-rwxrwxrwx   0 brad      (1000) brad      (1000)       38 2024-06-02 00:07:00.288464 graphmemory-0.1.2/setup.cfg
+-rwxrwxrwx   0 brad      (1000) brad      (1000)      593 2024-06-02 00:06:29.000000 graphmemory-0.1.2/setup.py
+drwxrwxrwx   0 brad      (1000) brad      (1000)        0 2024-06-02 00:07:00.268345 graphmemory-0.1.2/tests/
+-rwxrwxrwx   0 brad      (1000) brad      (1000)    10996 2024-06-01 00:29:29.000000 graphmemory-0.1.2/tests/tests.py
```

### Comparing `graphmemory-0.1.1/PKG-INFO` & `graphmemory-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,190 +1,172 @@
-Metadata-Version: 2.1
-Name: graphmemory
-Version: 0.1.1
-Summary: A package for creating a graph database for use with GraphRAG.
-Home-page: http://pypi.python.org/pypi/graphmemory/
-Author: BradAGI
-Author-email: cavemen_summary_0f@icloud.com
-License: LICENSE.txt
-Keywords: graphrag graph database rag
-Description-Content-Type: text/markdown
-Requires-Dist: duckdb
-Requires-Dist: pydantic
-
-# GraphMemory - GraphRAG Database
-
-## Overview
-This project provides an embedded graph database implementation with vector similarity search (VSS) using DuckDB. It includes a Python class `GraphRAG` for managing nodes and edges. 
-
-Each node has a unique ID, a JSON data field (any arbitrary dictionary), and a vector of floating point values. 
-
-Each edge has a unique ID, a source node ID, a target node ID, a relationship type, and a weight.
-
-This database can be used for any graph-based RAG application or knowledge graph application.
-
-Vector embeddings can be created using [sentence-transformers](https://www.sbert.net/) or other API based models.
-
-## Requirements
-- Python 3.x
-- DuckDB
-- Pydantic
-
-## Installation
-1. Clone the repository:
-    ```sh
-    git clone https://github.com/bradAGI/GraphMemory
-    ```
-2. Install the required packages:
-    ```sh
-    pip install -r requirements.txt
-    ```
-
-## Usage
-
-### GraphRAG Class
-The `GraphRAG` class provides methods to manage nodes and edges, perform bulk inserts, create indexes, and find nearest neighbors using vector similarity search.
-
-### Auto-Incrementing IDs
-If you do not provide an ID for a node or edge, the database will automatically assign a unique ID.
-
-### Example
-```python
-from graphrag.graphrag import GraphRAG
-from graphrag.models import Node, Edge
-
-
-# Initialize the database from disk (make sure to set vector_length correctly)
-graph_db = GraphRAG(database='graph.db', vector_length=3)
-
-# Insert nodes
-node1 = Node(data={"name": "George Washington", "role": "President"}, vector=[0.1, 0.2, 0.3])
-node1_id = graph_db.insert_node(node1)
-
-node2 = Node(data={"name": "Thomas Jefferson", "role": "Secretary of State"}, vector=[0.4, 0.5, 0.6])
-node2_id = graph_db.insert_node(node2)
-
-# Insert edge
-edge = Edge(source_id=node1_id, target_id=node2_id, relation="served_under", weight=0.5)
-graph_db.insert_edge(edge)
-
-# Print all nodes in the database
-nodes = graph_db.nodes_to_json()
-print("Nodes:", nodes)
-
-# Print all edges in the database
-edges = graph_db.edges_to_json()
-print("Edges:", edges)
-
-# Find connected nodes
-connected_nodes = graph_db.connected_nodes(node1_id)
-print("Connected Nodes:", connected_nodes)
-
-# Find nearest neighbors
-neighbors = graph_db.nearest_neighbors(vector=[0.1, 0.2, 0.3], limit=1)
-print("Nearest Neighbors:", neighbors)
-
-# Insert an edge between the two nodes with a relation
-edge = Edge(source_id=node1_id, target_id=node2_id, relation="served_under", weight=0.5)
-graph_db.insert_edge(edge)
-
-# Define the additional nodes for bulk insert
-nodes = [
-    Node(data={"name": "Alexander Hamilton", "role": "Secretary of the Treasury", "term": "1789–1795"}, vector=[0.7, 0.8, 0.9]),
-    Node(data={"name": "Oliver Wolcott Jr.", "role": "Secretary of the Treasury", "term": "1795–1797"}, vector=[1.6, 1.7, 1.8]),
-]
-
-# Bulk insert nodes
-graph_db.bulk_insert_nodes(nodes)
-
-# Define the additional edges for bulk insert
-edges = [
-    Edge(source_id=nodes[0].id, target_id=nodes[1].id, relation="succeeded_by", weight=0.7),
-    Edge(source_id=nodes[1].id, target_id=nodes[2].id, relation="succeeded_by", weight=0.8)
-]
-
-# Bulk insert edges
-graph_db.bulk_insert_edges(edges)
-
-# Delete a node
-graph_db.delete_node(nodes[-1].id)
-
-# Delete an edge
-graph_db.delete_edge(1, 2)
-
-# Find nearest nodes to a given vector by distance
-neighbors = graph_db.nearest_neighbors(vector=[0.1, 0.2, 0.3], limit=2)
-print("Nearest Neighbors:", neighbors)
-
-# Find connected nodes
-connected_nodes = graph_db.connected_nodes(nodes[1].id)
-print("Connected Nodes:", connected_nodes)
-```
-
-## GraphRAG Class Methods
-
-The `GraphRAG` class provides the following public methods for interacting with the graph database:
-
-1. `__init__(self, database=None, vector_length=3)`
-   - Initializes the database connection and sets up the database schema if necessary.
-
-2. `set_vector_length(self, vector_length)`
-   - Sets the length of the vectors for the nodes in the database.
-
-3. `create_tables(self)`
-   - Creates the necessary database tables for nodes and edges if they do not exist.
-
-4. `insert_node(self, node: Node) -> int`
-   - Inserts a node into the database and returns the node ID.
-
-5. `insert_edge(self, edge: Edge)`
-   - Inserts an edge between two nodes in the database.
-
-6. `bulk_insert_nodes(self, nodes: List[Node]) -> List[Node]`
-   - Performs a bulk insert of multiple nodes into the database.
-
-7. `bulk_insert_edges(self, edges: List[Edge])`
-   - Performs a bulk insert of multiple edges into the database.
-
-8. `delete_node(self, node_id: int)`
-   - Deletes a node and its associated edges from the database.
-
-9. `delete_edge(self, source_id: int, target_id: int)`
-   - Deletes an edge from the database.
-
-10. `create_index(self)`
-    - Creates an index on the node vectors to improve search performance.
-
-11. `nearest_neighbors(self, vector: List[float], limit: int) -> List[Neighbor]`
-    - Finds and returns the nearest neighbor nodes based on vector similarity.
-
-12. `connected_nodes(self, node_id: int) -> List[Node]`
-    - Retrieves all nodes directly connected to the specified node.
-
-13. `nodes_to_json(self)`
-    - Returns a JSON representation of all nodes in the database.
-
-14. `edges_to_json(self)`
-    - Returns a JSON representation of all edges in the database.
-
-15. `get_node(self, node_id: int)`
-    - Retrieves a specific node by its ID.
-
-16. `print_json(self)`
-    - Prints the JSON representation of all nodes and edges in the database.
-
-These methods facilitate the management and querying of the graph database, allowing for efficient data handling and retrieval.
-
-## Testing
-Unit tests are provided in `tests/tests.py`.
-
-### Running Tests
-To run the unit tests, use the following command:
-```sh
-python -m unittest discover -s tests
-```
-
-## License
-This project is licensed under the MIT License. See the LICENSE file for details.
-
-## Contributing
-Contributions are welcome! Please open an issue or submit a pull request.
+# GraphMemory - GraphRAG Database
+
+## Overview
+This project provides an embedded graph database implementation with vector similarity search (VSS) using DuckDB. It includes a Python class `GraphRAG` for managing nodes and edges. 
+
+Each node has a unique ID, a JSON data field (any arbitrary dictionary), and a vector of floating point values. 
+
+Each edge has a unique ID, a source node ID, a target node ID, a relationship type, and a weight.
+
+This database can be used for any graph-based RAG application or knowledge graph application.
+
+Vector embeddings can be created using [sentence-transformers](https://www.sbert.net/) or other API based models.
+
+## Installation
+1. Clone the repository:
+    ```sh
+    git clone https://github.com/bradAGI/GraphMemory
+    ```
+2. Install the required packages:
+    ```sh
+    pip install -r requirements.txt
+    ```
+
+## Usage
+
+### GraphRAG Class
+The `GraphRAG` class provides methods to manage nodes and edges, perform bulk inserts, create indexes, and find nearest neighbors using vector similarity search.
+
+### Auto-Incrementing IDs
+If you do not provide an ID for a node or edge, the database will automatically assign a unique ID.
+
+### Example
+```python
+from graphrag.graphrag import GraphRAG
+from graphrag.models import Node, Edge
+
+
+# Initialize the database from disk (make sure to set vector_length correctly)
+graph_db = GraphRAG(database='graph.db', vector_length=3)
+
+# Insert nodes
+node1 = Node(data={"name": "George Washington", "role": "President"}, vector=[0.1, 0.2, 0.3])
+node1_id = graph_db.insert_node(node1)
+
+node2 = Node(data={"name": "Thomas Jefferson", "role": "Secretary of State"}, vector=[0.4, 0.5, 0.6])
+node2_id = graph_db.insert_node(node2)
+
+# Insert edge
+edge = Edge(source_id=node1_id, target_id=node2_id, relation="served_under", weight=0.5)
+graph_db.insert_edge(edge)
+
+# Print all nodes in the database
+nodes = graph_db.nodes_to_json()
+print("Nodes:", nodes)
+
+# Print all edges in the database
+edges = graph_db.edges_to_json()
+print("Edges:", edges)
+
+# Find connected nodes
+connected_nodes = graph_db.connected_nodes(node1_id)
+print("Connected Nodes:", connected_nodes)
+
+# Find nearest neighbors
+neighbors = graph_db.nearest_neighbors(vector=[0.1, 0.2, 0.3], limit=1)
+print("Nearest Neighbors:", neighbors)
+
+# Insert an edge between the two nodes with a relation
+edge = Edge(source_id=node1_id, target_id=node2_id, relation="served_under", weight=0.5)
+graph_db.insert_edge(edge)
+
+# Define the additional nodes for bulk insert
+nodes = [
+    Node(data={"name": "Alexander Hamilton", "role": "Secretary of the Treasury", "term": "1789–1795"}, vector=[0.7, 0.8, 0.9]),
+    Node(data={"name": "Oliver Wolcott Jr.", "role": "Secretary of the Treasury", "term": "1795–1797"}, vector=[1.6, 1.7, 1.8]),
+]
+
+# Bulk insert nodes
+graph_db.bulk_insert_nodes(nodes)
+
+# Define the additional edges for bulk insert
+edges = [
+    Edge(source_id=nodes[0].id, target_id=nodes[1].id, relation="succeeded_by", weight=0.7),
+    Edge(source_id=nodes[1].id, target_id=nodes[2].id, relation="succeeded_by", weight=0.8)
+]
+
+# Bulk insert edges
+graph_db.bulk_insert_edges(edges)
+
+# Delete a node
+graph_db.delete_node(nodes[-1].id)
+
+# Delete an edge
+graph_db.delete_edge(1, 2)
+
+# Find nearest nodes to a given vector by distance
+neighbors = graph_db.nearest_neighbors(vector=[0.1, 0.2, 0.3], limit=2)
+print("Nearest Neighbors:", neighbors)
+
+# Find connected nodes
+connected_nodes = graph_db.connected_nodes(nodes[1].id)
+print("Connected Nodes:", connected_nodes)
+```
+
+## GraphRAG Class Methods
+
+The `GraphRAG` class provides the following public methods for interacting with the graph database:
+
+1. `__init__(self, database=None, vector_length=3)`
+   - Initializes the database connection and sets up the database schema if necessary.
+
+2. `set_vector_length(self, vector_length)`
+   - Sets the length of the vectors for the nodes in the database.
+
+3. `create_tables(self)`
+   - Creates the necessary database tables for nodes and edges if they do not exist.
+
+4. `insert_node(self, node: Node) -> int`
+   - Inserts a node into the database and returns the node ID.
+
+5. `insert_edge(self, edge: Edge)`
+   - Inserts an edge between two nodes in the database.
+
+6. `bulk_insert_nodes(self, nodes: List[Node]) -> List[Node]`
+   - Performs a bulk insert of multiple nodes into the database.
+
+7. `bulk_insert_edges(self, edges: List[Edge])`
+   - Performs a bulk insert of multiple edges into the database.
+
+8. `delete_node(self, node_id: int)`
+   - Deletes a node and its associated edges from the database.
+
+9. `delete_edge(self, source_id: int, target_id: int)`
+   - Deletes an edge from the database.
+
+10. `create_index(self)`
+    - Creates an index on the node vectors to improve search performance.
+
+11. `nearest_neighbors(self, vector: List[float], limit: int) -> List[Neighbor]`
+    - Finds and returns the nearest neighbor nodes based on vector similarity.
+
+12. `connected_nodes(self, node_id: int) -> List[Node]`
+    - Retrieves all nodes directly connected to the specified node.
+
+13. `nodes_to_json(self)`
+    - Returns a JSON representation of all nodes in the database.
+
+14. `edges_to_json(self)`
+    - Returns a JSON representation of all edges in the database.
+
+15. `get_node(self, node_id: int)`
+    - Retrieves a specific node by its ID.
+
+16. `print_json(self)`
+    - Prints the JSON representation of all nodes and edges in the database.
+
+These methods facilitate the management and querying of the graph database, allowing for efficient data handling and retrieval.
+
+## Testing
+Unit tests are provided in `tests/tests.py`.
+
+### Running Tests
+To run the unit tests, use the following command:
+```sh
+python -m unittest discover -s tests
+```
+
+## License
+This project is licensed under the MIT License. See the LICENSE file for details.
+
+## Contributing
+Contributions are welcome! Please open an issue or submit a pull request.
```

### Comparing `graphmemory-0.1.1/graphrag/database.py` & `graphmemory-0.1.2/graphrag/database.py`

 * *Files identical despite different names*

### Comparing `graphmemory-0.1.1/setup.py` & `graphmemory-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='graphmemory',
-    version='0.1.1',
+    version='0.1.2',
     author='BradAGI',
     author_email='cavemen_summary_0f@icloud.com',
     packages=find_packages(),
     url='http://pypi.python.org/pypi/graphmemory/',
     license='LICENSE.txt',
     description='A package for creating a graph database for use with GraphRAG.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
+    # long_description=open('README.md').read(),
+    # long_description_content_type='text/markdown',
     install_requires=[
         'duckdb',
         'pydantic'
     ],
     keywords='graphrag graph database rag'
 )
```

### Comparing `graphmemory-0.1.1/tests/tests.py` & `graphmemory-0.1.2/tests/tests.py`

 * *Files identical despite different names*

