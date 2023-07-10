# Comparing `tmp/nnx-0.0.6.tar.gz` & `tmp/nnx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.6.tar", max compression
+gzip compressed data, was "nnx-0.0.7.tar", max compression
```

## Comparing `nnx-0.0.6.tar` & `nnx-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.6/LICENSE
--rw-r--r--   0        0        0    19148 2023-06-19 14:04:51.402418 nnx-0.0.6/README.md
--rw-r--r--   0        0        0     1223 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/__init__.py
--rw-r--r--   0        0        0     7443 2023-06-13 22:07:35.044745 nnx-0.0.6/nnx/containers.py
--rw-r--r--   0        0        0     6512 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/contextlib.py
--rw-r--r--   0        0        0     4495 2023-06-13 22:07:35.044745 nnx-0.0.6/nnx/dataclasses.py
--rw-r--r--   0        0        0       45 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/errors.py
--rw-r--r--   0        0        0     3617 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/helpers.py
--rw-r--r--   0        0        0    23324 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/module.py
--rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.6/nnx/nn/__init__.py
--rw-r--r--   0        0        0      763 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/nn/activations.py
--rw-r--r--   0        0        0     2763 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     1888 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/nn/initializers.py
--rw-r--r--   0        0        0    16022 2023-06-12 22:45:21.347880 nnx-0.0.6/nnx/nn/linear.py
--rw-r--r--   0        0        0    13530 2023-06-12 22:45:21.347880 nnx-0.0.6/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2282 2023-06-12 22:45:21.351881 nnx-0.0.6/nnx/nn/stochastic.py
--rw-r--r--   0        0        0      348 2023-06-08 02:13:59.012365 nnx-0.0.6/nnx/nodes.py
--rw-r--r--   0        0        0     2240 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/partitioning.py
--rw-r--r--   0        0        0     8445 2023-06-13 22:07:35.044745 nnx-0.0.6/nnx/pytreelib.py
--rw-r--r--   0        0        0     2313 2023-06-12 22:45:21.351881 nnx-0.0.6/nnx/reprlib.py
--rw-r--r--   0        0        0     5399 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/state.py
--rw-r--r--   0        0        0     2412 2023-06-08 02:13:59.016365 nnx-0.0.6/nnx/tracers.py
--rw-r--r--   0        0        0    17611 2023-06-19 13:43:48.881037 nnx-0.0.6/nnx/transforms.py
--rw-r--r--   0        0        0     2037 2023-06-19 13:43:48.881037 nnx-0.0.6/nnx/utils.py
--rw-r--r--   0        0        0      764 2023-06-19 14:18:43.435867 nnx-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    19681 1970-01-01 00:00:00.000000 nnx-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-05 17:41:51.529317 nnx-0.0.7/LICENSE
+-rw-r--r--   0        0        0    21250 2023-07-10 14:57:54.628800 nnx-0.0.7/README.md
+-rw-r--r--   0        0        0     1410 2023-07-10 15:00:29.396804 nnx-0.0.7/nnx/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-10 15:00:28.184804 nnx-0.0.7/nnx/containers.py
+-rw-r--r--   0        0        0     5417 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/contextlib.py
+-rw-r--r--   0        0        0     4512 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/dataclasses.py
+-rw-r--r--   0        0        0       45 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/errors.py
+-rw-r--r--   0        0        0     4345 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/helpers.py
+-rw-r--r--   0        0        0     1832 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/ids.py
+-rw-r--r--   0        0        0    26625 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/module.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2763 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     2147 2023-07-08 19:31:09.240551 nnx-0.0.7/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    16022 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/nn/linear.py
+-rw-r--r--   0        0        0    13511 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2281 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0      348 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nodes.py
+-rw-r--r--   0        0        0     2037 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/partitioning.py
+-rw-r--r--   0        0        0     8738 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/pytreelib.py
+-rw-r--r--   0        0        0     2313 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/reprlib.py
+-rw-r--r--   0        0        0    13718 2023-07-08 19:31:09.240551 nnx-0.0.7/nnx/spmd.py
+-rw-r--r--   0        0        0     5103 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/state.py
+-rw-r--r--   0        0        0     2412 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/tracers.py
+-rw-r--r--   0        0        0    22437 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/transforms.py
+-rw-r--r--   0        0        0      764 2023-07-10 15:09:18.980819 nnx-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    22353 1970-01-01 00:00:00.000000 nnx-0.0.7/setup.py
+-rw-r--r--   0        0        0    21733 1970-01-01 00:00:00.000000 nnx-0.0.7/PKG-INFO
```

### Comparing `nnx-0.0.6/LICENSE` & `nnx-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.6/README.md` & `nnx-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 # NNX
 
 _**N**eural **N**etworks for JA**X**_
 
 NNX is a Neural Networks library for JAX that provides a simple yet powerful module system that adheres to standard Python semantics. Its aim is to combine the robustness of [Flax](https://flax.readthedocs.io/en/latest/) with a simplified, Pythonic API akin to that of [PyTorch](https://pytorch.org/).
 
 * **Pythonic**: Modules are just regular python classes, they contain their own state, are fully mutable, and allow sharing references between Modules.
-* **Fully Compatible**: Easy convert back and forth between Modules and pure pytrees compatible with any JAX transformation and other JAX tooling.
+* **Compatible**: Easily convert back and forth between Modules and pytrees using the Functional API to integrate with any JAX API.
 * **Safe**: NNX incorporates mechanisms to try to prevent tracer leakage, avoid stale RNGs, and ensure proper state propagation in order to help produce correct JAX programs.
 * **Semantic**: Partition a Module's state into different semantic collections, allowing for fine-grained control when applying JAX transformations.
-* **Lifted Transforms**: NNX offers a set of Module-aware transforms that automatically manage the Module's state and provide APIs to instruct the underlying JAX transform how to handle each state collection.
 
 #### Table of Contents
 * [Installation](#installation)
 * [Getting Started](#getting-started)
 * [FAQs](#faqs)
 * [Examples](#examples)
 * [User Guide](#user-guide)
@@ -37,20 +36,22 @@
 The following example guides you through creating a basic `Linear` model with NNX and executing a forward pass. It also demonstrate how handle mutable state by showing how to keep track of the number of times the model has been called.
 
 ```python
 import nnx
 import jax
 import jax.numpy as jnp
 
+class Count(nnx.Variable): pass
+
 class Linear(nnx.Module):
     def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
         key = ctx.make_rng("params")
-        self.w = nnx.param(jax.random.uniform(key, (din, dout)))
-        self.b = nnx.param(jnp.zeros((dout,)))
-        self.count = nnx.var("counts", 0)  # track the number of calls
+        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))
+        self.b = nnx.Param(jnp.zeros((dout,)))
+        self.count = Count(0)  # track the number of calls
 
     def __call__(self, x):
         self.count += 1
         return x @ self.w + self.b
 
 model = Linear(din=12, dout=2, ctx=nnx.context(0))
 
@@ -64,22 +65,22 @@
 inside `__init__` to generate a random key to initialize the parameters.
 
 ### Training with the Functional API
 
 The [Functional API](#functional-api) converts an NNX Module python semantics into pure pytree object with functional semantics. It is the recommended way to use NNX as it provides tight control over the state, allows you to use regular JAX transformations, and it minimizes overhead. In this example the model will be trained using Stochastic Gradient Descent (SGD).
 
 ```python
-(params, counts), moduledef = model.partition("params", "counts")
+(params, counts), moduledef = model.partition(nnx.Param, Count)
 
 @jax.jit
 def train_step(params, counts, x, y):
     def loss_fn(params):
         y_pred, (updates, _) = moduledef.apply(params, counts)(x)
         loss = jax.numpy.mean((y_pred - y) ** 2)
-        return loss, updates.filter("counts")
+        return loss, updates.filter(Count)
 
     # compute gradient
     grads, counts = jax.grad(loss_fn, has_aux=True)(params)
     # SGD update
     params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grads)
 
     return params, counts
@@ -98,36 +99,36 @@
 @nnx.jit
 def train_step(model, x, y):
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
     
     # compute gradient
-    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
+    grads: nnx.State = nnx.grad(loss_fn, wrt=nnx.Param)(model)
     # SGD update
     model.update_state(
-        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
+        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter(nnx.Param), grads)
     )
 
 # execute the training step
 train_step(model, x, y)
 assert model.count == 2
 ```
 
 **Note**: Using `nnx.jit` introduces some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes, but for production code use `jax.jit` directly.
 
 ## Examples
 
-* [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/01_jit_transform.py): Shows how to train a simple model using lifted transforms.
-* [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/02_functional_api.py): Shows how to train a simple model using the functional API.
+* [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/01_functional_api.py): Shows how to train a simple model using the functional API.
+* [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/02_lifted_transforms.py): Shows how to train a simple model using lifted transforms.
 * [Using TrainState](https://github.com/cgarciae/nnx/blob/main/examples/03_train_state.py): Shows how to train a simple model using the functional API with the help of `TrainState`.
 * [Using PureModule](https://github.com/cgarciae/nnx/blob/main/examples/04_pure.py) (experimental): Shows how to train a simple model using the functional API and leveraging `PureModule` to simplify the code.
 * [Training a VAE](https://github.com/cgarciae/nnx/blob/main/examples/05_vae.py): Shows how to train a VAE on the binarized MNIST dataset, uses the functional API, `TrainState`, and shows how to use capture intermediate values to retrieve `kl_loss`.
 * [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py): An contrived example that implements scan over layers with dropout and a share BatcNorm layer to showcase how lifted transforms can be implemented. It uses the functional API along with `jax.vmap` and `jax.lax.scan`.
-* [Creating a Transformer](https://github.com/cgarciae/nnx/blob/main/examples/07_tranformer.py): Shows how to create a Transformer with an auto-regressive decoder that uses scan over layers and a kv-cache for fast inference. Credits to @levskaya.
+* [Creating a Transformer](https://github.com/cgarciae/nnx/blob/main/examples/07_transformer.py): Shows how to create a Transformer with an auto-regressive decoder that uses scan over layers and a kv-cache for fast inference. Credits to @levskaya.
 
 ## FAQs
 
 ### Status
 NNX is still in early development so expect bugs and breaking changes. That said, current API is the result of months of experimentation and we don't expect any major changes in the near future.
 
 ### How is it different from Flax?
@@ -146,24 +147,24 @@
 
 One major difference between the two frameworks is that, by design, NNX Modules are not Pytrees. This adds a safety layer as it prevents state updates from being lost by accident due to referential transparency. It also removes the need of threading a separate [State container](https://docs.kidger.site/equinox/examples/stateful/) throughout the code in order to propagate state. In NNX state updates are either always preserved or explicitly discarded by the user.
 
 ## User Guide
 
 ### Modules
 
-NNX Modules are normal python classes, they obey regular python semantics such as mutability and reference sharing, including reference cycles. They can contain 2 types of attributes: node attributes and static attributes. Node attributes include NNX `Variable`s (e.g. `nnx.param`), Numpy arrays, JAX arrays, submodules Modules, and other NNX types. All other types are treated as static attributes.
+NNX Modules are normal python classes, they obey regular python semantics such as mutability and reference sharing, including reference cycles. They can contain 2 types of attributes: node attributes and static attributes. Node attributes include NNX `Variable`s (e.g. `nnx.Param`), Numpy arrays, JAX arrays, submodules Modules, and other NNX types. All other types are treated as static attributes.
 
 ```python
 class Foo(nnx.Module):
     def __init__(self, ctx: nnx.Context):
         # node attributes
-        self.variable = nnx.param(jnp.array(1))
+        self.variable = nnx.Param(jnp.array(1))
         self.np_buffer = np.array(2)
         self.jax_buffer = jnp.array(3)
-        self.node = nnx.node([4, 5])
+        self.node = nnx.Node([4, 5])
         self.submodule = nnx.Linear(2, 4, ctx=ctx)
         # static attributes
         self.int = 1
         self.float = 2.0
         self.str = "hello"
         self.list = [1, 2, 3]
 
@@ -179,17 +180,17 @@
 state, moduledef = model.partition()
 ```
 ```
 State({
   ('jax_buffer',): Array(3),
   ('node',): Node(value=[4, 5]),
   ('np_buffer',): array(2),
-  ('submodule', 'bias'): Variable(collection='params', value=Array(...)),
-  ('submodule', 'kernel'): Variable(collection='params', value=Array(...)),
-  ('variable',): Variable(collection='params', value=Array(1))
+  ('submodule', 'bias'): Param(value=Array(...)),
+  ('submodule', 'kernel'): Param(value=Array(...)),
+  ('variable',): Param(value=Array(1))
 })
 ```
 
 `State` and `ModuleDef` are pytrees so they can be passed to JAX transformations. More over, `ModuleDef` provides 2 very important methods: `merge` and `apply`. The `merge` method can be used to create a new `Module` from a `State` object:
 
 ```python
 model = moduledef.merge(state)
@@ -204,31 +205,31 @@
 # run submodule
 y, (state, moduledef) = moduledef.apply(state).submodule(x)
 ```
 
 `apply` can call any nested method or submodule as long as it can be accessed via the `.` or `[]` operators.
 
 ### Partitioning State
-`nnx.var` lets you create `Variable` attributes with `collection` metadata, this metadata can be used to partition the state into multiple substates. `nnx.param` is a special case of `nnx.var` where `collection="params"`. 
+In NNX you can filter based on any node type, most commonly you will want to filter based on `nnx.Variable` subclasses such as `nnx.Param` or `nnx.BatchStat`.
 
-Here are various examples of how you can use the `partition` method along with collection names to partition a module into multiple substates:
+Here are various examples of how you can use the `partition` method to split a module into multiple substates:
 
 ```python
 # partition the module into the state with all the nodes and the moduledef
 state, moduledef = model.partition()
 # verify that the state contains only params, else raise an error
-params, moduledef = model.partition("params")
+params, moduledef = model.partition(nnx.Param)
 # split the state into params and batch_stats, verify no nodes are left
-(params, batch_stats), moduledef = model.partition("params", "batch_stats")
+(params, batch_stats), moduledef = model.partition(nnx.Param, nnx.BatchStat)
 # if there are any nodes left, use the `...` filter to capture them
-(params, batch_stats, rest), moduledef = model.partition("params", "batch_stats", ...)
+(params, batch_stats, rest), moduledef = model.partition(nnx.Param, nnx.BatchStat, ...)
 # using `...` as the only filter is equivalent to not passing any filters
 model.partition(...) = model.partition()
 ```
-`partition` will make sure all nodes are match by atleast one filter, else it will raise an error. If you have non-`Variable` nodes like `nnx.node`, `jax.Array`, or `numpy.ndarray` attributes, you can use the `...` filter which will match any node. For a more general filter you can pass a predicate function of the form:
+`partition` will make sure all nodes are match by atleast one filter, else it will raise an error. If you have non-`Variable` nodes like `nnx.Node`, `jax.Array`, or `numpy.ndarray` attributes, you can use the `...` filter which will match any node. For a more general filter you can pass a predicate function of the form:
 
 ```python
 (path: Tuple[str, ...], value: Any) -> bool
 ```
 
 To reconstruct the module from a set of substates, you can use `merge` as usual but passing the substates as additional arguments:
 
@@ -241,130 +242,173 @@
 ```python
 y, (state, moduledef) = moduledef.apply(params, batch_stats, rest)(x)
 ```
 
  Note that `apply` will return a single `state` object, if you need to re-partition the state you can use `State`'s own `partition` method:
 
 ```python
-params, batch_stats, rest = state.partition("params", "batch_stats", ...)
+params, batch_stats, rest = state.partition(nnx.Param, nnx.BatchStat, ...)
 ```
 
 Alternatively, if you are just interested in a subset of partitions, you can use the `State.filter` method which will not raise an error if some nodes are not matched by any filter:
 
 ```python
 # only get params
-params = state.filter("params")
+params = state.filter(nnx.Param)
 # get params and batch_stats
-params, batch_stats = state.filter("params", "batch_stats")
+params, batch_stats = state.filter(nnx.Param, nnx.BatchStat)
 ```
 
 ### Filters
 
 Filters let you select subsets of nodes based on some criteria. These are use throughout the API in method like `partition`, `filter`, and `pop_state`. There are 4 types of filters:
 
-* `str`: matches all `Variable` nodes (e.g. `nnx.param` or `nnx.var`) with the given `collection` name.
 * `type`: matches all node instances of the given type.
 * `...`: matches all nodes.
 * `(path, any) -> bool`: a predicate function that takes a node path and value and returns a boolean.
 * `Tuple[Filter, ...]`: a tuple of filters, matches all nodes that match any of the filters.
 
 NNX also provides the following custom filters:
 
 * `nnx.Not(filter)`: matches all nodes that do not match the given filter
 * `nnx.buffers`: matches all `numpy.ndarray` and `jax.Array` nodes
 
 Here is an example of how to use `Not` and `buffers`:
 ```python
-rest = module.filter(nnx.Not("params"))
+rest = module.filter(nnx.Not(nnx.Param))
 buffers = module.filter(nnx.buffers)
 ```
 
 
 ### Capturing Intermediate Values
 In NNX you can easily propagate intemediate values by simply assigning them to an attribute at runtime. For convenience, you should assign them to a `Variable` attribute with a `collection` name by using `nnx.var` so you can easily retrieve them later.
 
 Here is an example of how to create a `Linear` module that captures its output into a `Variable` attribute with the `intermediates` collection name:
 
 ```python
 class Linear(nnx.Module):
     def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
         key = ctx.make_rng("params")
-        self.w = nnx.param(jax.random.uniform(key, (din, dout)))
-        self.b = nnx.param(jnp.zeros((dout,)))
+        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))
+        self.b = nnx.Param(jnp.zeros((dout,)))
 
     def __call__(self, x):
         y = x @ self.w + self.b
-        self.y = nnx.var("intermediates", y)
+        self.y = nnx.Intermediate(y)
         return y
 
 model = Linear(12, 2, ctx=nnx.context(0))
 ```
-Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `intermediates`:
+Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `Intermediate`:
 
 ```python
 y = model(jnp.ones((8, 12)))
-intermediates = model.pop_state("intermediates")
+intermediates = model.pop_state(nnx.Intermediate)
 ```
 `pop_state` will return a `State` object with the nodes that match the given filter and remove them from the module's attributes.
 
 ```
 State({
-  ('y',): Variable(
-    collection='intermediates',
+  ('y',): Intermediate(
     value=Array(...)
   )
 })
 ```
 
-If you use the functional API to call the module instead, the `intermediates` nodes will be present in the output `state`. To retrieve the `intermediates` nodes and optionally separate them from the output `state` you can use `State.partition`:
+If you use the functional API to call the module instead, the `Intermediate` nodes will be present in the output `state`. To retrieve the `intermediates` nodes and optionally separate them from the output `state` you can use `State.partition`:
 
 ```python
 state, moduledef = model.partition()
 y, (state, moduledef) = moduledef.apply(state)(jnp.ones((8, 12)))
 # "pop" the intermediates from the state
 intermediates, state = state.partition("intermediates", ...)
 ```
 
 Alternatively, you can use `State.filter` to retrieve the `intermediates` nodes without removing them from the `state`.
 
 
 
 ### Lifted Transforms
 
-Stateful transforms take a Module as their first argument, track changes in the state that occur within the transformation, and automatically propagate those changes to the input Module outside the transformation. In general, they behave as stateful functions with respect to the first argument.
+NNX lifted transforms analogous versions of JAX transforms but they know how to work with Modules. They usually perform the following tasks:
+
+* Handle the Module's substates and Context's RNG streams according to the transform's semantics.
+* Properly propagating state in and out of the transform, including updating the input Module's state with updates that happen inside the transform.
+
+Here's a diagram illustrating how lifted transformations work:
+
+![lifted-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
 
-Here's a diagram illustrating how stateful transformations work:
+Currently NNX provides the `jit`, `grad`, and `scan` lifted transforms.
 
-![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
+#### Manual Lifting
 
-Currently, `nnx.jit` and `nnx.grad` are the only stateful transformations.
+In case you want to use JAX transforms directly you can always use the functional API
+to manually lift your Modules. 
 
-The following example demonstrates how a `train_step` function can be implemented using `nnx.jit` and `nnx.grad`:
+Here we will create an example of how to implement an MLP that uses "scan over layers" to efficiently process a sequence of inputs assuming that each layer has the same parameters and input/output dimensions. The first thing we need to do is create a `Block` module that represents a single layer, this block with just contain a `Linear` layer, a `Dropout` layer, and a `GELU` activation function:
 
 ```python
-@nnx.jit
-def train_step(model, x, y):
+class Block(nnx.Module):
+    def __init__(self, dim: int, *, ctx: nnx.Context):
+        self.linear = nnx.Linear(dim, dim, ctx=ctx)
+        self.dropout = nnx.Dropout(0.5)
 
-    def loss_fn(model):
-        y_pred = model(x)
-        return jax.numpy.mean((y_pred - y) ** 2)
-    
-    # compute gradient
-    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
-    # SGD update
-    model.update_state(
-        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
-    )
+    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:
+        x = self.linear(x)
+        x = self.dropout(x, deterministic=not train, ctx=ctx)
+        x = jax.nn.gelu(x)
+        return x
+```
+
+Now we will define `ScanMLP`. During `__init__`, instead of creating a list of `Block`s, we will use `jax.vmap` to create a single `Block` whose parameters have an addtional `layer` axis. This will allow us to pass the parameters as inputs to scan so it will apply a layer at each step.
+
+```python
+class ScanMLP(nnx.Module):
+    def __init__(self, dim: int, *, n_layers: int, ctx: nnx.Context):
+        params_key = jax.random.split(ctx.make_rng("params"), n_layers)
+        self.n_layers = n_layers
+        self.layers = jax.vmap(
+            lambda key: Block(dim, ctx=nnx.context(params=key)).partition()
+        )(params_key).merge()
 
-# stateful update
-train_step(model, x, y)
 ```
+Note that we split the `params` key into `n_layers` keys so each layer has different parameters.
+
+Now we will define `__call__`. Here we need to split the `dropout` key into `n_layers` keys so each layer has a different dropout mask, and `partition` the layers to get their `params`. Both `params` and `dropout_key` will be passed as inputs, `x` will be the carry value. Inside the `scan_fn` we will merge the `params` back into a `Block` module and
+apply it to the input `x`, passing the sliced `dropout_key` as part of the `Context`.
+
+
+```python
+    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:
+        dropout_key = jax.random.split(ctx.make_rng("dropout"), self.n_layers)
+        params, moduledef = self.layers.partition(nnx.Param)
 
-The most interesting aspect of this design is that the code appears very imperative, as the state is automatically propagated in and out of the transformations.
+        def scan_fn(x: inputs):
+            params, dropout_key = inputs
+            module = moduledef.merge(params)
+            x = module(x, train=train, ctx=nnx.context(dropout=dropout_key))
+            return x, module.filter(nnx.Param)
+
+        x, params = jax.lax.scan(scan_fn, x, (params, dropout_key))
+        self.layers.update_state(params)
+        return x
+```
+Finally we apply `jax.lax.scan`, update the `layers` state with the new `params`, and return the final `x` value.
+
+Here is a simple way to test our `ScanMLP`:
+
+```python
+model = ScanMLP(10, n_layers=5, ctx=nnx.context(0))
+
+x = jnp.ones((3, 10))
+y = model(x, train=True, ctx=nnx.context(dropout=1))
+```
 
+For a more robust implementation with comments take a look at the [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py) example.
 
 ### Case Studies
 #### Shared State
 
 In NNX, you can create modules that share state between them. This is useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
 
 Here's an example of creating a module with shared state:
```

### Comparing `nnx-0.0.6/nnx/__init__.py` & `nnx-0.0.7/nnx/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 __version__ = "0.0.0"
 
 
 from .containers import (
+    BatchStat,
+    Cache,
     Container,
+    ContainerMetadata,
+    Intermediate,
     Node,
+    Param,
     Static,
     Variable,
-    VarMetadata,
-    node,
-    param,
-    static,
-    var,
-    var_metadata,
-    with_partitioning,
+    with_metadata,
 )
-from .contextlib import Context, RngStream, context
+from .contextlib import Context, context
 from .dataclasses import (
     dataclass,
     field,
     node_field,
     param_field,
     static_field,
     var_field,
@@ -55,10 +54,18 @@
     tanh,
 )
 from .nn.linear import Conv, Embed, Linear
 from .nn.normalization import BatchNorm, LayerNorm
 from .nn.stochastic import Dropout
 from .nodes import is_node, register_node_type
 from .partitioning import All, Not, buffers
-from .pytreelib import Pytree
+from .pytreelib import Pytree, TreeNode
+from .spmd import (
+    PARTITION_NAME,
+    get_partition_spec,
+    logical_axis_rules,
+    logical_to_mesh,
+    with_logical_constraint,
+    with_logical_partitioning,
+)
 from .state import State
-from .transforms import grad, jit, scan
+from .transforms import Remat, Scan, grad, jit, remat, scan
```

### Comparing `nnx-0.0.6/nnx/containers.py` & `nnx-0.0.7/nnx/containers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,311 +1,202 @@
 import dataclasses
 import functools
 import typing as tp
-from abc import ABC, abstractmethod
+from abc import ABCMeta
 from functools import partial
+from typing import Any
 
 import jax.tree_util as jtu
 
 from nnx import nodes, reprlib
-from nnx.nn import initializers
 
 A = tp.TypeVar("A")
 B = tp.TypeVar("B")
-C = tp.TypeVar("C", bound="Container[tp.Any]")
 F = tp.TypeVar("F", bound=tp.Callable[..., tp.Any])
-Sharding = tp.Tuple[str, ...]
+Sharding = tp.Tuple[tp.Optional[str], ...]
 
 
-class Container(ABC, tp.Generic[A]):
-    __slots__ = ("_value",)
-
-    def __init__(self, value: A):
-        self._value = value
+@dataclasses.dataclass
+class ContainerMetadata(tp.Generic[A]):
+    value: A
+    metadata: tp.Mapping[str, tp.Any]
 
-    @property
-    def value(self) -> A:
-        return self._value
 
-    def replace_value(self: C, value: tp.Any) -> C:
+class ContainerMetaclass(ABCMeta):
+    def __call__(self, value: A, **metadata: tp.Any) -> A:
         if isinstance(value, Container):
-            if not self.is_equivalent(value):
-                raise ValueError(
-                    "Cannot replace value from incompatible container, "
-                    f"expected {self}, got {value}"
-                )
-            value = value.value
+            container = value
+            value = container.value
+        else:
+            container = None
 
-        return self._replace_value(value)
+        obj = super().__call__(value, **metadata)
 
-    @abstractmethod
-    def _replace_value(self: C, value: tp.Any) -> C:
-        ...
+        if container is not None and not container.is_equivalent(obj):
+            raise ValueError(
+                f"input value of type '{type(container).__name__}' is not compatible "
+                f"with return type '{type(obj).__name__}'"
+            )
 
-    @abstractmethod
-    def is_equivalent(self, other: tp.Any) -> bool:
-        ...
+        return obj
 
-    @abstractmethod
-    def copy(self: C) -> C:
-        ...
 
+class Container(tp.Generic[A], reprlib.Representable, metaclass=ContainerMetaclass):
+    value: A
 
-class Node(Container[A], reprlib.Representable):
-    __slots__ = ()
+    def __init__(self, value: tp.Union[A, ContainerMetadata[A]], **metadata: tp.Any):
+        if isinstance(value, ContainerMetadata):
+            metadata.update(value.metadata)
+            value = tp.cast(A, value.value)
 
-    def __nnx_repr__(self):
-        yield reprlib.Object(type=type(self))
-        yield reprlib.Attr(
-            "value", repr(self._value) if isinstance(self._value, str) else self._value
-        )
+        vars(self).update(metadata, value=value)
 
-    def __eq__(self, other: object) -> bool:
-        return type(other) is Node and self._value == other._value
+    if tp.TYPE_CHECKING:
 
-    def copy(self) -> "Node[A]":
-        return Node(self._value)
+        def __getattr__(self, name: str) -> tp.Any:
+            ...
 
-    def _replace_value(
-        self,
-        value: B,
-    ) -> "Node[B]":
-        return Node(value)
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Container):
+            return False
+        return type(self) is type(other) and vars(other) == vars(self)
 
-    def is_equivalent(self, other: tp.Any) -> bool:
-        return type(other) is Node
+    @tp.overload
+    def replace(self, *, value: B, **kwargs) -> "Container[B]":
+        ...
 
+    @tp.overload
+    def replace(self, **kwargs) -> "Container[A]":
+        ...
 
-def _node_flatten(
-    x: Node[tp.Any],
-    *,
-    with_keys: bool,
-):
-    if with_keys:
-        node = (jtu.GetAttrKey("value"), x._value)
-    else:
-        node = x._value
+    def replace(self, **kwargs) -> "Container[tp.Any]":
+        if "value" in kwargs:
+            value = kwargs["value"]
+            if isinstance(value, Container):
+                if not self.is_equivalent(value):
+                    raise ValueError(
+                        "Cannot replace value from incompatible container, "
+                        f"expected {self}, got {value}"
+                    )
+                kwargs["value"] = value.value
+
+        attributes = vars(self).copy()
+        # validate keys
+        for key in kwargs:
+            if key not in attributes:
+                raise ValueError(f"Unknown metadata key {key!r}")
+        attributes.update(**kwargs)
+        node_type = type(self)
+        return node_type(**attributes)
 
-    return (node,), None
+    def is_equivalent(self, other: tp.Any) -> bool:
+        def metadata_fields(container: Container[tp.Any]) -> tp.Dict[str, tp.Any]:
+            return {k: v for k, v in vars(container).items() if k != "value"}
 
+        return type(self) is type(other) and metadata_fields(self) == metadata_fields(
+            other
+        )
 
-def _node_unflatten(metadata: None, children: tp.Tuple[A]) -> Node[A]:
-    return Node(children[0])
+    def copy(self: "Container[A]") -> "Container[A]":
+        return type(self)(**vars(self))
 
+    def __nnx_repr__(self):
+        yield reprlib.Object(type=type(self))
+        for name, value in vars(self).items():
+            yield reprlib.Attr(name, repr(value))
 
-jtu.register_pytree_with_keys(
-    Node,
-    partial(_node_flatten, with_keys=True),
-    _node_unflatten,
-    flatten_func=partial(_node_flatten, with_keys=False),
-)
 
+class NodeBase(Container[A]):
+    def __init_subclass__(cls):
+        super().__init_subclass__()
 
-@dataclasses.dataclass
-class VarMetadata(tp.Generic[A]):
-    value: A
-    sharding: Sharding
+        def _node_flatten(
+            x: NodeBase[tp.Any],
+            *,
+            with_keys: bool,
+        ):
+            attributes = vars(x).copy()
+            value = attributes.pop("value")
+            if with_keys:
+                node = (jtu.GetAttrKey("value"), value)
+            else:
+                node = value
 
+            return (node,), attributes
 
-def with_partitioning(
-    initializer: initializers.Initializer,
-    sharding: Sharding,
-) -> initializers.Initializer:
-    @functools.wraps(initializer)
-    def wrapper(*args):
-        return VarMetadata(initializer(*args), sharding)
+        def _node_unflatten(
+            metadata: tp.Mapping[str, tp.Any], children: tp.Tuple[A]
+        ) -> NodeBase[A]:
+            return cls(children[0], **metadata)
 
-    return wrapper  # type: ignore
+        jtu.register_pytree_with_keys(
+            cls,
+            partial(_node_flatten, with_keys=True),
+            _node_unflatten,
+            flatten_func=partial(_node_flatten, with_keys=False),
+        )
 
 
-def var_metadata(value: A, sharding: Sharding) -> VarMetadata[A]:
-    return VarMetadata(value, sharding)
+class Node(NodeBase[A]):
+    pass
 
 
-class Variable(Container[A], reprlib.Representable):
-    __slots__ = ("_collection", "_sharding")
+class Variable(Node[A]):
+    sharding: tp.Optional[Sharding]
 
     def __init__(
         self,
-        value: A,
-        collection: str,
-        sharding: tp.Optional[Sharding],
+        value: tp.Union[A, ContainerMetadata[A]],
+        sharding: tp.Optional[Sharding] = None,
+        **metadata: Any,
     ):
-        if isinstance(value, VarMetadata):
-            sharding = value.sharding if sharding is None else sharding
-            value = tp.cast(A, value.value)
+        super().__init__(value, sharding=sharding, **metadata)
 
-        self._value = value
-        self._collection = collection
-        self._sharding = sharding
 
-    def __eq__(self, other: object) -> bool:
-        return (
-            type(other) is Variable
-            and self._value == other._value
-            and self._collection == other._collection
-            and self._sharding == other._sharding
-        )
+class Param(Variable[A]):
+    pass
 
-    @property
-    def collection(self) -> str:
-        return self._collection
-
-    @property
-    def sharding(self) -> tp.Optional[Sharding]:
-        return self._sharding
 
-    def __nnx_repr__(self):
-        yield reprlib.Object(type=type(self))
-        yield reprlib.Attr("collection", repr(self._collection))
-        yield reprlib.Attr(
-            "value", repr(self._value) if isinstance(self._value, str) else self._value
-        )
-        if self._sharding is not None:
-            yield reprlib.Attr("sharding", self._sharding)
+class BatchStat(Variable[A]):
+    pass
 
-    def copy(self) -> "Variable[A]":
-        return Variable(self._value, self._collection, self._sharding)
 
-    def _replace_value(
-        self,
-        value: B,
-    ) -> "Variable[B]":
-        return Variable(
-            value,
-            self._collection,
-            self._sharding,
-        )
+class Cache(Variable[A]):
+    pass
 
-    def is_equivalent(self, other: tp.Any) -> bool:
-        return (
-            type(other) is Variable
-            and self._collection == other._collection
-            and self._sharding == other._sharding
-        )
 
-
-def _variable_flatten(
-    x: Variable[tp.Any],
-    *,
-    with_keys: bool,
-):
-    if with_keys:
-        node = (jtu.GetAttrKey("value"), x._value)
-    else:
-        node = x._value
-
-    return (node,), (x._collection, x._sharding)
-
-
-def _variable_unflatten(
-    metadata: tp.Tuple[str, tp.Optional[Sharding]], children: tp.Tuple[A]
-) -> Variable[A]:
-    return Variable(children[0], *metadata)
-
-
-jtu.register_pytree_with_keys(
-    Variable,
-    partial(_variable_flatten, with_keys=True),
-    _variable_unflatten,
-    flatten_func=partial(_variable_flatten, with_keys=False),
-)
+class Intermediate(Variable[A]):
+    pass
 
 
 class Static(Container[A], reprlib.Representable):
-    def __hash__(self) -> int:
-        return hash(self._value)
-
-    def __eq__(self, other: tp.Any) -> bool:
-        return type(other) is Static and self._value == other._value
-
-    def copy(self) -> "Static[A]":
-        return Static(self._value)
-
-    def _replace_value(
-        self,
-        value: B,
-    ) -> "Static[B]":
-        return Static(value)
-
-    def is_equivalent(self, other: tp.Any) -> bool:
-        return type(other) is Static
+    def __init__(self, value: A):
+        super().__init__(value)
 
-    def __nnx_repr__(self):
-        yield reprlib.Object(type=type(self))
-        yield reprlib.Attr(
-            "value", repr(self._value) if isinstance(self._value, str) else self._value
-        )
+    def __hash__(self) -> int:
+        return hash(self.value)
 
 
 def _static_flatten(x: Static[tp.Any]):
-    return (), x._value
+    return (), x.value
 
 
 def _static_unflatten(metadata: A, _) -> Static[A]:
     return Static(metadata)
 
 
 jtu.register_pytree_node(Static, _static_flatten, _static_unflatten)
 
 
-# --------------------
-# constructors
-# --------------------
-
-
-def check_container(f: F, *, num_arg: int) -> F:
-    @functools.wraps(f)
-    def wrapper(*args, **kwargs):
-        args = list(args)
-        value = args[num_arg]
-
-        if isinstance(value, Container):
-            container = value
-            value = container.value
-        else:
-            container = None
-
-        args[num_arg] = value
-        output = f(*args, **kwargs)
-
-        if container is not None and not container.is_equivalent(output):
-            raise ValueError(f"Container {container} is not equivalent to {output}")
-
-        return output
+def with_metadata(
+    initializer: F,
+    **metadata: tp.Any,
+) -> F:
+    @functools.wraps(initializer)
+    def wrapper(*args):
+        return ContainerMetadata(initializer(*args), metadata=metadata)
 
     return wrapper  # type: ignore
 
 
-@partial(check_container, num_arg=1)
-def var(
-    collection: str,
-    value: A,
-    sharding: tp.Optional[Sharding] = None,
-) -> A:
-    return Variable(  # type: ignore
-        value,
-        collection=collection,
-        sharding=sharding,
-    )
-
-
-def param(
-    value: A,
-    sharding: tp.Optional[Sharding] = None,
-) -> A:
-    return var("params", value, sharding=sharding)
-
-
-@partial(check_container, num_arg=0)
-def node(value: A) -> A:
-    return Node(value)  # type: ignore
-
-
-@partial(check_container, num_arg=0)
-def static(value: A) -> A:
-    return Static(value)  # type: ignore
-
-
 # register nodes
 nodes.register_node_type(Node)
-nodes.register_node_type(Variable)
```

### Comparing `nnx-0.0.6/nnx/contextlib.py` & `nnx-0.0.7/nnx/contextlib.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import builtins
+import dataclasses
 import hashlib
 import typing as tp
-from types import MappingProxyType
 
 import jax
 import jax.tree_util as jtu
 
 from nnx import errors, tracers
 
 KeyArray = jax.Array
@@ -16,90 +16,14 @@
     hash_str = " ".join(str(x) for x in data)
     _hash = hashlib.blake2s(hash_str.encode())
     hash_bytes = _hash.digest()
     # uint32 is represented as 4 bytes in big endian
     return int.from_bytes(hash_bytes[:4], byteorder="big")
 
 
-class RngStream:
-    __slots__ = ("_key", "_count", "_count_path", "_trace_state")
-
-    def __init__(self, key: KeyArray, count: int = 0, count_path: Counts = ()):
-        self._key = key
-        self._count = count
-        self._count_path = count_path
-        self._trace_state = tracers.TraceState()
-
-    @property
-    def count(self) -> int:
-        return self._count
-
-    @property
-    def count_path(self) -> Counts:
-        return self._count_path
-
-    def make_rng(self) -> jax.random.KeyArray:
-        if not self._trace_state.is_valid():
-            raise errors.TraceContextError(
-                "Cannot use RngStream from a different trace level"
-            )
-
-        fold_data = _stable_hash(self._count_path + (self._count,))
-        self._count += 1
-        return jax.random.fold_in(self._key, fold_data)
-
-    def fork(self) -> "RngStream":
-        if not self._trace_state.is_valid():
-            raise errors.TraceContextError(
-                "Cannot use RngStream from a different trace level"
-            )
-        count_path = self._count_path + (self._count,)
-        self._count += 1
-        return RngStream(self._key, count_path=count_path)
-
-    def split(self, n: int = 2) -> "RngStream":
-        if not self._trace_state.is_valid():
-            raise errors.TraceContextError(
-                "Cannot use RngStream from a different trace level"
-            )
-        key = self.make_rng()
-        key = jax.random.split(key, n)
-        return RngStream(key)
-
-
-def _rng_stream_flatten_with_keys(
-    rng: RngStream,
-) -> tp.Tuple[
-    tp.Tuple[tp.Tuple[tp.Hashable, jax.random.KeyArray], ...],
-    tp.Tuple[int, Counts],
-]:
-    return ((jtu.GetAttrKey("key"), rng._key),), (rng.count, rng.count_path)
-
-
-def _rng_stream_unflatten(
-    aux_data: tp.Tuple[int, Counts],
-    children: tp.Tuple[jax.random.KeyArray, ...],
-) -> RngStream:
-    count, count_path = aux_data
-    key = children[0]
-    return RngStream(key, count, count_path)
-
-
-def _rng_stream_flatten(rng: RngStream):
-    return (rng._key,), (rng.count, rng.count_path)
-
-
-jax.tree_util.register_pytree_with_keys(
-    RngStream,
-    _rng_stream_flatten_with_keys,
-    _rng_stream_unflatten,
-    flatten_func=_rng_stream_flatten,
-)
-
-
 class ContextDef:
     __slots__ = ("_rng_counts", "_flags")
 
     def __init__(
         self,
         rng_counts: tp.Tuple[tp.Tuple[str, Counts], ...],
         flags: tp.Tuple[tp.Tuple[str, bool], ...],
@@ -134,53 +58,79 @@
 
 def _pure_context_flatten(pure_context: PureContext):
     return tuple(pure_context), None
 
 
 def _pure_context_unflatten(
     aux_data: None,
-    children: tp.Tuple[tp.Dict[str, RngStream], ContextDef],
+    children: tp.Tuple[tp.Dict[str, KeyArray], ContextDef],
 ) -> PureContext:
     return PureContext(children)
 
 
 jtu.register_pytree_node(PureContext, _pure_context_flatten, _pure_context_unflatten)
 
 
+@dataclasses.dataclass
+class RngStream:
+    key: KeyArray
+    count: int = 0
+    count_path: Counts = ()
+
+
 class Context:
-    __slots__ = ("_rngs", "_flags")
+    __slots__ = ("_rngs", "_flags", "_trace_state")
 
     def __init__(
         self,
         rngs: tp.Mapping[str, RngStream],
         flags: tp.Mapping[str, bool],
     ):
         self._rngs = rngs
         self._flags = flags
+        self._trace_state = tracers.TraceState()
 
     def has_rng(self, name: str) -> bool:
         return name in self._rngs
 
     def make_rng(self, name: str) -> KeyArray:
         if name not in self._rngs:
             raise ValueError(f"Unknown Rng Stream: {name}")
-        return self._rngs[name].make_rng()
+        elif not self._trace_state.is_valid():
+            raise errors.TraceContextError(
+                "Cannot use Context from a different trace level"
+            )
+
+        stream = self._rngs[name]
+        fold_data = _stable_hash(stream.count_path + (stream.count,))
+        stream.count += 1
+        return jax.random.fold_in(stream.key, fold_data)
 
     def copy(self) -> "Context":
         return Context(rngs=self._rngs, flags=self._flags)
 
     def has_flag(self, name: str) -> bool:
         return name in self._flags
 
     def get_flag(self, name: str) -> tp.Optional[bool]:
         return self._flags.get(name, None)
 
     def partition(self) -> PureContext:
-        rngs = {name: stream.fork() for name, stream in self._rngs.items()}
-        keys = {name: stream._key for name, stream in rngs.items()}
+        if not self._trace_state.is_valid():
+            raise errors.TraceContextError(
+                "Cannot use Context from a different trace level"
+            )
+
+        def fork(stream) -> "RngStream":
+            count_path = stream.count_path + (stream.count,)
+            stream.count += 1
+            return RngStream(stream.key, count_path=count_path)
+
+        rngs = {name: fork(stream) for name, stream in self._rngs.items()}
+        keys = {name: stream.key for name, stream in rngs.items()}
         rng_counts = tuple((name, stream.count_path) for name, stream in rngs.items())
         return PureContext.new(keys, ContextDef(rng_counts, tuple(self._flags.items())))
 
 
 def context(
     params: tp.Union[int, KeyArray, RngStream, None] = None,
     *,
@@ -207,24 +157,31 @@
 if tp.TYPE_CHECKING:
     ellipsis = builtins.ellipsis
 else:
     ellipsis = tp.Any
 
 RngPredicate = tp.Callable[[str], bool]
 RngFilterLiteral = tp.Union[str, RngPredicate, ellipsis, None]
-RngFilter = tp.Union[RngFilterLiteral, tp.Sequence[RngFilterLiteral]]
+RngFilter = tp.Union[
+    RngFilterLiteral, tp.Sequence[RngFilterLiteral], tp.Mapping[RngFilterLiteral, bool]
+]
 
 
 def to_rng_predicate(filter: RngFilter) -> RngPredicate:
     if filter is None:
         return lambda _: False
     elif filter is ...:
         return lambda _: True
     elif callable(filter):
         return filter
     elif isinstance(filter, str):
         return lambda name: name == filter
-    elif isinstance(filter, tuple):
+    elif isinstance(filter, tp.Mapping):
+        predicates = tuple(
+            to_rng_predicate(filter) for filter, include in filter.items() if include
+        )
+        return lambda name: any(predicate(name) for predicate in predicates)
+    elif isinstance(filter, tp.Sequence):
         predicates = tuple(map(to_rng_predicate, filter))
         return lambda name: any(predicate(name) for predicate in predicates)
     else:
         raise TypeError(f"Invalid rng filter: {filter}")
```

### Comparing `nnx-0.0.6/nnx/dataclasses.py` & `nnx-0.0.7/nnx/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         metadata = {}
     else:
         metadata = dict(metadata)
 
     if "nnx_container_fn" in metadata:
         raise ValueError("'nnx_container_fn' found in metadata")
 
-    metadata["nnx_container_fn"] = lambda value: containers.node(value)
+    metadata["nnx_container_fn"] = lambda value: containers.Node(value)
 
     return field(
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
         hash=hash,
@@ -74,29 +74,29 @@
         metadata = {}
     else:
         metadata = dict(metadata)
 
     if "nnx_container_fn" in metadata:
         raise ValueError("'nnx_container_fn' found in metadata")
 
-    metadata["nnx_container_fn"] = lambda value: containers.static(value)
+    metadata["nnx_container_fn"] = lambda value: containers.Static(value)
 
     return field(
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
         hash=hash,
         compare=compare,
         metadata=metadata,
     )
 
 
 def var_field(
-    collection: str,
+    variable_type: tp.Type[containers.Variable[tp.Any]],
     *,
     default: tp.Any = dataclasses.MISSING,
     default_factory: tp.Any = dataclasses.MISSING,
     init: bool = True,
     repr: bool = True,
     hash: tp.Optional[bool] = None,
     compare: bool = True,
@@ -107,17 +107,15 @@
         metadata = {}
     else:
         metadata = dict(metadata)
 
     if "nnx_container_fn" in metadata:
         raise ValueError("'nnx_container_fn' found in metadata")
 
-    metadata["nnx_container_fn"] = lambda value: containers.var(
-        collection, value, sharding=sharding
-    )
+    metadata["nnx_container_fn"] = lambda value: variable_type(value, sharding=sharding)
 
     return field(
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
         hash=hash,
@@ -133,15 +131,15 @@
     init: bool = True,
     repr: bool = True,
     hash: tp.Optional[bool] = None,
     compare: bool = True,
     metadata: tp.Optional[tp.Mapping[str, tp.Any]] = None,
 ) -> tp.Any:
     return var_field(
-        "params",
+        containers.Param,
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
         hash=hash,
         compare=compare,
         metadata=metadata,
```

### Comparing `nnx-0.0.6/nnx/helpers.py` & `nnx-0.0.7/nnx/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import inspect
 import typing as tp
 
+import jax.numpy as jnp
 import optax
 
-from nnx import containers, pytreelib, utils
+from nnx import pytreelib
 from nnx.contextlib import Context
-from nnx.module import ApplyCaller, Module, Pure
+from nnx.module import ApplyCaller, Module, ModuleDef, Pure
 from nnx.state import State
 
 A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound=Module)
 
 
 class Dict(Module, tp.Mapping[str, A]):
@@ -74,15 +76,15 @@
                     kwargs = {}
                 elif isinstance(output, tp.Dict):
                     args = ()
                     kwargs = output
                 else:
                     args = (output,)
                     kwargs = {}
-            if ctx is not None and utils.has_keyword_arg(f, "ctx"):
+            if ctx is not None and has_keyword_arg(f, "ctx"):
                 kwargs["ctx"] = ctx
 
             output = f(*args, **kwargs)
 
         return output
 
 
@@ -90,37 +92,58 @@
     def __call__(self, state: State, *states: State) -> ApplyCaller["Pure[M]"]:
         ...
 
 
 class TrainState(pytreelib.Pytree, tp.Generic[M]):
     def __init__(
         self,
+        moduledef: ModuleDef[M],
         *,
-        apply_fn: ModuleDefApply[M],
         params: State,
         tx: optax.GradientTransformation,
         step: int = 0,
         **kwargs,
     ):
-        self.apply_fn = apply_fn
-        self.params: State = containers.node(params)
+        self.moduledef = moduledef
+        self.params: State = pytreelib.TreeNode(params)
         self.tx = tx
-        self.opt_state = containers.node(tx.init(self.params))
-        self.step = containers.node(step)
+        self.opt_state = pytreelib.TreeNode(tx.init(self.params))
+        self.step = pytreelib.TreeNode(jnp.asarray(step))
         for name, value in kwargs.items():
             setattr(self, name, value)
 
     if tp.TYPE_CHECKING:
 
         def __getattr__(self, key: str) -> tp.Any:
             ...
 
+    def apply(
+        self, state: tp.Union[State, str], *states: tp.Union[State, str]
+    ) -> ApplyCaller[Pure[State, M]]:
+        states = (state, *states)
+
+        _states = (
+            getattr(self, state) if isinstance(state, str) else state
+            for state in states
+        )
+
+        return self.moduledef.apply(*_states)
+
     def apply_gradients(self, grads: State, **kwargs) -> "TrainState[M]":
         updates, opt_state = self.tx.update(grads, self.opt_state, self.params)
         params = optax.apply_updates(self.params, updates)  # type: ignore
         step = self.step + 1
         return self.replace(
             params=params,
             opt_state=opt_state,
             step=step,
             **kwargs,
         )
+
+
+def has_keyword_arg(func: tp.Callable[..., tp.Any], name: str) -> bool:
+    """Return True if func has keyword-only arguments with the given name."""
+    return any(
+        param.name == name
+        and param.kind in (param.KEYWORD_ONLY, param.POSITIONAL_OR_KEYWORD)
+        for param in inspect.signature(func).parameters.values()
+    )
```

### Comparing `nnx-0.0.6/nnx/module.py` & `nnx-0.0.7/nnx/module.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,67 @@
 import dataclasses
 import typing as tp
 from abc import ABCMeta
 from typing import Any
 
 import jax.tree_util as jtu
 
-from nnx import errors, nodes, partitioning, reprlib, tracers, utils
-from nnx.containers import Container, Sharding, Variable
+from nnx import containers, errors, ids, nodes, partitioning, reprlib, tracers
+from nnx.containers import Container, Node, Sharding
 from nnx.state import State
 
 A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound="Module")
 S = tp.TypeVar("S", bound=tp.Union[State, tp.Tuple[State, ...]])
+V = tp.TypeVar("V", bound=containers.Variable[tp.Any])
 
-Path = tp.Tuple[str, ...]
+Path = str
+PathParts = tp.Tuple[str, ...]
 StateDict = tp.Dict[Path, tp.Any]
 StateMapping = tp.Mapping[Path, tp.Any]
 
 
+class _ProxyContext(tp.Protocol):
+    def __call__(self, __fn: tp.Callable[..., tp.Any], *args, **kwargs) -> tp.Any:
+        ...
+
+
+@dataclasses.dataclass
+class CallableProxy:
+    _proxy_context: _ProxyContext
+    _proxy_callable: tp.Callable[..., tp.Any]
+
+    def __call__(self, *args, **kwargs):
+        return self._proxy_context(self._proxy_callable, *args, **kwargs)
+
+    def __getattr__(self, name) -> "CallableProxy":
+        return CallableProxy(self._proxy_context, getattr(self._proxy_callable, name))
+
+    def __getitem__(self, key) -> "CallableProxy":
+        return CallableProxy(self._proxy_context, self._proxy_callable[key])
+
+
+def _identity(x):
+    return x
+
+
+@dataclasses.dataclass
+class DelayedAccessor:
+    accessor: tp.Callable[[tp.Any], tp.Any] = _identity
+
+    def __call__(self, x):
+        return self.accessor(x)
+
+    def __getattr__(self, name):
+        return DelayedAccessor(lambda x: getattr(x, name))
+
+    def __getitem__(self, key):
+        return DelayedAccessor(lambda x: x[key])
+
+
 class ApplyCaller(tp.Protocol, tp.Generic[A]):
     def __getattr__(self, __name) -> "ApplyCaller[A]":
         ...
 
     def __getitem__(self, __name) -> "ApplyCaller[A]":
         ...
 
@@ -99,23 +139,23 @@
         current_state = State({})
 
         _update_module(module, current_state, states)
 
         return module
 
     def apply(self, state: State, *states: State) -> ApplyCaller["Pure[State, M]"]:
-        accessesor = utils.DelayedAccessor()
+        accessesor = DelayedAccessor()
 
         def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, Pure[State, M]]:
             module = self.merge(state, *states)
             fn = accessesor(module)
             out = fn(*args, **kwargs)
             return out, module.partition()
 
-        return utils.CallableProxy(_context, accessesor)  # type: ignore
+        return CallableProxy(_context, accessesor)  # type: ignore
 
 
 def _moddef_flatten(moduledef: ModuleDef[M]):
     return (), (
         moduledef._type,
         moduledef._index,
         moduledef._submodules,
@@ -162,22 +202,22 @@
         if isinstance(self.states, tuple):
             return self.moduledef.apply(*self.states)
         else:
             return self.moduledef.apply(self.states)
 
     @property
     def call(self) -> M:
-        accessesor = utils.DelayedAccessor()
+        accessesor = DelayedAccessor()
 
         def _context(accessesor, *args, **kwargs):
             module = self.merge()
             fn = accessesor(module)
             return fn(*args, **kwargs)
 
-        return utils.CallableProxy(_context, accessesor)  # type: ignore
+        return CallableProxy(_context, accessesor)  # type: ignore
 
     def get_state(self) -> State:
         if isinstance(self.states, tuple):
             return State.merge(*self.states)
         return self.states
 
     @tp.overload
@@ -319,27 +359,32 @@
 
 
 jtu.register_pytree_node(Pure, _pure_module_flatten, _pure_module_unflatten)
 
 PureModule = Pure[tp.Union[State, tp.Tuple[State, ...]], M]
 
 
-SEEN_MODULES_REPR: tp.Set[int] = set()
+SEEN_MODULES_REPR: tp.Optional[tp.Set[ids.UUID]] = None
 
 
 class ModuleState(reprlib.Representable):
-    __slots__ = ("_trace_state",)
+    __slots__ = ("_trace_state", "_id")
 
     def __init__(self, trace_state: tracers.TraceState):
         self._trace_state = trace_state
+        self._id = ids.uuid()
 
     @property
     def trace_state(self) -> tracers.TraceState:
         return self._trace_state
 
+    @property
+    def id(self) -> ids.UUID:
+        return self._id
+
     def __nnx_repr__(self):
         yield reprlib.Object(type(self))
         yield reprlib.Attr("trace_state", self._trace_state)
 
 
 class ModuleMeta(ABCMeta):
     if not tp.TYPE_CHECKING:
@@ -362,62 +407,78 @@
                 value = vars(module)[field.name]
                 value = container_fn(value)
                 vars(module)[field.name] = value
 
         return module
 
 
+@tp.runtime_checkable
+class HasUnboxFn(tp.Protocol):
+    unbox_fn: tp.Callable[["Container[tp.Any]"], tp.Any]
+
+
 class Module(reprlib.Representable, metaclass=ModuleMeta):
     if tp.TYPE_CHECKING:
         _module__state: ModuleState
 
     if not tp.TYPE_CHECKING:
 
         def __getattribute__(self, name: str) -> Any:
             value = object.__getattribute__(self, name)
             if isinstance(value, Container):
+                if isinstance(value, HasUnboxFn):
+                    return value.unbox_fn(value)
                 return value.value
             return value
 
         def __setattr__(self, name: str, value: Any) -> None:
             self._setattr(name, value)
 
     def _setattr(self, name: str, value: Any) -> None:
         if not self._module__state.trace_state.is_valid():
             raise errors.TraceContextError(
                 "Cannot mutate Module from different trace level"
             )
 
         vars_dict = vars(self)
         if name in vars_dict and isinstance(vars_dict[name], Container):
-            vars_dict[name] = vars_dict[name].replace_value(value)
+            vars_dict[name] = vars_dict[name].replace(value=value)
         else:
             if isinstance(value, Container):
                 value = value.copy()
             vars_dict[name] = value
 
     def __hash__(self) -> int:
-        return id(self)
+        return hash(self._module__state.id)
 
     def __nnx_repr__(self):
-        if id(self) in SEEN_MODULES_REPR:
+        global SEEN_MODULES_REPR
+
+        if SEEN_MODULES_REPR is None:
+            SEEN_MODULES_REPR = set()
+            clear_seen = True
+        else:
+            clear_seen = False
+
+        if self._module__state.id in SEEN_MODULES_REPR:
             yield reprlib.Object(type=type(self), empty_repr="...")
             return
 
         yield reprlib.Object(type=type(self))
-        SEEN_MODULES_REPR.add(id(self))
+        SEEN_MODULES_REPR.add(self._module__state.id)
 
         try:
             for name, value in vars(self).items():
                 if isinstance(value, Module) or (
                     not nodes.is_node(value) and not name.startswith("_")
                 ):
                     yield reprlib.Attr(name, value)
         finally:
-            SEEN_MODULES_REPR.remove(id(self))
+            if clear_seen:
+                SEEN_MODULES_REPR = None
 
     def clone(self: M) -> M:
         return self.partition().merge()
 
     @tp.overload
     def partition(self: M) -> Pure[State, M]:
         ...
@@ -453,14 +514,17 @@
             return Pure.new(states, moduledef)
         else:
             return Pure.new(states, moduledef)
 
     def get_state(self) -> State:
         return _get_module_state(self)
 
+    def get_module_def(self: M) -> ModuleDef[M]:
+        return _get_module_def(self)
+
     @tp.overload
     def filter(self, first: partitioning.Filter, /) -> State:
         ...
 
     @tp.overload
     def filter(
         self,
@@ -515,23 +579,23 @@
         if len(states) == 1:
             return states[0]
         else:
             return states
 
     @property
     def apply(self: M) -> ApplyCaller[M]:
-        accessesor = utils.DelayedAccessor()
+        accessesor = DelayedAccessor()
 
         def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, M]:
             module = self.clone()
             fn = accessesor(module)
             out = fn(*args, **kwargs)
             return out, module
 
-        return utils.CallableProxy(_context, accessesor)  # type: ignore
+        return CallableProxy(_context, accessesor)  # type: ignore
 
     def update_state(
         self: M,
         updates: tp.Union[M, Pure[S, M], State, tp.Tuple[State, ...]],
     ) -> None:
         current_state = _get_module_state(self)
 
@@ -539,34 +603,66 @@
             updates = updates.states
         elif isinstance(updates, Module):
             assert type(self) == type(updates)
             updates = _get_module_state(updates)
 
         _update_module(self, current_state, updates)
 
-    @tp.overload
     def mutable_state_dict(self) -> tp.Dict[Path, "MutableLeaf"]:
-        ...
+        return {path: MutableLeaf(self, path) for path, _ in _iter_state(self)}
 
-    @tp.overload
-    def mutable_state_dict(self, sep: str) -> tp.Dict[str, "MutableLeaf"]:
-        ...
-
-    def mutable_state_dict(
-        self, sep: tp.Optional[str] = None
-    ) -> tp.Union[tp.Dict[Path, "MutableLeaf"], tp.Dict[str, "MutableLeaf"]]:
-        mutable_leaves = (
-            (path, MutableLeaf(self, path)) for path, _ in _iter_state(self)
-        )
-        if sep is not None:
-            state = {sep.join(path): leaf for path, leaf in mutable_leaves}
+    def sow(
+        self,
+        variable_type: tp.Type[containers.Variable],
+        name: str,
+        value: tp.Any,
+    ) -> None:
+        if hasattr(self, name):
+            variable = vars(self)[name]
+            if not isinstance(variable, containers.Variable):
+                raise ValueError(
+                    f"Expected '{name}' to be a Variable, got {type(variable).__name__}"
+                )
+            elif type(variable) != variable_type:
+                raise ValueError(
+                    f"Expected '{name}' to be of type '{variable_type.__name__}', "
+                    f"got '{type(variable).__name__}'"
+                )
+            current_value = variable.value
+            if not isinstance(current_value, tuple):
+                raise ValueError(
+                    f"Expected '{name}' to be a tuple, "
+                    f"got {type(current_value).__name__}"
+                )
+            value = current_value + (value,)
+            setattr(self, name, value)
         else:
-            state = {path: leaf for path, leaf in mutable_leaves}
+            setattr(self, name, variable_type((value,)))
+
+    def for_each(self, module_type: tp.Type[M], fn: tp.Callable[[M], None]) -> None:
+        visited: tp.Set[ids.UUID] = set()
+        self._on_all(module_type, fn, visited)
+
+    def _on_all(
+        self,
+        module_type: tp.Type[M],
+        fn: tp.Callable[[M], None],
+        visited: tp.Set[ids.UUID],
+    ) -> None:
+        if self._module__state.id in visited:
+            return
+
+        visited.add(self._module__state.id)
 
-        return state
+        if isinstance(self, module_type):
+            fn(self)
+
+        for value in vars(self).values():
+            if isinstance(value, Module):
+                value._on_all(module_type, fn, visited)
 
     # Pytree Definition
     # def __init_subclass__(cls) -> None:
     #     super().__init_subclass__()
 
     #     def _flatten(module: Module, *, with_keys: bool):
     #         state, moduledef = module.partition()
@@ -596,73 +692,66 @@
     #     )
 
 
 class MutableLeaf(reprlib.Representable):
     __slots__ = ("_module", "_name")
 
     def __init__(self, root: Module, path: Path):
-        *module_path, name = path
+        path_parts = path.split("/")
+        *module_path, name = path_parts
         module = _get_value_path(root, module_path)
         if not isinstance(module, Module):
             raise ValueError(
-                f"Expected a module at path {path[:-1]}, ",
+                f"Expected a module at path {path_parts[:-1]}, ",
                 f" got {type(module).__name__}",
             )
         self._module = module
         self._name = name
 
     @property
     def value(self) -> tp.Any:
         return getattr(self._module, self._name)
 
     @value.setter
     def value(self, value: tp.Any) -> None:
         setattr(self._module, self._name, value)
 
     @property
-    def collection(self) -> tp.Optional[str]:
-        module = vars(self._module)[self._name]
-        if not isinstance(module, Variable):
-            return None
-
-        return module.collection
-
-    @property
     def sharding(self) -> tp.Optional[Sharding]:
-        module = vars(self._module)[self._name]
-        if not isinstance(module, Variable):
+        attr = vars(self._module)[self._name]
+        if not isinstance(attr, Node):
             return None
 
-        return module.sharding
+        return attr.metadata.get("sharding", None)
 
 
 def _get_module_state(module: Module) -> State:
     return State(_iter_state(module))
 
 
 def _get_module_def(module: M) -> ModuleDef[M]:
-    module_index: tp.Dict[int, int] = {}
-    path: Path = ()
+    module_index: tp.Dict[ids.UUID, int] = {}
+    path: PathParts = ()
 
     moduledef = _make_module_def_recursive(module, module_index, path)
     assert isinstance(moduledef, ModuleDef)
 
     return moduledef
 
 
 def _make_module_def_recursive(
     module: M,
-    module_index: tp.Dict[int, int],
-    path: Path,
+    module_index: tp.Dict[ids.UUID, int],
+    path: PathParts,
 ) -> tp.Union[ModuleDef[M], int]:
-    if id(module) in module_index:
-        return module_index[id(module)]
+    if module._module__state.id in module_index:
+        return module_index[module._module__state.id]
 
     index = len(module_index)
-    module_index[id(module)] = index
+    module_index[module._module__state.id] = index
 
     submodules = []
     static_fields = []
 
     for name, value in sorted(vars(module).items(), key=lambda x: x[0]):
         value_path = (*path, name)
         if isinstance(value, Module):
@@ -677,41 +766,44 @@
         submodules=tuple(submodules),
         static_fields=tuple(static_fields),
     )
     return module_def
 
 
 def _iter_state(module: Module) -> tp.Iterator[tp.Tuple[Path, tp.Any]]:
-    seen_modules: tp.Set[int] = set()
-    path: Path = ()
+    seen_modules: tp.Set[ids.UUID] = set()
+    path_parts: PathParts = ()
 
-    yield from _iter_state_recursive(module, seen_modules, path)
+    yield from _iter_state_recursive(module, seen_modules, path_parts)
 
 
 def _iter_state_recursive(
-    module: Module, seen_modules: tp.Set[int], path: Path
+    module: Module, seen_modules: tp.Set[ids.UUID], path_parts: PathParts
 ) -> tp.Iterator[tp.Tuple[Path, tp.Any]]:
-    if id(module) in seen_modules:
+    if module._module__state.id in seen_modules:
         return
 
-    seen_modules.add(id(module))
+    seen_modules.add(module._module__state.id)
 
     for name, value in sorted(vars(module).items(), key=lambda x: x[0]):
-        value_path = (*path, name)
+        new_path_parts = (*path_parts, name)
         if isinstance(value, Module):
-            yield from _iter_state_recursive(value, seen_modules, value_path)
+            yield from _iter_state_recursive(value, seen_modules, new_path_parts)
         elif nodes.is_node(value):
-            yield value_path, value
+            path = "/".join(new_path_parts)
+            yield path, value
 
 
-def _set_value_at_path(module: tp.Any, path: tp.Sequence[str], value: tp.Any):
-    if len(path) == 1:
-        setattr(module, path[0], value)
+def _set_value_at_path(
+    module: tp.Any, path_parts: tp.Union[PathParts, tp.List[str]], value: tp.Any
+):
+    if len(path_parts) == 1:
+        setattr(module, path_parts[0], value)
     else:
-        _set_value_at_path(vars(module)[path[0]], path[1:], value)
+        _set_value_at_path(vars(module)[path_parts[0]], path_parts[1:], value)
 
 
 def _get_value_path(module: tp.Any, path: tp.Sequence[str]) -> tp.Any:
     if len(path) == 0:
         return module
     else:
         return _get_value_path(vars(module)[path[0]], path[1:])
@@ -748,48 +840,48 @@
     return module
 
 
 def _pop(
     module: Module,
     filters: tp.Tuple[partitioning.Filter, ...],
 ) -> tp.Tuple[State, ...]:
-    module_index: tp.Dict[int, int] = {}
-    path: Path = ()
+    module_index: tp.Dict[ids.UUID, int] = {}
+    path_parts: PathParts = ()
     predicates = tuple(partitioning.to_predicate(filter) for filter in filters)
     states = tuple({} for _ in predicates)
-    _pop_recursive(module, module_index, path, states, predicates)
+    _pop_recursive(module, module_index, path_parts, states, predicates)
 
     return tuple(State(x) for x in states)
 
 
 def _pop_recursive(
     module: Module,
-    module_index: tp.Dict[int, int],
-    path: Path,
+    module_index: tp.Dict[ids.UUID, int],
+    path_parts: PathParts,
     states: tp.Tuple[tp.Dict[Path, tp.Any]],
     predicates: tp.Tuple[partitioning.Predicate, ...],
 ) -> None:
-    if id(module) in module_index:
+    if module._module__state.id in module_index:
         return
 
     for name, value in list(vars(module).items()):
-        value_path = (*path, name)
         if isinstance(value, Module):
-            _pop_recursive(value, module_index, value_path, states, predicates)
+            _pop_recursive(value, module_index, (*path_parts, name), states, predicates)
             continue
         elif not nodes.is_node(value):
             continue
 
+        path = "/".join((*path_parts, name))
         for state, predicate in zip(states, predicates):
-            if predicate(value_path, value):
-                state[value_path] = value
+            if predicate(path, value):
+                state[path] = value
                 delattr(module, name)
                 break
 
-    module_index[id(module)] = len(module_index)
+    module_index[module._module__state.id] = len(module_index)
 
 
 def _update_module(
     module: Module, current_state: State, updates: tp.Union[State, tp.Tuple[State, ...]]
 ) -> None:
     new_states = [current_state]
 
@@ -799,13 +891,21 @@
         new_states.extend(updates)
 
     state: StateDict = {}
     for new_state in new_states:
         state.update(new_state)
 
     for path, value in state.items():
-        _set_value_at_path(module, path, value)
+        path_parts = path.split("/")
+        _set_value_at_path(module, path_parts, value)
+
+
+def first_from(*args: tp.Optional[A]) -> A:
+    """Return the first non-None argument."""
+    for arg in args:
+        if arg is not None:
+            return arg
+    raise ValueError("No non-None arguments found.")
 
 
 # register nodes
-nodes.register_node_type(Module)
 nodes.register_node_type(Pure)
```

### Comparing `nnx-0.0.6/nnx/nn/activations.py` & `nnx-0.0.7/nnx/nn/activations.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.6/nnx/nn/dtypes.py` & `nnx-0.0.7/nnx/nn/dtypes.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.6/nnx/nn/initializers.py` & `nnx-0.0.7/nnx/nn/initializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import typing as tp
+
 import jax
-from jax.nn.initializers import Initializer as Initializer
+import jax.numpy as jnp
 from jax.nn.initializers import constant as constant
 from jax.nn.initializers import delta_orthogonal as delta_orthogonal
 from jax.nn.initializers import glorot_normal as glorot_normal
 from jax.nn.initializers import glorot_uniform as glorot_uniform
 from jax.nn.initializers import he_normal as he_normal
 from jax.nn.initializers import he_uniform as he_uniform
 from jax.nn.initializers import kaiming_normal as kaiming_normal
@@ -13,14 +15,27 @@
 from jax.nn.initializers import normal as normal
 from jax.nn.initializers import orthogonal as orthogonal
 from jax.nn.initializers import uniform as uniform
 from jax.nn.initializers import variance_scaling as variance_scaling
 from jax.nn.initializers import xavier_normal as xavier_normal
 from jax.nn.initializers import xavier_uniform as xavier_uniform
 
+Shape = tp.Sequence[int]
+DTypeLikeInexact = tp.Any
+KeyArray = jax.random.KeyArray
+Array = jax.Array
+
+
+class Initializer(tp.Protocol):
+    @staticmethod
+    def __call__(
+        key: KeyArray, shape: Shape, dtype: DTypeLikeInexact = jnp.float_
+    ) -> Array:
+        ...
+
 
 def zeros() -> Initializer:
     """Builds an initializer that returns a constant array full of zeros.
 
     >>> import jax, jax.numpy as jnp
     >>> from flax.linen.initializers import zeros_init
     >>> zeros_initializer = zeros_init()
```

### Comparing `nnx-0.0.6/nnx/nn/linear.py` & `nnx-0.0.7/nnx/nn/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,22 +84,22 @@
         precision: PrecisionLike = None,
         kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = default_kernel_init,
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         dot_general: DotGeneralT = lax.dot_general,
         ctx: contextlib.Context,
     ):
         kernel_key = ctx.make_rng("params")
-        self.kernel = nnx.param(
+        self.kernel = nnx.Param(
             kernel_init(kernel_key, (in_features, out_features), param_dtype)
         )
         if use_bias:
             bias_key = ctx.make_rng("params")
-            self.bias = nnx.param(bias_init(bias_key, (out_features,), param_dtype))
+            self.bias = nnx.Param(bias_init(bias_key, (out_features,), param_dtype))
         else:
-            self.bias = nnx.param(None)
+            self.bias = nnx.Param(None)
 
         self.in_features = in_features
         self.out_features = out_features
         self.use_bias = use_bias
         self.dtype = dtype
         self.param_dtype = param_dtype
         self.precision = precision
@@ -202,22 +202,22 @@
             kernel_size = tuple(kernel_size)
 
         kernel_shape = kernel_size + (
             in_features // feature_group_count,
             out_features,
         )
         kernel_key = ctx.make_rng("params")
-        self.kernel = nnx.param(kernel_init(kernel_key, kernel_shape, param_dtype))
+        self.kernel = nnx.Param(kernel_init(kernel_key, kernel_shape, param_dtype))
 
         if use_bias:
             bias_shape = (out_features,)
             bias_key = ctx.make_rng("params")
-            self.bias = nnx.param(bias_init(bias_key, bias_shape, param_dtype))
+            self.bias = nnx.Param(bias_init(bias_key, bias_shape, param_dtype))
         else:
-            self.bias = nnx.param(None)
+            self.bias = nnx.Param(None)
 
         self.in_features = in_features
         self.out_features = out_features
         self.kernel_size = kernel_size
         self.strides = strides
         self.padding = padding
         self.input_dilation = input_dilation
@@ -364,15 +364,15 @@
         dtype: tp.Optional[Dtype] = None,
         param_dtype: Dtype = jnp.float32,
         embedding_init: tp.Callable[
             [PRNGKey, Shape, Dtype], Array
         ] = default_embed_init,
         ctx: contextlib.Context,
     ):
-        self.embedding = nnx.param(
+        self.embedding = nnx.Param(
             embedding_init(
                 ctx.make_rng("params"), (num_embeddings, features), param_dtype
             )
         )
 
         self.num_embeddings = num_embeddings
         self.features = features
```

### Comparing `nnx-0.0.6/nnx/nn/normalization.py` & `nnx-0.0.7/nnx/nn/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing as tp
 
 import jax
 import jax.numpy as jnp
 from jax import lax
 
 import nnx
-from nnx import contextlib, utils
-from nnx.module import Module
+from nnx import contextlib
+from nnx.module import Module, first_from
 from nnx.nn import dtypes, initializers
 
 PRNGKey = jax.Array
 Array = jax.Array
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
 
@@ -190,28 +190,28 @@
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones(),
         axis_name: tp.Optional[str] = None,
         axis_index_groups: tp.Any = None,
         ctx: contextlib.Context,
     ):
         feature_shape = (num_features,)
-        self.mean = nnx.var("batch_stats", jnp.zeros(feature_shape, jnp.float32))
-        self.var = nnx.var("batch_stats", jnp.ones(feature_shape, jnp.float32))
+        self.mean = nnx.BatchStat(jnp.zeros(feature_shape, jnp.float32))
+        self.var = nnx.BatchStat(jnp.ones(feature_shape, jnp.float32))
 
         if use_scale:
             key = ctx.make_rng("params")
-            self.scale = nnx.param(scale_init(key, feature_shape, param_dtype))
+            self.scale = nnx.Param(scale_init(key, feature_shape, param_dtype))
         else:
-            self.scale = nnx.param(None)
+            self.scale = nnx.Param(None)
 
         if use_bias:
             key = ctx.make_rng("params")
-            self.bias = nnx.param(bias_init(key, feature_shape, param_dtype))
+            self.bias = nnx.Param(bias_init(key, feature_shape, param_dtype))
         else:
-            self.bias = nnx.param(None)
+            self.bias = nnx.Param(None)
 
         self.num_features = num_features
         self.use_running_average = use_running_average
         self.axis = axis
         self.momentum = momentum
         self.epsilon = epsilon
         self.dtype = dtype
@@ -237,15 +237,15 @@
           use_running_average: if true, the statistics stored in batch_stats
             will be used instead of computing the batch statistics on the input.
 
         Returns:
           Normalized inputs (the same shape as inputs).
         """
 
-        use_running_average = utils.first_from(
+        use_running_average = first_from(
             use_running_average,
             self.use_running_average,
             ctx and ctx.get_flag("use_running_average"),
         )
         feature_axes = _canonicalize_axes(x.ndim, self.axis)
         reduction_axes = tuple(i for i in range(x.ndim) if i not in feature_axes)
 
@@ -324,23 +324,23 @@
         axis_index_groups: tp.Any = None,
         ctx: contextlib.Context,
     ):
         feature_shape = (num_features,)
 
         if use_scale:
             key = ctx.make_rng("params")
-            self.scale = nnx.param(scale_init(key, feature_shape, param_dtype))
+            self.scale = nnx.Param(scale_init(key, feature_shape, param_dtype))
         else:
-            self.scale = nnx.param(None)
+            self.scale = nnx.Param(None)
 
         if use_bias:
             key = ctx.make_rng("params")
-            self.bias = nnx.param(bias_init(key, feature_shape, param_dtype))
+            self.bias = nnx.Param(bias_init(key, feature_shape, param_dtype))
         else:
-            self.bias = nnx.param(None)
+            self.bias = nnx.Param(None)
 
         self.num_features = num_features
         self.epsilon = epsilon
         self.dtype = dtype
         self.param_dtype = param_dtype
         self.use_bias = use_bias
         self.use_scale = use_scale
```

### Comparing `nnx-0.0.6/nnx/nn/stochastic.py` & `nnx-0.0.7/nnx/nn/stochastic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 from typing import Optional, Sequence
 
 import jax.numpy as jnp
 from jax import lax, random
 
-from nnx import contextlib, utils
-from nnx.module import Module
+from nnx import contextlib
+from nnx.module import Module, first_from
 
 
 @dataclasses.dataclass
 class Dropout(Module):
     """Create a dropout layer.
 
     Attributes:
@@ -40,15 +40,15 @@
           deterministic: if false the inputs are scaled by `1 / (1 - rate)` and
             masked, whereas if true, no mask is applied and the inputs are returned
             as is.
 
         Returns:
           The masked inputs reweighted to preserve mean.
         """
-        deterministic = utils.first_from(
+        deterministic = first_from(
             deterministic,
             self.deterministic,
             ctx and ctx.get_flag("deterministic"),
         )
 
         if (self.rate == 0.0) or deterministic:
             return inputs
```

### Comparing `nnx-0.0.6/nnx/partitioning.py` & `nnx-0.0.7/nnx/partitioning.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,45 +8,35 @@
 import nnx
 
 if tp.TYPE_CHECKING:
     ellipsis = builtins.ellipsis
 else:
     ellipsis = tp.Any
 
-Path = tp.Tuple[str, ...]
+Path = str
 Predicate = tp.Callable[[Path, tp.Any], bool]
-FilterLiteral = tp.Union[str, type, Predicate, ellipsis, None]
+FilterLiteral = tp.Union[type, Predicate, ellipsis, None]
 Filter = tp.Union[FilterLiteral, tp.Tuple[FilterLiteral, ...]]
 
 
 def to_predicate(filter: Filter) -> Predicate:
     if isinstance(filter, str):
-        return FromCollection(filter)
+        raise TypeError(f"Invalid filter of type '{type(filter).__name__}'")
     elif isinstance(filter, type):
         return OfType(filter)
     elif filter is Ellipsis:
         return Everything()
     elif filter is None:
         return Nothing()
     elif callable(filter):
         return filter
     elif isinstance(filter, tp.Tuple):
         return Any(*filter)
     else:
-        raise TypeError(f"Invalid collection filter: {filter}")
-
-
-@dataclasses.dataclass
-class FromCollection:
-    collection: str
-
-    def __call__(self, path: Path, x: tp.Any):
-        if isinstance(x, nnx.Variable):
-            return x.collection == self.collection
-        return False
+        raise TypeError(f"Invalid collection filter: {filter:!r}. ")
 
 
 @dataclasses.dataclass
 class OfType:
     type: type
 
     def __call__(self, path: Path, x: tp.Any):
```

### Comparing `nnx-0.0.6/nnx/pytreelib.py` & `nnx-0.0.7/nnx/pytreelib.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 from abc import ABCMeta
 from copy import copy
 from functools import partial
 from types import MappingProxyType
 
 import jax
 
-from nnx import nodes
-from nnx.containers import Container
+from nnx import containers, nodes, reprlib
 
 A = tp.TypeVar("A")
 P = tp.TypeVar("P", bound="Pytree")
 
 
+class TreeNode(containers.NodeBase[A]):
+    pass
+
+
 @contextlib.contextmanager
 def _mutable(obj: P) -> tp.Iterator[None]:
     vars(obj)["_pytree__is_mutable"] = True
     try:
         yield
     finally:
         del vars(obj)["_pytree__is_mutable"]
@@ -60,24 +63,24 @@
                 vars(obj)[field.name] = value
 
         vars(obj)["_pytree__sorted_fields"] = sorted(vars(obj))
 
         return obj
 
 
-class Pytree(metaclass=PytreeMeta):
+class Pytree(reprlib.Representable, metaclass=PytreeMeta):
     _pytree__is_mutable: bool
     _pytree__class_is_mutable: bool
     _pytree__sorted_fields: tp.Tuple[str, ...]
 
     if not tp.TYPE_CHECKING:
 
         def __getattribute__(self, name: str) -> tp.Any:
             value = object.__getattribute__(self, name)
-            if isinstance(value, Container):
+            if isinstance(value, containers.Container):
                 return value.value
             return value
 
         def __setattr__(self, name: str, value: tp.Any) -> None:
             self._setattr(name, value)
 
     def _setattr(self: P, name: str, value: tp.Any):
@@ -90,18 +93,18 @@
             "_pytree__is_mutable" not in vars_dict
             and not self._pytree__class_is_mutable
         ):
             raise AttributeError(
                 f"{type(self)} is immutable, trying to update field {name}"
             )
 
-        if name in vars_dict and isinstance(vars_dict[name], Container):
-            vars_dict[name] = vars_dict[name].replace_value(value)
+        if name in vars_dict and isinstance(vars_dict[name], containers.Container):
+            vars_dict[name] = vars_dict[name].replace(value=value)
         else:
-            if isinstance(value, Container):
+            if isinstance(value, containers.Container):
                 value = value.copy()
             vars_dict[name] = value
 
     def __init_subclass__(cls, mutable: bool = False):
         super().__init_subclass__()
         # init class variables
         cls._pytree__is_mutable = False
@@ -252,10 +255,16 @@
         pytree = copy(self)
         with _mutable(pytree):
             for key, value in kwargs.items():
                 setattr(pytree, key, value)
 
         return pytree
 
+    def __nnx_repr__(self):
+        yield reprlib.Object(type(self))
+        for name, value in vars(self).items():
+            yield reprlib.Attr(name, repr(value))
+
 
 # register node types
 nodes.register_node_type(Pytree)
+nodes.register_node_type(TreeNode)
```

### Comparing `nnx-0.0.6/nnx/reprlib.py` & `nnx-0.0.7/nnx/reprlib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.6/nnx/state.py` & `nnx-0.0.7/nnx/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 import typing as tp
 
 import jax
 import jax.tree_util as jtu
 
 from nnx import nodes, partitioning, reprlib
-from nnx.containers import Variable
+from nnx.containers import Node
 
 A = tp.TypeVar("A")
 
 Leaf = tp.Any
-Path = tp.Tuple[str, ...]
+Path = str
 StateDict = tp.Dict[Path, tp.Any]
 StateMapping = tp.Mapping[Path, tp.Any]
 
 
-class State(tp.Mapping[tp.Tuple[str, ...], Leaf], reprlib.Representable):
+class State(tp.Mapping[Path, Leaf], reprlib.Representable):
     __slots__ = ("_mapping",)
 
     def __init__(
         self,
         __input: tp.Union[
-            tp.Mapping[tp.Tuple[str, ...], Leaf],
-            tp.Iterator[tp.Tuple[tp.Tuple[str, ...], Leaf]],
+            tp.Mapping[Path, Leaf],
+            tp.Iterator[tp.Tuple[Path, Leaf]],
         ],
         /,
     ):
         if isinstance(__input, tp.Mapping):
             self._mapping = dict(sorted(__input.items(), key=lambda x: x[0]))
         else:
             self._mapping = dict(sorted(__input, key=lambda x: x[0]))
 
-    def get_collections(self) -> tp.Set[tp.Union[str, None]]:
-        return {
-            value.collection if isinstance(value, Variable) else None
-            for value in self._mapping.values()
-        }
-
-    def __getitem__(self, __key: tp.Tuple[str, ...]) -> Leaf:
+    def __getitem__(self, __key: Path) -> Leaf:
         return self._mapping[__key]
 
-    def __iter__(self) -> tp.Iterator[tp.Tuple[str, ...]]:
+    def __iter__(self) -> tp.Iterator[Path]:
         return iter(self._mapping)
 
     def __len__(self) -> int:
         return len(self._mapping)
 
     def __nnx_repr__(self):
         yield reprlib.Object(type(self), value_sep=": ", start="({", end="})")
 
         for k, v in self._mapping.items():
-            yield reprlib.Attr(str(k), v)
+            yield reprlib.Attr(repr(k), v)
 
     @tp.overload
     def partition(self, first: partitioning.Filter, /) -> "State":
         ...
 
     @tp.overload
     def partition(
```

### Comparing `nnx-0.0.6/nnx/tracers.py` & `nnx-0.0.7/nnx/tracers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.6/nnx/transforms.py` & `nnx-0.0.7/nnx/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import functools
 import typing as tp
 from types import MappingProxyType
 
 import jax
 import jax.numpy as jnp
 import jax.stages
+import jax.tree_util as jtu
 
-from nnx import contextlib, partitioning, tracers, utils
-from nnx.module import Module, ModuleDef, PureModule
+from nnx import containers, contextlib, partitioning, spmd, tracers
+from nnx.module import CallableProxy, DelayedAccessor, Module, ModuleDef, PureModule
 from nnx.state import State
 
 A = tp.TypeVar("A")
 C = tp.TypeVar("C")
 F = tp.TypeVar("F", bound=tp.Callable[..., tp.Any])
 G = tp.TypeVar("G", bound=tp.Callable[..., tp.Any])
 M = tp.TypeVar("M", bound=Module)
@@ -215,15 +216,15 @@
     reduce_axes: tp.Sequence[AxisName] = (),
 ) -> tp.Callable[..., tp.Tuple[State, tp.Any]]:
     ...
 
 
 def grad(
     fun: tp.Callable[..., tp.Any],
-    wrt: partitioning.Filter = "params",
+    wrt: partitioning.Filter = containers.Param,
     *,
     stateful: bool = True,
     has_aux: bool = False,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: tp.Sequence[AxisName] = (),
 ) -> tp.Callable[..., tp.Union[tp.Tuple[State, tp.Any], State]]:
@@ -244,43 +245,43 @@
 
 # NOTE: I don't understand why variable_broadcasts exists. Passing them as
 # captures to `scan_fn` makes it impossible to propagate state updates from
 # them. Maybe, there should only be `variable_carry` and `variable_axes`.
 class Scan(Module, tp.Generic[M]):
     def __init__(
         self,
-        module_type: tp.Type[M],
+        *,
+        module_constructor: tp.Callable[..., M],
         module_init_args: tp.Tuple[tp.Any, ...],
         module_init_kwargs: tp.Dict[str, tp.Any],
-        *,
-        variable_axes: tp.Mapping[partitioning.Filter, int] = MappingProxyType({}),
-        variable_broadcast: partitioning.Filter = None,
-        variable_carry: partitioning.Filter = ...,
-        split_rngs: contextlib.RngFilter = None,
-        in_axes=0,
-        out_axes=0,
-        length: tp.Optional[int] = None,
-        reverse: bool = False,
-        unroll: int = 1,
-        data_transform: tp.Optional[tp.Callable[..., tp.Any]] = None,
-        metadata_params: tp.Mapping[tp.Any, tp.Any] = {},
+        variable_axes: tp.Mapping[partitioning.Filter, int],
+        variable_broadcast: partitioning.Filter,
+        variable_carry: partitioning.Filter,
+        split_rngs: contextlib.RngFilter,
+        in_axes: tp.Any,
+        out_axes: tp.Any,
+        length: tp.Optional[int],
+        reverse: bool,
+        unroll: int,
+        data_transform: tp.Optional[tp.Callable[..., tp.Any]],
+        metadata_params: tp.Mapping[tp.Any, tp.Any],
     ):
-        self.module_type = module_type
+        self.module_constructor = module_constructor
         self.variable_axes = variable_axes
         self.variable_broadcast = variable_broadcast
         self.variable_carry = variable_carry
         self.split_rngs = split_rngs
         self.in_axes = in_axes
         self.out_axes = out_axes
         self.length = length
         self.reverse = reverse
         self.unroll = unroll
         self.data_transform = data_transform
         self.metadata_params = metadata_params
-        self.module = self.create_module(*module_init_args, **module_init_kwargs)
+        self.scan_module = self.create_module(*module_init_args, **module_init_kwargs)
 
     def create_module(
         self: "Scan[M]", *args, ctx: tp.Optional[contextlib.Context] = None, **kwargs
     ) -> M:
         if self.variable_axes and self.length is None:
             raise ValueError("Cannot use variable_axes without specifying a length")
 
@@ -320,15 +321,15 @@
 
             if ctxdef is not None:
                 assert key_names is not None
                 keys = dict(zip(key_names, key_values))
                 ctx = ctxdef.merge(keys)
                 kwargs["ctx"] = ctx
 
-            module = self.module_type(*args, **kwargs)
+            module = self.module_constructor(*args, **kwargs)
 
             # lift module
             filters = (
                 *self.variable_axes.keys(),
                 self.variable_broadcast,
                 self.variable_carry,
             )
@@ -341,18 +342,25 @@
             _init_state = jax.vmap(
                 _init_state,
                 in_axes=key_axes,
                 out_axes=init_out_axes,
                 axis_size=self.length,
             )
 
-        module_states = _init_state(*key_values)
+        *axes_states, broadcast_state, carry_state = _init_state(*key_values)
         moduledef = tp.cast(ModuleDef[M], moduledef)
 
-        module = moduledef.merge(*module_states)
+        # add additional axis name to Variable.sharding
+        if spmd.PARTITION_NAME in self.metadata_params:
+            axes_states = [
+                spmd.add_axis(state, index, self.metadata_params)
+                for state, index in zip(axes_states, self.variable_axes.values())
+            ]
+
+        module = moduledef.merge(*axes_states, broadcast_state, carry_state)
 
         return module
 
     def __call__(
         self,
         carry_arg: C,
         axes_arg,
@@ -362,15 +370,15 @@
     ) -> tp.Tuple[C, tp.Any]:
         return self.call(  # type: ignore
             carry_arg, axes_arg, *broadcast_args, ctx=ctx, **broadcast_kwargs
         )
 
     @property
     def call(self) -> M:
-        accessesor = utils.DelayedAccessor()
+        accessesor = DelayedAccessor()
 
         def _context(
             accessesor,
             carry_arg: C,
             axes_arg,
             *broadcast_args,
             ctx: tp.Optional[contextlib.Context] = None,
@@ -382,23 +390,23 @@
                 self.variable_broadcast,
                 self.variable_carry,
             )
             (
                 *axes_states,
                 broadcast_state,
                 carry_state,
-            ), moduledef = self.module.partition(*filters)
+            ), moduledef = self.scan_module.partition(*filters)
 
             # transpose axes state
             axes_states = tuple(
                 jax.tree_map(lambda x: jnp.moveaxis(x, axis, 0), axes_state)
                 for axes_state, axis in zip(axes_states, self.variable_axes.values())
             )
             # transpose axes arg
-            axes_arg = utils.tree_map_upto_left(
+            axes_arg = tree_map_upto_left(
                 lambda axis, node: jax.tree_map(
                     lambda x: jnp.moveaxis(x, axis, 0), node
                 ),
                 self.in_axes,
                 axes_arg,
             )
 
@@ -465,27 +473,45 @@
 
                 # merge rng state
                 if ctxdef is not None:
                     assert axes_keys is not None and broadcast_keys is not None
                     ctx = ctxdef.merge({**axes_keys, **broadcast_keys})
                     broadcast_kwargs["ctx"] = ctx
 
+                # remove metadata axis name from Variable.sharding
+                if spmd.PARTITION_NAME in self.metadata_params:
+                    axes_states = [
+                        spmd.remove_axis(state, index, self.metadata_params)
+                        for state, index in zip(
+                            axes_states, self.variable_axes.values()
+                        )
+                    ]
+
                 # merge module state
                 module = moduledef.merge(*axes_states, broadcast_state, carry_state)
 
                 fn = accessesor(module)
                 (carry_out, axes_out) = fn(
                     carry_arg, axes_arg, *broadcast_args, **broadcast_kwargs
                 )
 
                 # split module state
                 (*axes_states, _broadcast_state, carry_state), _ = module.partition(
                     *filters
                 )
 
+                # add metadata axis name to Variable.sharding
+                if spmd.PARTITION_NAME in self.metadata_params:
+                    axes_states = [
+                        spmd.add_axis(state, index, self.metadata_params)
+                        for state, index in zip(
+                            axes_states, self.variable_axes.values()
+                        )
+                    ]
+
                 carry = (carry_state, carry_out)
                 out = (axes_states, axes_out)
 
                 return carry, out
 
             carry, scan_out = jax.lax.scan(
                 scan_fn,
@@ -500,55 +526,169 @@
 
             # transpose axes state
             axes_states = tuple(
                 jax.tree_map(lambda x: jnp.moveaxis(x, 0, axis), axes_state)
                 for axes_state, axis in zip(axes_states, self.variable_axes.values())
             )
             # transpose axes arg
-            out = utils.tree_map_upto_left(
+            out = tree_map_upto_left(
                 lambda axis, node: jax.tree_map(
                     lambda x: jnp.moveaxis(x, 0, axis), node
                 ),
                 self.out_axes,
                 out,
             )
 
-            self.module.update_state((*axes_states, carry_state))
+            self.scan_module.update_state((*axes_states, carry_state))
 
             return carry_out, out
 
-        return utils.CallableProxy(_context, accessesor)  # type: ignore
+        return CallableProxy(_context, accessesor)  # type: ignore
 
 
 def scan(
-    module_type: tp.Type[M],
+    module_constructor: tp.Callable[..., M],
     variable_axes: tp.Mapping[partitioning.Filter, int] = MappingProxyType({}),
     variable_broadcast: partitioning.Filter = None,
     variable_carry: partitioning.Filter = ...,
     split_rngs: contextlib.RngFilter = None,
-    in_axes=0,
-    out_axes=0,
+    in_axes: tp.Any = 0,
+    out_axes: tp.Any = 0,
     length: tp.Optional[int] = None,
     reverse: bool = False,
     unroll: int = 1,
     data_transform: tp.Optional[tp.Callable[..., tp.Any]] = None,
     metadata_params: tp.Mapping[tp.Any, tp.Any] = {},
 ) -> tp.Callable[..., Scan[M]]:
     def _create_scan(*args, **kwargs) -> Scan[M]:
         return Scan(
-            module_type,
-            args,
-            kwargs,
+            module_constructor=module_constructor,
+            module_init_args=args,
+            module_init_kwargs=kwargs,
             variable_axes=variable_axes,
             variable_broadcast=variable_broadcast,
             variable_carry=variable_carry,
             split_rngs=split_rngs,
             in_axes=in_axes,
             out_axes=out_axes,
             length=length,
             reverse=reverse,
             unroll=unroll,
             data_transform=data_transform,
             metadata_params=metadata_params,
         )
 
     return _create_scan
+
+
+class Remat(Module, tp.Generic[M]):
+    def __init__(
+        self,
+        *,
+        module_constructor: tp.Callable[..., M],
+        module_init_args: tp.Tuple[tp.Any, ...],
+        module_init_kwargs: tp.Dict[str, tp.Any],
+        # variables: lift.CollectionFilter,
+        # rngs: lift.PRNGSequenceFilter,
+        prevent_cse: bool,
+        static_argnums: tp.Union[int, tuple[int, ...]],
+        policy: tp.Optional[tp.Callable[..., bool]],
+    ):
+        if isinstance(static_argnums, int):
+            static_argnums = (static_argnums,)
+
+        # add 2 as an offset to account for state and keys
+        static_argnums = tuple(x + 2 if x >= 0 else x for x in static_argnums)
+
+        self.module_constructor = module_constructor
+        self.prevent_cse = prevent_cse
+        self.static_argnums = static_argnums
+        self.policy = policy
+        self.remat_module = self.module_constructor(
+            *module_init_args, **module_init_kwargs
+        )
+
+    def __call__(
+        self,
+        *args,
+        ctx: tp.Optional[contextlib.Context] = None,
+    ):
+        return self.call(*args, ctx=ctx)  # type: ignore
+
+    @property
+    def call(self) -> M:
+        accessesor = DelayedAccessor()
+
+        def _call(
+            accessesor, *args, ctx: tp.Optional[contextlib.Context] = None
+        ) -> tp.Tuple[tp.Any]:
+            state, moduledef = self.remat_module.partition()
+
+            if ctx is not None:
+                keys, ctxdef = ctx.partition()
+            else:
+                keys = None
+                ctxdef = None
+
+            def _remat_fn(
+                state: State,
+                keys: tp.Optional[tp.Dict[str, jax.Array]],
+                *args,
+            ) -> tp.Tuple[State, tp.Any]:
+                kwargs = {}
+                if keys is not None:
+                    assert ctxdef is not None
+                    kwargs["ctx"] = ctxdef.merge(keys)
+
+                module = moduledef.merge(state)
+                fn = accessesor(module)
+                out = fn(*args, **kwargs)
+
+                state, _ = module.partition()
+
+                return state, out
+
+            state, out = jax.checkpoint(
+                _remat_fn,
+                prevent_cse=self.prevent_cse,
+                static_argnums=self.static_argnums,
+                policy=self.policy,
+            )(state, keys, *args)
+
+            self.remat_module.update_state(state)
+
+            return out
+
+        return CallableProxy(_call, accessesor)  # type: ignore
+
+
+def remat(
+    module_constructor: tp.Callable[..., M],
+    # variables: lift.CollectionFilter = True,
+    # rngs: lift.PRNGSequenceFilter = True,
+    prevent_cse: bool = True,
+    static_argnums: tp.Union[int, tuple[int, ...]] = (),
+    policy: tp.Optional[tp.Callable[..., bool]] = None,
+) -> tp.Callable[..., Remat[M]]:
+    def create_remat(*args, **kwargs) -> Remat[M]:
+        return Remat(
+            module_constructor=module_constructor,
+            module_init_args=args,
+            module_init_kwargs=kwargs,
+            prevent_cse=prevent_cse,
+            static_argnums=static_argnums,
+            policy=policy,
+        )
+
+    return create_remat
+
+
+def tree_map_upto_left(
+    f: tp.Callable[[tp.Any, tp.Any], tp.Any], left: tp.Any, right: tp.Any
+) -> tp.Any:
+    leaves_left, treedef = jtu.tree_flatten(left)
+    leaves_right = treedef.flatten_up_to(right)
+
+    return treedef.unflatten(
+        f(left_leaf, right_leaf)
+        for left_leaf, right_leaf in zip(leaves_left, leaves_right)
+    )
```

### Comparing `nnx-0.0.6/pyproject.toml` & `nnx-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 jax = "*"
 jaxlib = "*"
 optax = "*"
 typing-extensions = "*"
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `nnx-0.0.6/PKG-INFO` & `nnx-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: nnx
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Cristian Garcia
 Author-email: cgarcia.e88@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: optax
 Requires-Dist: typing-extensions
@@ -21,18 +20,17 @@
 # NNX
 
 _**N**eural **N**etworks for JA**X**_
 
 NNX is a Neural Networks library for JAX that provides a simple yet powerful module system that adheres to standard Python semantics. Its aim is to combine the robustness of [Flax](https://flax.readthedocs.io/en/latest/) with a simplified, Pythonic API akin to that of [PyTorch](https://pytorch.org/).
 
 * **Pythonic**: Modules are just regular python classes, they contain their own state, are fully mutable, and allow sharing references between Modules.
-* **Fully Compatible**: Easy convert back and forth between Modules and pure pytrees compatible with any JAX transformation and other JAX tooling.
+* **Compatible**: Easily convert back and forth between Modules and pytrees using the Functional API to integrate with any JAX API.
 * **Safe**: NNX incorporates mechanisms to try to prevent tracer leakage, avoid stale RNGs, and ensure proper state propagation in order to help produce correct JAX programs.
 * **Semantic**: Partition a Module's state into different semantic collections, allowing for fine-grained control when applying JAX transformations.
-* **Lifted Transforms**: NNX offers a set of Module-aware transforms that automatically manage the Module's state and provide APIs to instruct the underlying JAX transform how to handle each state collection.
 
 #### Table of Contents
 * [Installation](#installation)
 * [Getting Started](#getting-started)
 * [FAQs](#faqs)
 * [Examples](#examples)
 * [User Guide](#user-guide)
@@ -55,20 +53,22 @@
 The following example guides you through creating a basic `Linear` model with NNX and executing a forward pass. It also demonstrate how handle mutable state by showing how to keep track of the number of times the model has been called.
 
 ```python
 import nnx
 import jax
 import jax.numpy as jnp
 
+class Count(nnx.Variable): pass
+
 class Linear(nnx.Module):
     def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
         key = ctx.make_rng("params")
-        self.w = nnx.param(jax.random.uniform(key, (din, dout)))
-        self.b = nnx.param(jnp.zeros((dout,)))
-        self.count = nnx.var("counts", 0)  # track the number of calls
+        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))
+        self.b = nnx.Param(jnp.zeros((dout,)))
+        self.count = Count(0)  # track the number of calls
 
     def __call__(self, x):
         self.count += 1
         return x @ self.w + self.b
 
 model = Linear(din=12, dout=2, ctx=nnx.context(0))
 
@@ -82,22 +82,22 @@
 inside `__init__` to generate a random key to initialize the parameters.
 
 ### Training with the Functional API
 
 The [Functional API](#functional-api) converts an NNX Module python semantics into pure pytree object with functional semantics. It is the recommended way to use NNX as it provides tight control over the state, allows you to use regular JAX transformations, and it minimizes overhead. In this example the model will be trained using Stochastic Gradient Descent (SGD).
 
 ```python
-(params, counts), moduledef = model.partition("params", "counts")
+(params, counts), moduledef = model.partition(nnx.Param, Count)
 
 @jax.jit
 def train_step(params, counts, x, y):
     def loss_fn(params):
         y_pred, (updates, _) = moduledef.apply(params, counts)(x)
         loss = jax.numpy.mean((y_pred - y) ** 2)
-        return loss, updates.filter("counts")
+        return loss, updates.filter(Count)
 
     # compute gradient
     grads, counts = jax.grad(loss_fn, has_aux=True)(params)
     # SGD update
     params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grads)
 
     return params, counts
@@ -116,36 +116,36 @@
 @nnx.jit
 def train_step(model, x, y):
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
     
     # compute gradient
-    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
+    grads: nnx.State = nnx.grad(loss_fn, wrt=nnx.Param)(model)
     # SGD update
     model.update_state(
-        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
+        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter(nnx.Param), grads)
     )
 
 # execute the training step
 train_step(model, x, y)
 assert model.count == 2
 ```
 
 **Note**: Using `nnx.jit` introduces some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes, but for production code use `jax.jit` directly.
 
 ## Examples
 
-* [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/01_jit_transform.py): Shows how to train a simple model using lifted transforms.
-* [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/02_functional_api.py): Shows how to train a simple model using the functional API.
+* [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/01_functional_api.py): Shows how to train a simple model using the functional API.
+* [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/02_lifted_transforms.py): Shows how to train a simple model using lifted transforms.
 * [Using TrainState](https://github.com/cgarciae/nnx/blob/main/examples/03_train_state.py): Shows how to train a simple model using the functional API with the help of `TrainState`.
 * [Using PureModule](https://github.com/cgarciae/nnx/blob/main/examples/04_pure.py) (experimental): Shows how to train a simple model using the functional API and leveraging `PureModule` to simplify the code.
 * [Training a VAE](https://github.com/cgarciae/nnx/blob/main/examples/05_vae.py): Shows how to train a VAE on the binarized MNIST dataset, uses the functional API, `TrainState`, and shows how to use capture intermediate values to retrieve `kl_loss`.
 * [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py): An contrived example that implements scan over layers with dropout and a share BatcNorm layer to showcase how lifted transforms can be implemented. It uses the functional API along with `jax.vmap` and `jax.lax.scan`.
-* [Creating a Transformer](https://github.com/cgarciae/nnx/blob/main/examples/07_tranformer.py): Shows how to create a Transformer with an auto-regressive decoder that uses scan over layers and a kv-cache for fast inference. Credits to @levskaya.
+* [Creating a Transformer](https://github.com/cgarciae/nnx/blob/main/examples/07_transformer.py): Shows how to create a Transformer with an auto-regressive decoder that uses scan over layers and a kv-cache for fast inference. Credits to @levskaya.
 
 ## FAQs
 
 ### Status
 NNX is still in early development so expect bugs and breaking changes. That said, current API is the result of months of experimentation and we don't expect any major changes in the near future.
 
 ### How is it different from Flax?
@@ -164,24 +164,24 @@
 
 One major difference between the two frameworks is that, by design, NNX Modules are not Pytrees. This adds a safety layer as it prevents state updates from being lost by accident due to referential transparency. It also removes the need of threading a separate [State container](https://docs.kidger.site/equinox/examples/stateful/) throughout the code in order to propagate state. In NNX state updates are either always preserved or explicitly discarded by the user.
 
 ## User Guide
 
 ### Modules
 
-NNX Modules are normal python classes, they obey regular python semantics such as mutability and reference sharing, including reference cycles. They can contain 2 types of attributes: node attributes and static attributes. Node attributes include NNX `Variable`s (e.g. `nnx.param`), Numpy arrays, JAX arrays, submodules Modules, and other NNX types. All other types are treated as static attributes.
+NNX Modules are normal python classes, they obey regular python semantics such as mutability and reference sharing, including reference cycles. They can contain 2 types of attributes: node attributes and static attributes. Node attributes include NNX `Variable`s (e.g. `nnx.Param`), Numpy arrays, JAX arrays, submodules Modules, and other NNX types. All other types are treated as static attributes.
 
 ```python
 class Foo(nnx.Module):
     def __init__(self, ctx: nnx.Context):
         # node attributes
-        self.variable = nnx.param(jnp.array(1))
+        self.variable = nnx.Param(jnp.array(1))
         self.np_buffer = np.array(2)
         self.jax_buffer = jnp.array(3)
-        self.node = nnx.node([4, 5])
+        self.node = nnx.Node([4, 5])
         self.submodule = nnx.Linear(2, 4, ctx=ctx)
         # static attributes
         self.int = 1
         self.float = 2.0
         self.str = "hello"
         self.list = [1, 2, 3]
 
@@ -197,17 +197,17 @@
 state, moduledef = model.partition()
 ```
 ```
 State({
   ('jax_buffer',): Array(3),
   ('node',): Node(value=[4, 5]),
   ('np_buffer',): array(2),
-  ('submodule', 'bias'): Variable(collection='params', value=Array(...)),
-  ('submodule', 'kernel'): Variable(collection='params', value=Array(...)),
-  ('variable',): Variable(collection='params', value=Array(1))
+  ('submodule', 'bias'): Param(value=Array(...)),
+  ('submodule', 'kernel'): Param(value=Array(...)),
+  ('variable',): Param(value=Array(1))
 })
 ```
 
 `State` and `ModuleDef` are pytrees so they can be passed to JAX transformations. More over, `ModuleDef` provides 2 very important methods: `merge` and `apply`. The `merge` method can be used to create a new `Module` from a `State` object:
 
 ```python
 model = moduledef.merge(state)
@@ -222,31 +222,31 @@
 # run submodule
 y, (state, moduledef) = moduledef.apply(state).submodule(x)
 ```
 
 `apply` can call any nested method or submodule as long as it can be accessed via the `.` or `[]` operators.
 
 ### Partitioning State
-`nnx.var` lets you create `Variable` attributes with `collection` metadata, this metadata can be used to partition the state into multiple substates. `nnx.param` is a special case of `nnx.var` where `collection="params"`. 
+In NNX you can filter based on any node type, most commonly you will want to filter based on `nnx.Variable` subclasses such as `nnx.Param` or `nnx.BatchStat`.
 
-Here are various examples of how you can use the `partition` method along with collection names to partition a module into multiple substates:
+Here are various examples of how you can use the `partition` method to split a module into multiple substates:
 
 ```python
 # partition the module into the state with all the nodes and the moduledef
 state, moduledef = model.partition()
 # verify that the state contains only params, else raise an error
-params, moduledef = model.partition("params")
+params, moduledef = model.partition(nnx.Param)
 # split the state into params and batch_stats, verify no nodes are left
-(params, batch_stats), moduledef = model.partition("params", "batch_stats")
+(params, batch_stats), moduledef = model.partition(nnx.Param, nnx.BatchStat)
 # if there are any nodes left, use the `...` filter to capture them
-(params, batch_stats, rest), moduledef = model.partition("params", "batch_stats", ...)
+(params, batch_stats, rest), moduledef = model.partition(nnx.Param, nnx.BatchStat, ...)
 # using `...` as the only filter is equivalent to not passing any filters
 model.partition(...) = model.partition()
 ```
-`partition` will make sure all nodes are match by atleast one filter, else it will raise an error. If you have non-`Variable` nodes like `nnx.node`, `jax.Array`, or `numpy.ndarray` attributes, you can use the `...` filter which will match any node. For a more general filter you can pass a predicate function of the form:
+`partition` will make sure all nodes are match by atleast one filter, else it will raise an error. If you have non-`Variable` nodes like `nnx.Node`, `jax.Array`, or `numpy.ndarray` attributes, you can use the `...` filter which will match any node. For a more general filter you can pass a predicate function of the form:
 
 ```python
 (path: Tuple[str, ...], value: Any) -> bool
 ```
 
 To reconstruct the module from a set of substates, you can use `merge` as usual but passing the substates as additional arguments:
 
@@ -259,130 +259,173 @@
 ```python
 y, (state, moduledef) = moduledef.apply(params, batch_stats, rest)(x)
 ```
 
  Note that `apply` will return a single `state` object, if you need to re-partition the state you can use `State`'s own `partition` method:
 
 ```python
-params, batch_stats, rest = state.partition("params", "batch_stats", ...)
+params, batch_stats, rest = state.partition(nnx.Param, nnx.BatchStat, ...)
 ```
 
 Alternatively, if you are just interested in a subset of partitions, you can use the `State.filter` method which will not raise an error if some nodes are not matched by any filter:
 
 ```python
 # only get params
-params = state.filter("params")
+params = state.filter(nnx.Param)
 # get params and batch_stats
-params, batch_stats = state.filter("params", "batch_stats")
+params, batch_stats = state.filter(nnx.Param, nnx.BatchStat)
 ```
 
 ### Filters
 
 Filters let you select subsets of nodes based on some criteria. These are use throughout the API in method like `partition`, `filter`, and `pop_state`. There are 4 types of filters:
 
-* `str`: matches all `Variable` nodes (e.g. `nnx.param` or `nnx.var`) with the given `collection` name.
 * `type`: matches all node instances of the given type.
 * `...`: matches all nodes.
 * `(path, any) -> bool`: a predicate function that takes a node path and value and returns a boolean.
 * `Tuple[Filter, ...]`: a tuple of filters, matches all nodes that match any of the filters.
 
 NNX also provides the following custom filters:
 
 * `nnx.Not(filter)`: matches all nodes that do not match the given filter
 * `nnx.buffers`: matches all `numpy.ndarray` and `jax.Array` nodes
 
 Here is an example of how to use `Not` and `buffers`:
 ```python
-rest = module.filter(nnx.Not("params"))
+rest = module.filter(nnx.Not(nnx.Param))
 buffers = module.filter(nnx.buffers)
 ```
 
 
 ### Capturing Intermediate Values
 In NNX you can easily propagate intemediate values by simply assigning them to an attribute at runtime. For convenience, you should assign them to a `Variable` attribute with a `collection` name by using `nnx.var` so you can easily retrieve them later.
 
 Here is an example of how to create a `Linear` module that captures its output into a `Variable` attribute with the `intermediates` collection name:
 
 ```python
 class Linear(nnx.Module):
     def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
         key = ctx.make_rng("params")
-        self.w = nnx.param(jax.random.uniform(key, (din, dout)))
-        self.b = nnx.param(jnp.zeros((dout,)))
+        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))
+        self.b = nnx.Param(jnp.zeros((dout,)))
 
     def __call__(self, x):
         y = x @ self.w + self.b
-        self.y = nnx.var("intermediates", y)
+        self.y = nnx.Intermediate(y)
         return y
 
 model = Linear(12, 2, ctx=nnx.context(0))
 ```
-Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `intermediates`:
+Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `Intermediate`:
 
 ```python
 y = model(jnp.ones((8, 12)))
-intermediates = model.pop_state("intermediates")
+intermediates = model.pop_state(nnx.Intermediate)
 ```
 `pop_state` will return a `State` object with the nodes that match the given filter and remove them from the module's attributes.
 
 ```
 State({
-  ('y',): Variable(
-    collection='intermediates',
+  ('y',): Intermediate(
     value=Array(...)
   )
 })
 ```
 
-If you use the functional API to call the module instead, the `intermediates` nodes will be present in the output `state`. To retrieve the `intermediates` nodes and optionally separate them from the output `state` you can use `State.partition`:
+If you use the functional API to call the module instead, the `Intermediate` nodes will be present in the output `state`. To retrieve the `intermediates` nodes and optionally separate them from the output `state` you can use `State.partition`:
 
 ```python
 state, moduledef = model.partition()
 y, (state, moduledef) = moduledef.apply(state)(jnp.ones((8, 12)))
 # "pop" the intermediates from the state
 intermediates, state = state.partition("intermediates", ...)
 ```
 
 Alternatively, you can use `State.filter` to retrieve the `intermediates` nodes without removing them from the `state`.
 
 
 
 ### Lifted Transforms
 
-Stateful transforms take a Module as their first argument, track changes in the state that occur within the transformation, and automatically propagate those changes to the input Module outside the transformation. In general, they behave as stateful functions with respect to the first argument.
+NNX lifted transforms analogous versions of JAX transforms but they know how to work with Modules. They usually perform the following tasks:
+
+* Handle the Module's substates and Context's RNG streams according to the transform's semantics.
+* Properly propagating state in and out of the transform, including updating the input Module's state with updates that happen inside the transform.
+
+Here's a diagram illustrating how lifted transformations work:
+
+![lifted-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
 
-Here's a diagram illustrating how stateful transformations work:
+Currently NNX provides the `jit`, `grad`, and `scan` lifted transforms.
 
-![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
+#### Manual Lifting
 
-Currently, `nnx.jit` and `nnx.grad` are the only stateful transformations.
+In case you want to use JAX transforms directly you can always use the functional API
+to manually lift your Modules. 
 
-The following example demonstrates how a `train_step` function can be implemented using `nnx.jit` and `nnx.grad`:
+Here we will create an example of how to implement an MLP that uses "scan over layers" to efficiently process a sequence of inputs assuming that each layer has the same parameters and input/output dimensions. The first thing we need to do is create a `Block` module that represents a single layer, this block with just contain a `Linear` layer, a `Dropout` layer, and a `GELU` activation function:
 
 ```python
-@nnx.jit
-def train_step(model, x, y):
+class Block(nnx.Module):
+    def __init__(self, dim: int, *, ctx: nnx.Context):
+        self.linear = nnx.Linear(dim, dim, ctx=ctx)
+        self.dropout = nnx.Dropout(0.5)
 
-    def loss_fn(model):
-        y_pred = model(x)
-        return jax.numpy.mean((y_pred - y) ** 2)
-    
-    # compute gradient
-    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
-    # SGD update
-    model.update_state(
-        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
-    )
+    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:
+        x = self.linear(x)
+        x = self.dropout(x, deterministic=not train, ctx=ctx)
+        x = jax.nn.gelu(x)
+        return x
+```
+
+Now we will define `ScanMLP`. During `__init__`, instead of creating a list of `Block`s, we will use `jax.vmap` to create a single `Block` whose parameters have an addtional `layer` axis. This will allow us to pass the parameters as inputs to scan so it will apply a layer at each step.
+
+```python
+class ScanMLP(nnx.Module):
+    def __init__(self, dim: int, *, n_layers: int, ctx: nnx.Context):
+        params_key = jax.random.split(ctx.make_rng("params"), n_layers)
+        self.n_layers = n_layers
+        self.layers = jax.vmap(
+            lambda key: Block(dim, ctx=nnx.context(params=key)).partition()
+        )(params_key).merge()
 
-# stateful update
-train_step(model, x, y)
 ```
+Note that we split the `params` key into `n_layers` keys so each layer has different parameters.
+
+Now we will define `__call__`. Here we need to split the `dropout` key into `n_layers` keys so each layer has a different dropout mask, and `partition` the layers to get their `params`. Both `params` and `dropout_key` will be passed as inputs, `x` will be the carry value. Inside the `scan_fn` we will merge the `params` back into a `Block` module and
+apply it to the input `x`, passing the sliced `dropout_key` as part of the `Context`.
+
+
+```python
+    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:
+        dropout_key = jax.random.split(ctx.make_rng("dropout"), self.n_layers)
+        params, moduledef = self.layers.partition(nnx.Param)
 
-The most interesting aspect of this design is that the code appears very imperative, as the state is automatically propagated in and out of the transformations.
+        def scan_fn(x: inputs):
+            params, dropout_key = inputs
+            module = moduledef.merge(params)
+            x = module(x, train=train, ctx=nnx.context(dropout=dropout_key))
+            return x, module.filter(nnx.Param)
+
+        x, params = jax.lax.scan(scan_fn, x, (params, dropout_key))
+        self.layers.update_state(params)
+        return x
+```
+Finally we apply `jax.lax.scan`, update the `layers` state with the new `params`, and return the final `x` value.
+
+Here is a simple way to test our `ScanMLP`:
+
+```python
+model = ScanMLP(10, n_layers=5, ctx=nnx.context(0))
+
+x = jnp.ones((3, 10))
+y = model(x, train=True, ctx=nnx.context(dropout=1))
+```
 
+For a more robust implementation with comments take a look at the [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py) example.
 
 ### Case Studies
 #### Shared State
 
 In NNX, you can create modules that share state between them. This is useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
 
 Here's an example of creating a module with shared state:
```

