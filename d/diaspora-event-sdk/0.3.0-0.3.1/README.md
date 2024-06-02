# Comparing `tmp/diaspora-event-sdk-0.3.0.tar.gz` & `tmp/diaspora-event-sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.3.0.tar", last modified: Sat Jun  1 20:12:13 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.3.1.tar", last modified: Sun Jun  2 14:54:52 2024, max compression
```

## Comparing `diaspora-event-sdk-0.3.0.tar` & `diaspora-event-sdk-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.012838 diaspora-event-sdk-0.3.0/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-06-01 20:12:13.012714 diaspora-event-sdk-0.3.0/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-15 22:04:54.000000 diaspora-event-sdk-0.3.0/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.008702 diaspora-event-sdk-0.3.0/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.010116 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      640 2024-06-01 20:11:52.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     3942 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/aws_iam_msk.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.011065 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)    18699 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/auth.py
--rw-r--r--   0 haochen    (501) staff       (20)     9344 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/awsrequest.py
--rw-r--r--   0 haochen    (501) staff       (20)    11197 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/compat.py
--rw-r--r--   0 haochen    (501) staff       (20)     2455 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/credentials.py
--rw-r--r--   0 haochen    (501) staff       (20)     2002 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/exceptions.py
--rw-r--r--   0 haochen    (501) staff       (20)     5370 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/utils.py
--rw-r--r--   0 haochen    (501) staff       (20)     8625 2024-06-01 20:11:52.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4286 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.012165 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-05-15 22:04:54.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1013 2024-06-01 20:11:52.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-05-15 22:04:54.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-05-15 22:04:54.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.012354 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     4793 2024-06-01 20:11:52.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-06-01 20:11:52.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.009261 diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-06-01 20:12:12.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1412 2024-06-01 20:12:12.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-06-01 20:12:12.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      110 2024-06-01 20:12:12.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-06-01 20:12:12.000000 diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-06-01 20:12:13.012888 diaspora-event-sdk-0.3.0/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1358 2024-05-17 12:50:50.000000 diaspora-event-sdk-0.3.0/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.012457 diaspora-event-sdk-0.3.0/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.3.0/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-06-01 20:12:13.012542 diaspora-event-sdk-0.3.0/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-05-15 22:04:54.000000 diaspora-event-sdk-0.3.0/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-05-15 22:04:54.000000 diaspora-event-sdk-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.451977 diaspora-event-sdk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-06-02 14:54:52.451977 diaspora-event-sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.447977 diaspora-event-sdk-0.3.1/diaspora_event_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.447977 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/aws_iam_msk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.447977 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18699 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.447977 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.451977 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.447977 diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-06-02 14:54:52.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-02 14:54:52.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:54:52.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-02 14:54:52.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 14:54:52.000000 diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:54:52.451977 diaspora-event-sdk-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.451977 diaspora-event-sdk-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:54:52.451977 diaspora-event-sdk-0.3.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/tests/unit/apis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/tests/unit/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-02 14:54:45.000000 diaspora-event-sdk-0.3.1/tox.ini
```

### Comparing `diaspora-event-sdk-0.3.0/LICENSE` & `diaspora-event-sdk-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `diaspora-event-sdk-0.3.0/PKG-INFO` & `diaspora-event-sdk-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: Apache 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
 License-File: LICENSE
 
-# Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
+# Diaspora Event Fabric SDK
 
-## Event Fabric SDK Installation Guide
-### Recommended Method: Use with `kafka-python`
-For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
-
-To install the Event Fabric SDK and `kafka-python,` with the following command:
+## Installation Guide
+### Recommended Method: With `kafka-python`
+To integrate with Diaspora Event Fabric using `KafkaProducer` and `KafkaConsumer`, install the SDK with `kafka-python`:
 ```bash
 pip install "diaspora-event-sdk[kafka-python]"
 ```
 
 ### Alternative Installation: Without Kafka Client Library
-To use alternative Kafka client libraries (e.g., `confluent-kafka-python`, `aiokafka`, and libraries for other programming laguages), you can install the SDK without the `kafka-python` dependency. This option still provides topic-level access control (authorization) and login credential management features.
-
-To install the SDK without `kafka-python`, use:
+For other Kafka client libraries (e.g., `confluent-kafka-python`, `aiokafka`), install the SDK without `kafka-python`:
 ```bash
 pip install diaspora-event-sdk
 ```
-Note: This method does not include dependencies for `KafkaProducer` and `KafkaConsumer` classes mentioned in the QuickStart
-
-## Use Diaspora Event Fabric SDK
-
-**Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
+Note: This does not include `KafkaProducer` and `KafkaConsumer` dependencies.
 
-**Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
+## Using Diaspora Event Fabric SDK
+Check our [Notebook](DiasporaDemo.ipynb) for a quickstart and demonstration.
 
-**Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
+<!-- **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
-**Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+**Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively. -->
 
+<!-- **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust. -->
 
+<!-- **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration. -->
```

