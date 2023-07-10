# Comparing `tmp/fa-models-1.0.74.tar.gz` & `tmp/fa-models-1.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.74.tar", last modified: Thu Jul  6 07:39:48 2023, max compression
+gzip compressed data, was "fa-models-1.0.75.tar", last modified: Mon Jul 10 06:14:47 2023, max compression
```

## Comparing `fa-models-1.0.74.tar` & `fa-models-1.0.75.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.154089 fa-models-1.0.74/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 07:39:48.154089 fa-models-1.0.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-06 07:39:17.000000 fa-models-1.0.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.146089 fa-models-1.0.74/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.146089 fa-models-1.0.74/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.150089 fa-models-1.0.74/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.154089 fa-models-1.0.74/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 07:39:40.000000 fa-models-1.0.74/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:39:48.154089 fa-models-1.0.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 07:39:17.000000 fa-models-1.0.74/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.154089 fa-models-1.0.74/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-06 07:39:17.000000 fa-models-1.0.74/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 07:39:17.000000 fa-models-1.0.74/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-10 06:14:47.211431 fa-models-1.0.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-10 06:14:11.000000 fa-models-1.0.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.207431 fa-models-1.0.75/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.207431 fa-models-1.0.75/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-10 06:14:37.000000 fa-models-1.0.75/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:14:47.211431 fa-models-1.0.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-10 06:14:11.000000 fa-models-1.0.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-10 06:14:11.000000 fa-models-1.0.75/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 06:14:11.000000 fa-models-1.0.75/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.74/PKG-INFO` & `fa-models-1.0.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.74
+Version: 1.0.75
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.74/README.md` & `fa-models-1.0.75/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.75/fa_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.74
+Version: 1.0.75
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.74/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.75/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/algorithm.py` & `fa-models-1.0.75/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/investor.py` & `fa-models-1.0.75/famodels/models/investor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 key = os.environ.get("ENCRYPTION_KEY").encode()
 ENCRYPTION_KEY = urlsafe_b64encode(sha256(key).digest())
 
 class Subscription(EmbeddedJsonModel):
     id: str = Field(index=False)
     algo_id:str = Field(index=True)
     # redis model can only store these fields of the embedded json model as string
-    start_timestamp:str = Field(index=True, default=int(time.time() * 1000))
+    start_timestamp:Optional[str]
     stop_timestamp: Optional[str]
 
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="subscription"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.74/famodels/models/investor_statement.py` & `fa-models-1.0.75/famodels/models/investor_statement.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,13 +11,14 @@
     investor_id: str = Field(index=True)
     timestamp: int = Field(index=True, default=int(time.time() * 1000))
     available_cash: float = Field(index=True, default=0)
     """All the available cash (in USDT)"""
     invested_assets_valued_in_quote: float = Field(index=True, default=0)
     """All the available assets - except the cash/quote currency - valued in quote currency (USDT)."""
     total_assets_value = float = (Field(index=True, default=0))
+    total_assets_value = float = (Field(index=True, default=0))
     """Total values of invested assets + available cash = total_assets_value"""
 
     class Meta:
         # global_key_prefix="order-and-trade-processing"
         model_key_prefix="investor-statement"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.74/famodels/models/market/public_trade.py` & `fa-models-1.0.75/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/order.py` & `fa-models-1.0.75/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/person.py` & `fa-models-1.0.75/famodels/models/person.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 class Person(EmbeddedJsonModel):    
     given_name: str = Field(index=True)
     family_name: str = Field(index=True, full_text_search=True)
     email: EmailStr = Field(index=True)
-    sex: int = Field(index=True)    
-    """0=male, 1=female"""
+    gender: str = Field(index=True, max_length=1)    
+    """m or f"""
     nationality_iso3: str = Field(index=True, max_length=3, min_length=3)
     identification_type: Optional[str]
     identification_reference: Optional[str]
     country_of_residence_iso3: str = Field(index=True, max_length=3, min_length=3)
     phone: str = Field(index=True)
     
     class Meta:
```

### Comparing `fa-models-1.0.74/famodels/models/processed_signal.py` & `fa-models-1.0.75/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/signal_provider.py` & `fa-models-1.0.75/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/trade.py` & `fa-models-1.0.75/famodels/models/trade.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """The trade id is the reference that keeps the state updates correlated. It will generate a UUID by default.
         Use this for the first record you insert. Inserting updated records (new records should then have the trade_id
         provided to create the correlation.)"""
     investor_id: str = Field(index=True)
     fund_id: str = Field(index=True)
     pos_idx:int
     market:str = Field(index=True)    
