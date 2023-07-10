# Comparing `tmp/mlflow_knative-0.2.0.tar.gz` & `tmp/mlflow_knative-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_knative-0.2.0.tar", max compression
+gzip compressed data, was "mlflow_knative-0.3.0.tar", max compression
```

## Comparing `mlflow_knative-0.2.0.tar` & `mlflow_knative-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1085 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     5315 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/README.md
--rw-r--r--   0        0        0      526 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/mlflow_knative/__init__.py
--rw-r--r--   0        0        0    15280 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/mlflow_knative/deployment_client.py
--rw-r--r--   0        0        0     5799 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/mlflow_knative/knative.py
--rw-r--r--   0        0        0     2232 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/mlflow_knative/mlflow_docker.py
--rw-r--r--   0        0        0      808 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/mlflow_knative/service.yaml
--rw-r--r--   0        0        0     1089 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/mlflow_knative/templating.py
--rw-r--r--   0        0        0     1617 2023-07-08 02:32:58.000000 mlflow_knative-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 mlflow_knative-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     5315 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/README.md
+-rw-r--r--   0        0        0      526 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/__init__.py
+-rw-r--r--   0        0        0    15767 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/deployment_client.py
+-rw-r--r--   0        0        0     6330 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/knative.py
+-rw-r--r--   0        0        0     2232 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/mlflow_docker.py
+-rw-r--r--   0        0        0      808 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/service.yaml
+-rw-r--r--   0        0        0     1089 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/mlflow_knative/templating.py
+-rw-r--r--   0        0        0     1616 2023-07-10 14:11:48.000000 mlflow_knative-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6158 1970-01-01 00:00:00.000000 mlflow_knative-0.3.0/PKG-INFO
```

### Comparing `mlflow_knative-0.2.0/LICENSE.md` & `mlflow_knative-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.2.0/README.md` & `mlflow_knative-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.2.0/mlflow_knative/__init__.py` & `mlflow_knative-0.3.0/mlflow_knative/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.2.0/mlflow_knative/deployment_client.py` & `mlflow_knative-0.3.0/mlflow_knative/deployment_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,19 +106,19 @@
                 )
             except kubernetes.client.rest.ApiException as error:
                 if error.status == HTTPStatus.CONFLICT:
                     raise mlflow.exceptions.MlflowException(
                         f"a deployment with name '{name}' "
                         f"already exists in namespace '{namespace}'."
                     )
-                else:  # pragma: no cover
+                else:
                     raise mlflow.exceptions.MlflowException(
                         f"Kubernetes API error ({error.status})"
                     ) from error
-            except KnativeTimeoutError as error:  # pragma: no cover
+            except KnativeTimeoutError as error:
                 raise mlflow.exceptions.MlflowException(
                     f"service creation failed: {str(error)}"
                 )
 
         return {"name": service["metadata"]["name"], "flavor": flavor}
 
     def update_deployment(
@@ -182,19 +182,19 @@
                 )
             except kubernetes.client.rest.ApiException as error:
                 if error.status == HTTPStatus.NOT_FOUND:
                     raise mlflow.exceptions.MlflowException(
                         f"no deployment with name '{name}' "
                         f"found in namespace '{namespace}'."
                     )
-                else:  # pragma: no cover
+                else:
                     raise mlflow.exceptions.MlflowException(
                         f"Kubernetes API error ({error.status})"
                     ) from error