### Comparing `diaspora-event-sdk-0.3.0/README.md` & `diaspora-event-sdk-0.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-# Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
+# Diaspora Event Fabric SDK
 
-## Event Fabric SDK Installation Guide
-### Recommended Method: Use with `kafka-python`
-For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
-
-To install the Event Fabric SDK and `kafka-python,` with the following command:
+## Installation Guide
+### Recommended Method: With `kafka-python`
+To integrate with Diaspora Event Fabric using `KafkaProducer` and `KafkaConsumer`, install the SDK with `kafka-python`:
 ```bash
 pip install "diaspora-event-sdk[kafka-python]"
 ```
 
 ### Alternative Installation: Without Kafka Client Library
-To use alternative Kafka client libraries (e.g., `confluent-kafka-python`, `aiokafka`, and libraries for other programming laguages), you can install the SDK without the `kafka-python` dependency. This option still provides topic-level access control (authorization) and login credential management features.
-
-To install the SDK without `kafka-python`, use:
+For other Kafka client libraries (e.g., `confluent-kafka-python`, `aiokafka`), install the SDK without `kafka-python`:
 ```bash
 pip install diaspora-event-sdk
 ```
-Note: This method does not include dependencies for `KafkaProducer` and `KafkaConsumer` classes mentioned in the QuickStart
+Note: This does not include `KafkaProducer` and `KafkaConsumer` dependencies.
 
-## Use Diaspora Event Fabric SDK
+## Using Diaspora Event Fabric SDK
+Check our [Notebook](DiasporaDemo.ipynb) for a quickstart and demonstration.
 
-**Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
+<!-- **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
-**Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
+**Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively. -->
 
-**Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
+<!-- **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust. -->
 
-**Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+<!-- **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration. -->
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/_environments.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/_environments.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 # TOKEN_EXCHANGE = "http://3.220.110.101/"
 DIASPORA_RESOURCE_SERVER = "2b9d2f5c-fa32-45b5-875b-b24cd343b917"
 
 
 def _get_envname():
     return os.getenv("DIASPORA_SDK_ENVIRONMENT", "production")
 
+
 def get_web_service_url(envname: Union[str, None] = None) -> str:
     env = envname or _get_envname()
     urls = {
         "production": "https://diaspora-web-service.ml22sevubfnks.us-east-1.cs.amazonlightsail.com",
         "dev": "https://diaspora-web-service-dev.ml22sevubfnks.us-east-1.cs.amazonlightsail.com",
         "local": "http://localhost:8000",
+        "legacy": "http://3.220.110.101/",
     }
 
     return urls.get(env, urls["production"])
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/aws_iam_msk.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/aws_iam_msk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 #  Copyright 2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 
 import base64
+
 # import logging
 from datetime import datetime, timezone
 from urllib.parse import parse_qs, urlparse
 
 # import boto3
 # import botocore.session
 # import pkg_resources
 from .botocore.auth import SigV4QueryAuth
 from .botocore.awsrequest import AWSRequest
+
 # from botocore.config import Config
 from .botocore.credentials import Credentials
 
 ENDPOINT_URL_TEMPLATE = "https://kafka.{}.amazonaws.com/"
 DEFAULT_TOKEN_EXPIRY_SECONDS = 900
 DEFAULT_STS_SESSION_NAME = "MSKSASLDefaultSession"
 ACTION_TYPE = "Action"
 ACTION_NAME = "kafka-cluster:Connect"
 SIGNING_NAME = "kafka-cluster"
 USER_AGENT_KEY = "User-Agent"
 LIB_NAME = "aws-msk-iam-sasl-signer-python"
 
 
 def __get_user_agent__():
-    return (f"{LIB_NAME}/1.0.1")
+    return f"{LIB_NAME}/1.0.1"
 
 
 def __get_expiration_time_ms(request):
     """
     Private function that parses the url and gets the expiration time
 
     Args: request (AWSRequest): The signed aws request object
     """
     # Parse the signed request
     parsed_url = urlparse(request.url)
     parsed_ul_params = parse_qs(parsed_url.query)
