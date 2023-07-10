# Comparing `tmp/fsrs4anki_optimizer-3.26.1.tar.gz` & `tmp/fsrs4anki_optimizer-3.26.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.26.1.tar", last modified: Thu Jul  6 02:15:28 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.26.2.tar", last modified: Mon Jul 10 11:35:13 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.26.1.tar` & `fsrs4anki_optimizer-3.26.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45685 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/setup.py
```

### Comparing `fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                         torch.pow(state[:,0], self.w[7]) *
                         (torch.exp((1 - r) * self.w[8]) - 1))
         return new_s
 
     def stability_after_failure(self, state: Tensor, new_d: Tensor, r: Tensor) -> Tensor:
         new_s = self.w[9] * torch.pow(new_d, self.w[10]) * torch.pow(
             state[:,0], self.w[11]) * torch.exp((1 - r) * self.w[12])
-        return new_s
+        return new_s.clamp(max=state[:,0])
 
     def step(self, X: Tensor, state: Tensor) -> Tensor:
         '''
         :param X: shape[batch_size, 2], X[:,0] is elapsed time, X[:,1] is rating
         :param state: shape[batch_size, 2], state[:,0] is stability, state[:,1] is difficulty
         :return state:
         '''
@@ -628,15 +628,15 @@
         def init_stability(d):
             return max(((d - self.w[2]) / self.w[3] + 2) * self.w[1] + self.w[0], np.power(base, -index_offset))
 
         def cal_next_recall_stability(s, r, d, response):
             if response == 1:
                 return s * (1 + np.exp(self.w[6]) * (11 - d) * np.power(s, self.w[7]) * (np.exp((1 - r) * self.w[8]) - 1))
             else:
-                return self.w[9] * np.power(d, self.w[10]) * np.power(s, self.w[11]) * np.exp((1 - r) * self.w[12])
+                return np.minimum(self.w[9] * np.power(d, self.w[10]) * np.power(s, self.w[11]) * np.exp((1 - r) * self.w[12]), s)
 
         terminal_stability = minimum_stability
         for _ in range(128):
             terminal_stability = cal_next_recall_stability(terminal_stability, 0.96, d_range, 1)
         index_len = stability2index(terminal_stability)
         stability_list = np.array([np.power(base, i - index_offset) for i in range(index_len)])
         print(f"terminal stability: {stability_list.max(): .2f}")
```