-            except KnativeTimeoutError as error:  # pragma: no cover
+            except KnativeTimeoutError as error:
                 raise mlflow.exceptions.MlflowException(
                     f"service update failed: {str(error)}"
                 )
 
         return {"name": service["metadata"]["name"], "flavor": flavor}
 
     def delete_deployment(
@@ -218,42 +218,48 @@
                 knative_api.delete_namespaced_service(namespace=namespace, name=name)
             except kubernetes.client.rest.ApiException as error:
                 if error.status == HTTPStatus.NOT_FOUND:
                     raise mlflow.exceptions.MlflowException(
                         f"no deployment with name '{name}' "
                         f"found in namespace '{namespace}'."
                     )
-                else:  # pragma: no cover
+                else:
                     raise mlflow.exceptions.MlflowException(
                         f"Kubernetes API error ({error.status})"
                     ) from error
 
     def list_deployments(self, endpoint: str | None = None) -> list[dict[str, str]]:
         """List deployments on a Knative target (across all namespaces)."""
         if endpoint:
             raise EndpointArgumentNotSupported
 
         with self._kubernetes_client as kubernetes_client:
             core_api = kubernetes.client.CoreV1Api(kubernetes_client)
             knative_api = KnativeServingV1Api(kubernetes_client)
-
-            return [
-                {
-                    "name": service["metadata"]["name"],
-                    "namespace": service["metadata"]["namespace"],
-                    "url": service["status"]["url"],
-                    "generation": service["metadata"]["generation"],
-                    "creation_timestamp": service["metadata"]["creationTimestamp"],
-                    "run_id": service["metadata"]["annotations"].get(RUN_ID_ANNOTATION),
-                }
-                for namespace in core_api.list_namespace().items
-                for service in knative_api.list_namespaced_service(
-                    namespace=namespace.metadata.name
-                )["items"]
-            ]
+            try:
+                return [
+                    {
+                        "name": service["metadata"]["name"],
+                        "namespace": service["metadata"]["namespace"],
+                        "url": service["status"]["url"],
+                        "generation": service["metadata"]["generation"],
+                        "creation_timestamp": service["metadata"]["creationTimestamp"],
+                        "run_id": service["metadata"]["annotations"].get(
+                            RUN_ID_ANNOTATION
+                        ),
+                    }
+                    for namespace in core_api.list_namespace().items
+                    for service in knative_api.list_namespaced_service(
+                        namespace=namespace.metadata.name
+                    )["items"]
+                ]
+            except kubernetes.client.rest.ApiException as error:
+                raise mlflow.exceptions.MlflowException(
+                    f"Kubernetes API error ({error.status})"
+                ) from error
 
     def get_deployment(self, name: str, endpoint: str | None = None) -> dict[str, str]:
         """Get metadata for a deployment on a Knative target (across all namespaces).
 
         Note: this fails if multiple deployments with the same name exist across
         multiple namespaces.
         Unfortunately MLflow deployment client interface does not allow passing
@@ -285,14 +291,18 @@
                                 RUN_ID_ANNOTATION
                             ),
                         }
                     )
                 except kubernetes.client.rest.ApiException as error:
                     if error.status == HTTPStatus.NOT_FOUND:
                         pass
+                    else:
+                        raise mlflow.exceptions.MlflowException(
+                            f"Kubernetes API error ({error.status})"
+                        ) from error
 
             try:
                 (deployment,) = deployments
             except ValueError as error:
                 raise mlflow.exceptions.MlflowException(
                     "must return exactly one deployment matching the provided name."
                 ) from error
@@ -323,17 +333,17 @@
             )
             response.raise_for_status()
         except requests.exceptions.ConnectionError as error:
             raise mlflow.exceptions.MlflowException(
                 "could not connect to the deployment, are you sure "
                 f"the service URL '{deployment['url']}' is publicly available?"
             ) from error
-        except requests.exceptions.HTTPError as error:
+        except requests.exceptions.RequestException as error:
             raise mlflow.exceptions.MlflowException(
-                "deployment request HTTP error."
+                "deployment request error."
             ) from error
 
         return response.json()
 
 
 def run_local(
     name: str,
@@ -354,15 +364,19 @@
 
     config = config if config is not None else {}
 
     with warnings.catch_warnings():
         warnings.simplefilter("once")
         model = mlflow.pyfunc.load_model(model_uri)
 
-    model.serve(enable_mlserver=True, host=config.get("host"), port=config.get("port"))
+    model.serve(
+        enable_mlserver=True,
+        host=config.get("host", "localhost"),
+        port=config.get("port", 8080),
+    )
 
 
 def target_help() -> str | None:
     """MLflow deployments Knative target.
 
     * A `target_uri` must be constructed with the scheme "knative:/<kube context>".
       (e.g. for AWS EKS clusters, the context is the ARN of the cluster
```

### Comparing `mlflow_knative-0.2.0/mlflow_knative/knative.py` & `mlflow_knative-0.3.0/mlflow_knative/knative.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,34 @@
 
 
 def _handle_namespaced_service_is_ready_event(
     namespace: str, name: str, event: dict
 ) -> bool:
     """Handle the ready event for Knative services."""
     try:
+        # Only consider a resource modification event.
         if event["type"] != KUBERNETES_EVENT_TYPE_MODIFIED:
             return False
 
         metadata = event["object"]["metadata"]
+        # Event query is namespaced, so the redundant namespace check *shouldn't*
+        # be required, but still present to ensure the safety of this handler.
         if metadata["namespace"] != namespace or metadata["name"] != name:
-            return False
+            return False  # pragma: no cover
 
+        # All service status readiness conditions must be fulfilled for the service to
+        # be considered ready.
         return all(
             condition["status"] == str(True)
             for condition in event["object"]["status"]["conditions"]
         )
-    except KeyError:
+
+    # In the event a key required to accept the event or perform service status
+    # readiness checks is missing, we assume this is not an accepted event.
+    except KeyError:  # pragma: no cover
         return False
 
 
 class KnativeTimeoutError(Exception):
     """Raised when the creation or update of a Knative services reaches a timeout."""
```

### Comparing `mlflow_knative-0.2.0/mlflow_knative/mlflow_docker.py` & `mlflow_knative-0.3.0/mlflow_knative/mlflow_docker.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.2.0/mlflow_knative/service.yaml` & `mlflow_knative-0.3.0/mlflow_knative/service.yaml`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.2.0/mlflow_knative/templating.py` & `mlflow_knative-0.3.0/mlflow_knative/templating.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.2.0/pyproject.toml` & `mlflow_knative-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "mlflow-knative"
-version = "0.2.0"
+version = "0.3.0"
 description = "MLflow plugin adding a Knative deployment target"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "deployment", "deployments", "knative", "kubernetes", "kn", "k8s"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 repository = "https://gitlab.com/lzinsou/mlflow-knative"
 packages = [{include = "mlflow_knative"}]
```

### Comparing `mlflow_knative-0.2.0/PKG-INFO` & `mlflow_knative-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlflow-knative
-Version: 0.2.0
+Version: 0.3.0
 Summary: MLflow plugin adding a Knative deployment target
 Home-page: https://gitlab.com/lzinsou/mlflow-knative
 Keywords: mlflow,plugin,mlops,deployment,deployments,knative,kubernetes,kn,k8s
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<3.13
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