-    parsed_signing_time = datetime.strptime(parsed_ul_params['X-Amz-Date'][0],
-                                            "%Y%m%dT%H%M%SZ")
+    parsed_signing_time = datetime.strptime(
+        parsed_ul_params["X-Amz-Date"][0], "%Y%m%dT%H%M%SZ"
+    )
 
     # Make the datetime object timezone-aware
     signing_time = parsed_signing_time.replace(tzinfo=timezone.utc)
 
     # Convert the Unix timestamp to milliseconds
-    expiration_timestamp_seconds = int(
-        signing_time.timestamp()) + DEFAULT_TOKEN_EXPIRY_SECONDS
+    expiration_timestamp_seconds = (
+        int(signing_time.timestamp()) + DEFAULT_TOKEN_EXPIRY_SECONDS
+    )
 
     # Get lifetime of token
     expiration_timestamp_ms = expiration_timestamp_seconds * 1000
 
     return expiration_timestamp_ms
 
 
@@ -70,16 +74,15 @@
     endpoint_url = ENDPOINT_URL_TEMPLATE.format(region)
 
     # Set up resource path and query parameters
     query_params = {ACTION_TYPE: ACTION_NAME}
 
     # Create SigV4 instance
     sig_v4 = SigV4QueryAuth(
-        aws_credentials, SIGNING_NAME, region,
-        expires=DEFAULT_TOKEN_EXPIRY_SECONDS
+        aws_credentials, SIGNING_NAME, region, expires=DEFAULT_TOKEN_EXPIRY_SECONDS
     )
 
     # Create request with url and parameters
     request = AWSRequest(method="GET", url=endpoint_url, params=query_params)
 
     # Add auth to the request and prepare the request
     sig_v4.add_auth(request)
@@ -106,14 +109,16 @@
         region (str): The AWS region where the cluster is located.
     Returns:
         str: A base64-encoded authorization token.
     """
 
     # Load credentials
     import os
+
     assert os.environ["AWS_ACCESS_KEY_ID"]
     assert os.environ["AWS_SECRET_ACCESS_KEY"]
 
-    aws_credentials = Credentials(os.environ["AWS_ACCESS_KEY_ID"],
-                                  os.environ["AWS_SECRET_ACCESS_KEY"])
+    aws_credentials = Credentials(
+        os.environ["AWS_ACCESS_KEY_ID"], os.environ["AWS_SECRET_ACCESS_KEY"]
+    )
 
     return __construct_auth_token(region, aws_credentials)
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/auth.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/auth.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/awsrequest.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/compat.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/compat.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/credentials.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/credentials.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/exceptions.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/exceptions.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/botocore/utils.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         # but if login handling is implicit (as when no login manager is passed)
         # then ensure that the user is logged in
         else:
             self.login_manager = LoginManager(environment=environment)
             self.login_manager.ensure_logged_in()
 
         self.web_client = self.login_manager.get_web_client(
-            base_url=self.web_service_address)
+            base_url=self.web_service_address
+        )
         self.auth_client = self.login_manager.get_auth_client()
         self.subject_openid = self.auth_client.oauth2_userinfo()["sub"]
 
     def logout(self):
         """Remove credentials from your local system"""
         self.login_manager.logout()
 
@@ -149,36 +150,42 @@
         return self.web_client.update_topic_configs(self.subject_openid, topic, configs)
 
     @requires_login
     def update_topic_partitions(self, topic, new_partitions):
         """
         Increases the number of partitions for a given topic to the specified new partition count.
         """
-        return self.web_client.update_topic_partitions(self.subject_openid, topic, new_partitions)
+        return self.web_client.update_topic_partitions(
+            self.subject_openid, topic, new_partitions
+        )
 
     @requires_login
     def reset_topic(self, topic):
         """
         Deletes and recreates the topic, removing all messages and restoring the topic to the default configurations while user access is not affected.
         """
         return self.web_client.reset_topic(self.subject_openid, topic)
 
     @requires_login
     def grant_user_access(self, topic, user):
         """
         Authorizes another user to access a registered topic under the invoker's account.
         """
-        return self.web_client.grant_user_access(self.subject_openid, topic, user, "grant")
+        return self.web_client.grant_user_access(
+            self.subject_openid, topic, user, "grant"
+        )
 
     @requires_login
     def revoke_user_access(self, topic, user):
         """
         Removes access permissions for another user from a registered topic under the invoker's account.
         """
-        return self.web_client.grant_user_access(self.subject_openid, topic, user, "revoke")
+        return self.web_client.grant_user_access(
+            self.subject_openid, topic, user, "revoke"
+        )
 
     @requires_login
     def list_topic_users(self, topic):
         """
         Returns a list of users that have access to the topic.
         """
         return self.web_client.list_topic_users(self.subject_openid, topic)
@@ -189,42 +196,49 @@
         Retrieves a list of triggers associated created under the user's account, showing each trigger's configurations and UUID.
         """
         return self.web_client.list_triggers(self.subject_openid)
 
     @requires_login
     def create_trigger(self, topic, function, function_configs, trigger_configs):
         """
-        Creates a new trigger under the user's account with specific function and invocation configurations. 
+        Creates a new trigger under the user's account with specific function and invocation configurations.
         """
         return self.web_client.create_trigger(
-            self.subject_openid, topic, function, "create", function_configs, trigger_configs)
+            self.subject_openid,
+            topic,
+            function,
+            "create",
+            function_configs,
+            trigger_configs,
+        )
 
     @requires_login
     def delete_trigger(self, topic, function):
         """
         Deletes a trigger and related AWS resources, while the associated topic remains unaffected.
         """
         return self.web_client.create_trigger(
-            self.subject_openid, topic, function, "delete", {}, {})
+            self.subject_openid, topic, function, "delete", {}, {}
+        )
 
     @requires_login
     def update_trigger(self, trigger_uuid, trigger_configs):
         """
         Updates invocation configurations of an existing trigger, identified by its unique trigger UUID.
         """