-    status:StateOfTrade = Field(index=True, default=StateOfTrade.NEW)
+    state:StateOfTrade = Field(index=True, default=StateOfTrade.NEW)
     direction:Direction
     amount: float
     time_of_initiation:datetime = Field(index=True, default=int(time.time() * 1000))
     """When we decided to start this trade."""
     buy_order_id: Optional[str] = None
     sell_order_id:Optional[str] = None
     take_profit:Optional[float] = None
```

### Comparing `fa-models-1.0.74/famodels/models/trading_signal.py` & `fa-models-1.0.75/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/famodels/models/virtual_order.py` & `fa-models-1.0.75/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/pyproject.toml` & `fa-models-1.0.75/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.74"
+version = "1.0.75"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.74"
+current_version = "1.0.75"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.74/setup.py` & `fa-models-1.0.75/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.74/tests/test_investor.py` & `fa-models-1.0.75/tests/test_investor.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     if 'CI' not in os.environ:
         os.system('docker stop redis-unit-test')
         os.system('docker rm redis-unit-test')
 
 
 def test_investor_model():
-    # Now we can create an instance of `Investor` without connecting to a real Redis server
-    person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    """Simple test if we can create a Investor model."""
+    person = Person(given_name="john", family_name="Doe", email="john@doe.com", gender="f", nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
     investor = Investor(id='123', name="Jonathans Investements Ltd", email='test@example.com', accountable=person)    
 
 
 @pytest.mark.parametrize(
     "email, nationality_iso3, country_of_residence_iso3",
     [
         ("invalidemail", "GBR", "IRE"),  # invalid email
@@ -43,15 +43,15 @@
 )
 def test_negative_person(email, nationality_iso3, country_of_residence_iso3):
     with pytest.raises(ValidationError):
         Person(
             given_name="john",
             family_name="Doe",
             email=email,
-            sex=0,
+            gender="f",
             nationality_iso3=nationality_iso3,
             country_of_residence_iso3=country_of_residence_iso3,
             phone="+43 681 11 24",
         )
 
 @pytest.mark.parametrize(
     "email, nationality_iso3, country_of_residence_iso3",
@@ -65,15 +65,15 @@
 )
 def test_positive_person(email, nationality_iso3, country_of_residence_iso3):
     try:
         Person(
             given_name="john",
             family_name="Doe",
             email=email,
-            sex=0,
+            gender="f",
             nationality_iso3=nationality_iso3,
             country_of_residence_iso3=country_of_residence_iso3,
             phone="+43 681 11 24",
         )
     except ValidationError:
         pytest.fail("ValidationError raised unexpectedly!")
 
@@ -105,15 +105,15 @@
     [
         ("1", "Superion Corp.", "investor1@example.com", [{"id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"id": "s2", "algo_id": "a2"}, {"id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
         ("2", "Super Investment Ltd", "investor2@example.com", [{"id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"id": "s4", "algo_id": "a4"}, {"id": "s5", "algo_id": "a5"}, {"id": "s6", "algo_id": "a6"}], "compounding": 1}]),
         ("3", "XY Funds", "investor3@example.com", [{"id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"id": "s8", "algo_id": "a8"}, {"id": "s9", "algo_id": "a9"}, {"id": "s10", "algo_id": "a10"}]}])
     ]
 )
 def test_investor_funds(investor_id, name, email, funds):
-    person = Person(given_name="john", family_name="Doe", email=email, sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    person = Person(given_name="john", family_name="Doe", email=email, gender="f", nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
 
     funds_objects = []
     for fund in funds:
         subscriptions = [Subscription(**subscription) for subscription in fund.pop('subscriptions')]
         fund_obj = Fund(subscriptions=subscriptions, **fund)
         funds_objects.append(fund_obj)
 
@@ -128,15 +128,15 @@
         assert investor.funds[i].name == funds_objects[i].name
         assert investor.funds[i].compounding == funds_objects[i].compounding
         assert len(investor.funds[i].subscriptions) == len(funds_objects[i].subscriptions)
 
 
 def test_passphrase():
     # Create an Investor instance
-    person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    person = Person(given_name="john", family_name="Doe", email="john@doe.com", gender="f", nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
     investor = Investor(id='123', name="Johnny's Investments", email='test@example.com', accountable=person)
     investor.setPassphrase("testpass")
     # Check that passphrase can't be retrieved directly
     with pytest.raises(Exception) as e:
         print(f"INVOKING IS FORBIDDEN --> {investor.passphrase}")
     assert str(e.value) == "Cannot retrieve passphrase."
```

### Comparing `fa-models-1.0.74/tests/test_processed_trading_signal.py` & `fa-models-1.0.75/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