-        return self.web_client.update_trigger(self.subject_openid, trigger_uuid, trigger_configs)
+        return self.web_client.update_trigger(
+            self.subject_openid, trigger_uuid, trigger_configs
+        )
 
     @requires_login
     def list_log_streams(self, trigger):
         """
         List log streams of a trigger under the user's account
         """
-        return self.web_client.list_log_streams(
-            self.subject_openid, trigger)
+        return self.web_client.list_log_streams(self.subject_openid, trigger)
 
     @requires_login
     def get_log_events(self, trigger, stream):
         """
         Get events in a particular log stream of a trigger under the user's account
         """
-        return self.web_client.get_log_events(
-            self.subject_openid, trigger, stream)
+        return self.web_client.get_log_events(self.subject_openid, trigger, stream)
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from kafka import KafkaConsumer as KCons  # type: ignore[import,import-not-found]
     import os
 
     class MSKTokenProvider:
         def token(self):
             token, _ = generate_auth_token("us-east-1")
             return token
-except Exception as e:
+except Exception:
     kafka_available = False
 
 
 def get_diaspora_config(extra_configs: Dict[str, Any] = {}) -> Dict[str, Any]:
     """
     Retrieve default Diaspora event fabric connection configurations for Kafka clients.
     Merges default configurations with custom ones provided.
@@ -86,28 +86,28 @@
         try:
             producer = KafkaProducer(max_block_ms=10 * 1000)
             future = producer.send(
                 topic="__connection_test",
                 value={"message": "Synchronous message from Diaspora SDK"},
             )
             result["producer_connection_test"] = future.get(timeout=10)
-        except Exception as e:
+        except Exception:
             pass
 
     def consumer_connection_test(result):
         try:
             consumer = KafkaConsumer(
                 "__connection_test",
                 consumer_timeout_ms=10 * 1000,
                 auto_offset_reset="earliest",
             )
             for msg in consumer:
                 result["consumer_connection_test"] = msg
                 break
-        except Exception as e:
+        except Exception:
             pass
 
     result, retry_count = {}, 0
     start_time = time.time()
     while len(result) < 2:  # two tests
         if retry_count > 0:
             print(
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Logic for using client identities with the Diaspora SDK
 
 The design is based on the Globus CLI client login:
 https://github.com/globus/globus-cli/blob/main/src/globus_cli/login_manager/client_login.py
 """
+
 from __future__ import annotations
 
 import logging
 import os
 import uuid
 from typing import Union
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -28,8 +28,8 @@
         )
     )
 
     # come back with auth code
     auth_code = input("Enter the resulting Authorization Code here: ").strip()
 
     # finish auth flow
-    return auth_client.oauth2_exchange_code_for_tokens(auth_code)
+    return auth_client.oauth2_exchange_code_for_tokens(auth_code)
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
-import json
 import os
 import pathlib
 
 from globus_sdk.tokenstorage import SQLiteAdapter
 
 from .._environments import _get_envname
 from .client_login import get_client_login, is_client_login
-from .globus_auth import internal_auth_client
 
 
 def _home() -> pathlib.Path:
     # this is a hook point for tests to patch over
     # it just returns `pathlib.Path.home()`
     # replace this with a mock to return some test directory
     return pathlib.Path.home()
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk/sdk/web_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,106 +32,124 @@
         return self.get("/api/v2/topics", headers={"Subject": str(subject)})
 
     def register_topic(
         self, subject: UUID_LIKE_T, topic: str, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.put(
             f"/api/v2/topic/{topic}",
-            headers={"Subject": str(subject), "Action": action}
+            headers={"Subject": str(subject), "Action": action},
         )
 
     def get_topic_configs(
         self, subject: UUID_LIKE_T, topic: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(
-            f"/api/v2/topic/{topic}",
-            headers={"Subject": str(subject), "Topic": topic}
+            f"/api/v2/topic/{topic}", headers={"Subject": str(subject), "Topic": topic}
         )
 
     def update_topic_configs(
         self, subject: UUID_LIKE_T, topic: str, configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}",
-            headers={"Subject": str(subject), "Topic": topic,
-                     "Content-Type": "text/plain"},
-            data=json.dumps(configs).encode("utf-8")
+            headers={
+                "Subject": str(subject),
+                "Topic": topic,
+                "Content-Type": "text/plain",
+            },
+            data=json.dumps(configs).encode("utf-8"),
         )
 
     def update_topic_partitions(
         self, subject: UUID_LIKE_T, topic: str, new_partitions: int
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/partitions",
-            headers={"Subject": str(subject), "Topic": topic,
-                     "NewPartitions": str(new_partitions)}
+            headers={
+                "Subject": str(subject),
+                "Topic": topic,
+                "NewPartitions": str(new_partitions),
+            },
         )
 
     def reset_topic(
         self, subject: UUID_LIKE_T, topic: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/reset",
-            headers={"Subject": str(subject),
-                     "Topic": topic}
+            headers={"Subject": str(subject), "Topic": topic},
         )
 
     def grant_user_access(
         self, subject: UUID_LIKE_T, topic: str, user: UUID_LIKE_T, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/user",
-            headers={"Subject": str(subject), "Action": action,
-                     "Topic": topic, "User": str(user)}
+            headers={
+                "Subject": str(subject),
+                "Action": action,
+                "Topic": topic,
+                "User": str(user),
+            },
         )
 
     def list_topic_users(
         self, subject: UUID_LIKE_T, topic: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(
             f"/api/v2/topic/{topic}/users",
-            headers={"Subject": str(subject),
-                     "Topic": topic}
+            headers={"Subject": str(subject), "Topic": topic},
         )
 
     def list_triggers(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.get("/api/v2/triggers", headers={"Subject": str(subject)})
 
     def create_trigger(
-        self, subject: UUID_LIKE_T, topic: str, function: str, action: str,
-        function_configs: dict, trigger_configs: dict
+        self,
+        subject: UUID_LIKE_T,
+        topic: str,
+        function: str,
+        action: str,
+        function_configs: dict,
+        trigger_configs: dict,
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.put(
             "/api/v2/trigger",
-            headers={"Subject": str(subject), "Topic": topic,
-                     "Trigger": function, "Action": action,
-                     "Content-Type": "text/plain"},
-            data=json.dumps({"function": function_configs,
-                             "trigger": trigger_configs}).encode("utf-8")
+            headers={
+                "Subject": str(subject),
+                "Topic": topic,
+                "Trigger": function,
+                "Action": action,
+                "Content-Type": "text/plain",
+            },
+            data=json.dumps(
+                {"function": function_configs, "trigger": trigger_configs}
+            ).encode("utf-8"),
         )
 
     def update_trigger(
         self, subject: UUID_LIKE_T, trigger_uuid: UUID_LIKE_T, trigger_configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/triggers/{trigger_uuid}",
-            headers={"Subject": str(subject), "Trigger_id": str(trigger_uuid),
-                     "Content-Type": "text/plain"},
-            data=json.dumps(trigger_configs).encode("utf-8")
+            headers={
+                "Subject": str(subject),
+                "Trigger_id": str(trigger_uuid),
+                "Content-Type": "text/plain",
+            },
+            data=json.dumps(trigger_configs).encode("utf-8"),
         )
 
     def list_log_streams(
         self, subject: UUID_LIKE_T, trigger: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(
-            f"/api/v2/logs",
-            headers={"Subject": str(subject), "Trigger": trigger}
+            "/api/v2/logs", headers={"Subject": str(subject), "Trigger": trigger}
         )
 
     def get_log_events(
         self, subject: UUID_LIKE_T, trigger: str, stream: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(
-            f"/api/v2/log",
-            headers={"Subject": str(subject), "Trigger": trigger,
-                     "Stream": stream}
+            "/api/v2/log",
+            headers={"Subject": str(subject), "Trigger": trigger, "Stream": stream},
         )
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: Apache 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
 License-File: LICENSE
 
-# Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
+# Diaspora Event Fabric SDK
 
-## Event Fabric SDK Installation Guide
-### Recommended Method: Use with `kafka-python`
-For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
-
-To install the Event Fabric SDK and `kafka-python,` with the following command:
+## Installation Guide
+### Recommended Method: With `kafka-python`
+To integrate with Diaspora Event Fabric using `KafkaProducer` and `KafkaConsumer`, install the SDK with `kafka-python`:
 ```bash
 pip install "diaspora-event-sdk[kafka-python]"
 ```
 
 ### Alternative Installation: Without Kafka Client Library
-To use alternative Kafka client libraries (e.g., `confluent-kafka-python`, `aiokafka`, and libraries for other programming laguages), you can install the SDK without the `kafka-python` dependency. This option still provides topic-level access control (authorization) and login credential management features.
-
-To install the SDK without `kafka-python`, use:
+For other Kafka client libraries (e.g., `confluent-kafka-python`, `aiokafka`), install the SDK without `kafka-python`:
 ```bash
 pip install diaspora-event-sdk
 ```
-Note: This method does not include dependencies for `KafkaProducer` and `KafkaConsumer` classes mentioned in the QuickStart
-
-## Use Diaspora Event Fabric SDK
-
-**Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
+Note: This does not include `KafkaProducer` and `KafkaConsumer` dependencies.
 
-**Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
+## Using Diaspora Event Fabric SDK
+Check our [Notebook](DiasporaDemo.ipynb) for a quickstart and demonstration.
 
-**Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
+<!-- **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
-**Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+**Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively. -->
 
+<!-- **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust. -->
 
+<!-- **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration. -->
```

### Comparing `diaspora-event-sdk-0.3.0/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.3.1/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+mypy.ini
 setup.py
 tox.ini
 diaspora_event_sdk/__init__.py
 diaspora_event_sdk/version.py
 diaspora_event_sdk.egg-info/PKG-INFO
 diaspora_event_sdk.egg-info/SOURCES.txt
 diaspora_event_sdk.egg-info/dependency_links.txt
@@ -31,8 +32,9 @@
 diaspora_event_sdk/sdk/login_manager/login_flow.py
 diaspora_event_sdk/sdk/login_manager/manager.py
 diaspora_event_sdk/sdk/login_manager/protocol.py
 diaspora_event_sdk/sdk/login_manager/tokenstore.py
 diaspora_event_sdk/sdk/utils/__init__.py
 diaspora_event_sdk/sdk/utils/uuid_like.py
 tests/__init__.py
-tests/unit/test_client.py
+tests/unit/apis_test.py
+tests/unit/client_test.py
```

### Comparing `diaspora-event-sdk-0.3.0/setup.py` & `diaspora-event-sdk-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import os
 import re
 from pathlib import Path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-TEST_REQUIRES = ["pytest", "pytest-cov", "coverage", "mypy", "tox", "check-manifest"]
+TEST_REQUIRES = [
+    "pytest",
+    "pytest-cov",
+    "coverage",
+    "mypy",
+    "tox",
+    "check-manifest",
+    "pre-commit",
+]
 
 
 def parse_version():
     # single source of truth for package version
     version_string = ""
     version_pattern = re.compile(r'__version__ = "([^"]*)"')
     with open(os.path.join("diaspora_event_sdk", "version.py")) as f:
```

### Comparing `diaspora-event-sdk-0.3.0/tests/unit/test_client.py` & `diaspora-event-sdk-0.3.1/tests/unit/client_test.py`

 * *Files identical despite different names*

