# Comparing `tmp/appscommon-0.0.1.tar.gz` & `tmp/appscommon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appscommon-0.0.1.tar", last modified: Mon Mar 20 17:30:02 2023, max compression
+gzip compressed data, was "appscommon-0.0.2.tar", last modified: Mon Jul 10 06:49:45 2023, max compression
```

## Comparing `appscommon-0.0.1.tar` & `appscommon-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:02.039554 appscommon-0.0.1/
--rw-rw-rw-   0        0        0      586 2023-03-20 17:30:02.038551 appscommon-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-03-06 11:51:35.000000 appscommon-0.0.1/README.md
--rw-rw-rw-   0        0        0      627 2023-03-20 17:23:47.000000 appscommon-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-20 17:30:02.040551 appscommon-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.900524 appscommon-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.935522 appscommon-0.0.1/src/appscommon/
--rw-rw-rw-   0        0        0        0 2023-03-06 11:51:35.000000 appscommon-0.0.1/src/appscommon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.904524 appscommon-0.0.1/src/appscommon/db/
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.961520 appscommon-0.0.1/src/appscommon/db/adapters/
--rw-rw-rw-   0        0        0        0 2023-03-13 08:54:47.000000 appscommon-0.0.1/src/appscommon/db/adapters/__init__.py
--rw-rw-rw-   0        0        0     1462 2023-03-16 15:43:22.000000 appscommon-0.0.1/src/appscommon/db/adapters/unit_of_work.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.973523 appscommon-0.0.1/src/appscommon/db/interfaces/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:04:00.000000 appscommon-0.0.1/src/appscommon/db/interfaces/__init__.py
--rw-rw-rw-   0        0        0      439 2023-03-13 13:58:37.000000 appscommon-0.0.1/src/appscommon/db/interfaces/repository.py
--rw-rw-rw-   0        0        0      816 2023-03-13 14:23:46.000000 appscommon-0.0.1/src/appscommon/db/interfaces/unit_of_work.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.977739 appscommon-0.0.1/src/appscommon/domain/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:05:33.000000 appscommon-0.0.1/src/appscommon/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.983551 appscommon-0.0.1/src/appscommon/domain/models/
--rw-rw-rw-   0        0        0       93 2023-03-13 09:11:29.000000 appscommon-0.0.1/src/appscommon/domain/models/__init__.py
--rw-rw-rw-   0        0        0      457 2023-03-14 09:59:19.000000 appscommon-0.0.1/src/appscommon/domain/models/basemodel.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.992553 appscommon-0.0.1/src/appscommon/enums/
--rw-rw-rw-   0        0        0      116 2023-03-09 13:12:37.000000 appscommon-0.0.1/src/appscommon/enums/__init__.py
--rw-rw-rw-   0        0        0      110 2023-03-09 13:12:47.000000 appscommon-0.0.1/src/appscommon/enums/response_status_enum.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:02.008552 appscommon-0.0.1/src/appscommon/exception/
--rw-rw-rw-   0        0        0      153 2023-03-09 13:11:09.000000 appscommon-0.0.1/src/appscommon/exception/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-03-16 14:10:12.000000 appscommon-0.0.1/src/appscommon/exception/exceptions.py
--rw-rw-rw-   0        0        0     1356 2023-03-16 14:10:44.000000 appscommon-0.0.1/src/appscommon/exception/handler.py
--rw-rw-rw-   0        0        0      381 2023-03-06 11:51:35.000000 appscommon-0.0.1/src/appscommon/exception/message.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:02.013551 appscommon-0.0.1/src/appscommon/flaskutils/
--rw-rw-rw-   0        0        0        0 2023-03-09 12:27:40.000000 appscommon-0.0.1/src/appscommon/flaskutils/__init__.py
--rw-rw-rw-   0        0        0     2964 2023-03-17 06:13:19.000000 appscommon-0.0.1/src/appscommon/flaskutils/confighelper.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:02.022618 appscommon-0.0.1/src/appscommon/flaskutils/http/
--rw-rw-rw-   0        0        0        0 2023-03-10 06:15:21.000000 appscommon-0.0.1/src/appscommon/flaskutils/http/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:02.028626 appscommon-0.0.1/src/appscommon/flaskutils/http/middleware/
--rw-rw-rw-   0        0        0      112 2023-03-10 06:20:48.000000 appscommon-0.0.1/src/appscommon/flaskutils/http/middleware/__init__.py
--rw-rw-rw-   0        0        0     1697 2023-03-17 13:55:33.000000 appscommon-0.0.1/src/appscommon/flaskutils/http/middleware/filters.py
--rw-rw-rw-   0        0        0      199 2023-03-10 09:53:07.000000 appscommon-0.0.1/src/appscommon/flaskutils/http/utils.py
--rw-rw-rw-   0        0        0      959 2023-03-10 09:59:45.000000 appscommon-0.0.1/src/appscommon/logconfig.py
--rw-rw-rw-   0        0        0      283 2023-03-09 12:59:38.000000 appscommon-0.0.1/src/appscommon/readonly.py
--rw-rw-rw-   0        0        0      541 2023-03-06 11:51:35.000000 appscommon-0.0.1/src/appscommon/schemas.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:01.952729 appscommon-0.0.1/src/appscommon.egg-info/
--rw-rw-rw-   0        0        0      586 2023-03-20 17:30:01.000000 appscommon-0.0.1/src/appscommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-03-20 17:30:01.000000 appscommon-0.0.1/src/appscommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 17:30:01.000000 appscommon-0.0.1/src/appscommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-20 17:30:01.000000 appscommon-0.0.1/src/appscommon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-20 17:30:02.033552 appscommon-0.0.1/tests/
--rw-rw-rw-   0        0        0      470 2023-03-10 10:00:52.000000 appscommon-0.0.1/tests/test_logconfig.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.973385 appscommon-0.0.2/
+-rw-r--r--   0 danush     (501) staff       (20)      571 2023-07-10 06:49:45.973197 appscommon-0.0.2/PKG-INFO
+-rw-r--r--   0 danush     (501) staff       (20)       99 2023-04-03 18:14:50.000000 appscommon-0.0.2/README.md
+-rw-r--r--   0 danush     (501) staff       (20)      781 2023-07-10 06:47:00.000000 appscommon-0.0.2/pyproject.toml
+-rw-r--r--   0 danush     (501) staff       (20)       38 2023-07-10 06:49:45.973440 appscommon-0.0.2/setup.cfg
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.964832 appscommon-0.0.2/src/
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.967514 appscommon-0.0.2/src/appscommon/
+-rw-r--r--   0 danush     (501) staff       (20)        0 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/__init__.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.965041 appscommon-0.0.2/src/appscommon/db/
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.968696 appscommon-0.0.2/src/appscommon/db/adapters/
+-rw-r--r--   0 danush     (501) staff       (20)        0 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/db/adapters/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)     1408 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/db/adapters/unit_of_work.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.969526 appscommon-0.0.2/src/appscommon/db/interfaces/
+-rw-r--r--   0 danush     (501) staff       (20)        0 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/db/interfaces/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)      420 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/db/interfaces/repository.py
+-rw-r--r--   0 danush     (501) staff       (20)      780 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/db/interfaces/unit_of_work.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.969805 appscommon-0.0.2/src/appscommon/domain/
+-rw-r--r--   0 danush     (501) staff       (20)        0 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/domain/__init__.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.970214 appscommon-0.0.2/src/appscommon/domain/models/
+-rw-r--r--   0 danush     (501) staff       (20)       88 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/domain/models/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)      441 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/domain/models/basemodel.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.970617 appscommon-0.0.2/src/appscommon/enums/
+-rw-r--r--   0 danush     (501) staff       (20)      110 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/enums/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)      104 2023-05-29 10:41:29.000000 appscommon-0.0.2/src/appscommon/enums/response_status_enum.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.971494 appscommon-0.0.2/src/appscommon/exception/
+-rw-r--r--   0 danush     (501) staff       (20)      146 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/exception/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)     2432 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/exception/exceptions.py
+-rw-r--r--   0 danush     (501) staff       (20)     1305 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/exception/handler.py
+-rw-r--r--   0 danush     (501) staff       (20)      369 2023-05-29 10:41:29.000000 appscommon-0.0.2/src/appscommon/exception/message.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.971873 appscommon-0.0.2/src/appscommon/flaskutils/
+-rw-r--r--   0 danush     (501) staff       (20)        0 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/flaskutils/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)     2876 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/flaskutils/confighelper.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.972240 appscommon-0.0.2/src/appscommon/flaskutils/http/
+-rw-r--r--   0 danush     (501) staff       (20)        0 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/flaskutils/http/__init__.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.972620 appscommon-0.0.2/src/appscommon/flaskutils/http/middleware/
+-rw-r--r--   0 danush     (501) staff       (20)      106 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/flaskutils/http/middleware/__init__.py
+-rw-r--r--   0 danush     (501) staff       (20)     1648 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/flaskutils/http/middleware/filters.py
+-rw-r--r--   0 danush     (501) staff       (20)      190 2023-04-03 18:14:50.000000 appscommon-0.0.2/src/appscommon/flaskutils/http/utils.py
+-rw-r--r--   0 danush     (501) staff       (20)      964 2023-06-16 10:57:34.000000 appscommon-0.0.2/src/appscommon/logconfig.py
+-rw-r--r--   0 danush     (501) staff       (20)      269 2023-05-29 10:41:29.000000 appscommon-0.0.2/src/appscommon/readonly.py
+-rw-r--r--   0 danush     (501) staff       (20)      558 2023-06-16 10:58:09.000000 appscommon-0.0.2/src/appscommon/schemas.py
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.968445 appscommon-0.0.2/src/appscommon.egg-info/
+-rw-r--r--   0 danush     (501) staff       (20)      571 2023-07-10 06:49:45.000000 appscommon-0.0.2/src/appscommon.egg-info/PKG-INFO
+-rw-r--r--   0 danush     (501) staff       (20)     1169 2023-07-10 06:49:45.000000 appscommon-0.0.2/src/appscommon.egg-info/SOURCES.txt
+-rw-r--r--   0 danush     (501) staff       (20)        1 2023-07-10 06:49:45.000000 appscommon-0.0.2/src/appscommon.egg-info/dependency_links.txt
+-rw-r--r--   0 danush     (501) staff       (20)       30 2023-07-10 06:49:45.000000 appscommon-0.0.2/src/appscommon.egg-info/requires.txt
+-rw-r--r--   0 danush     (501) staff       (20)       11 2023-07-10 06:49:45.000000 appscommon-0.0.2/src/appscommon.egg-info/top_level.txt
+drwxr-xr-x   0 danush     (501) staff       (20)        0 2023-07-10 06:49:45.972806 appscommon-0.0.2/tests/
+-rw-r--r--   0 danush     (501) staff       (20)      453 2023-04-03 18:14:50.000000 appscommon-0.0.2/tests/test_logconfig.py
```

### Comparing `appscommon-0.0.1/PKG-INFO` & `appscommon-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: appscommon
-Version: 0.0.1
-Summary: Common utility package.
-Author-email: Danush Kumar Baskarraj <danushkumar.baskar@gmail.com>
-Project-URL: Homepage, https://github.com/danushk97/componenet-appscommon
-Project-URL: Bug Tracker, https://github.com/danushk97/componenet-appscommon/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# apputils Package
-
-All the common functionalities that are used project wide are maintained here.
+Metadata-Version: 2.1
+Name: appscommon
+Version: 0.0.2
+Summary: Common utility package.
+Author-email: Danush Kumar Baskarraj <danushkumar.baskar@gmail.com>
+Project-URL: Homepage, https://github.com/danushk97/componenet-appscommon
+Project-URL: Bug Tracker, https://github.com/danushk97/componenet-appscommon/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+# apputils Package
+
+All the common functionalities that are used project wide are maintained here.
```

### Comparing `appscommon-0.0.1/src/appscommon/db/adapters/unit_of_work.py` & `appscommon-0.0.2/src/appscommon/db/adapters/unit_of_work.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""
-This module holds the unit of work class for sqlalchemy.
-"""
-
-from appscommon.db.interfaces.unit_of_work import AbstractUnitOfWork
-
-
-class UnitOfWork(AbstractUnitOfWork):
-    """
-    Handles and keeps track of all the transaction made with the database and
-    also handles the database session.
-
-    Attributes:
-        session_factory: A session maker that should return a db session object.
-    """
-    def __init__(self, session_factory):
-        """
-        Instantiates the class.
-        """
-        self._session_factory = session_factory
-
-    def __enter__(self):
-        """
-        Gets executed when this instance of class is used with "with" statement.
-        """
-        self._session = self._session_factory()
-
-        return super().__enter__()
-
-    def commit(self) -> None:
-        """
-        Saves all the changes whcih was made during the current database
-        session.
-        """
-        self._session.commit()
-
-    def flush(self) -> None:
-        """
-        Saves all the changes whcih was made during the current database
-        session.
-        """
-        self._session.flush()
-
-    def rollback(self) -> None:
-        """
-        Discards all the changes whcih was made after the latest commit.
-        """
-        self._session.rollback()
-
-    def end_session(self) -> None:
-        """
-        Closes the current DB session.
-        """
-        self._session.close()
+"""
+This module holds the unit of work class for sqlalchemy.
+"""
+
+from appscommon.db.interfaces.unit_of_work import AbstractUnitOfWork
+
+
+class UnitOfWork(AbstractUnitOfWork):
+    """
+    Handles and keeps track of all the transaction made with the database and
+    also handles the database session.
+
+    Attributes:
+        session_factory: A session maker that should return a db session object.
+    """
+    def __init__(self, session_factory):
+        """
+        Instantiates the class.
+        """
+        self._session_factory = session_factory
+
+    def __enter__(self):
+        """
+        Gets executed when this instance of class is used with "with" statement.
+        """
+        self._session = self._session_factory()
+
+        return super().__enter__()
+
+    def commit(self) -> None:
+        """
+        Saves all the changes whcih was made during the current database
+        session.
+        """
+        self._session.commit()
+
+    def flush(self) -> None:
+        """
+        Saves all the changes whcih was made during the current database
+        session.
+        """
+        self._session.flush()
+
+    def rollback(self) -> None:
+        """
+        Discards all the changes whcih was made after the latest commit.
+        """
+        self._session.rollback()
+
+    def end_session(self) -> None:
+        """
+        Closes the current DB session.
+        """
+        self._session.close()
```

### Comparing `appscommon-0.0.1/src/appscommon/exception/exceptions.py` & `appscommon-0.0.2/src/appscommon/exception/exceptions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-"""
-This module holds the exception classes.
-"""
-
-from http import HTTPStatus
-
-from appscommon.exception.message import ErrorMessage
-from appscommon.enums import ResponseStatusEnum
-
-
-class AppException(Exception):
-    """
-    Base Exception class which should be inherited any other app exception
-    classes.
-
-    Attributes:
-        type (str): A URI reference that identifies the problem type.When this member is not present,
-                    its value is assumed to be "about:blank".
-        title (str): A short, human-readable summary of the problem type.
-        detail (str): A human-readable explanation specific to this occurrence of the problem.
-        status (int): The HTTP status code.
-    """
-    def __init__(self,
-        type: str = 'about:blank',
-        title: str = ErrorMessage.INTERNAL_SERVER_ERROR,
-        detail: str = ErrorMessage.INTERNAL_SERVER_ERROR,
-        status: int = HTTPStatus.INTERNAL_SERVER_ERROR,
-        log_message: str = None
-    ) -> None:
-        """
-        Intansiates the class.
-        """
-        self.type = type
-        self.title = title
-        self.detail = detail
-        self.status = status
-        self._log_message = log_message
-
-    def dict(self) -> dict:
-        return {
-            'type': self.type,
-            'title': self.title,
-            'detail': self.detail,
-            'status': ResponseStatusEnum.FAILURE.value
-        }
-
-    def __str__(self) -> str:
-        message = f'<{type(self).__name__}> {self._log_message or self.detail}'
-        if self.__cause__:
-            message += f' [CAUSE]: {self.__cause__}'
-
-        return message
-
-
-class InvalidParamsException(AppException):
-    """
-    This class represents invalid params exception which should be raised whenever a request parameters did not
-    validate.
-
-    Args:
-        invalid_params (list): A list of dict containing invalid field/param name and a reason.
-    """
-    def __init__(self,
-        invalid_params: list,
-        type: str = 'about:blank',
-        title: str = ErrorMessage.VALIDATION_ERROR,
-        detail: str = ErrorMessage.REQUEST_PARAMS_DID_NOT_VALIDATE,
-        status: int = HTTPStatus.BAD_REQUEST
-    ) -> None:
-        super().__init__(type, title, detail, status, invalid_params)
-        self.invalid_params = invalid_params
-
-    def dict(self) -> dict:
-        return {
-            **super().dict(),
-            'invalid_params': self.invalid_params
-        }
+"""
+This module holds the exception classes.
+"""
+
+from http import HTTPStatus
+
+from appscommon.exception.message import ErrorMessage
+from appscommon.enums import ResponseStatusEnum
+
+
+class AppException(Exception):
+    """
+    Base Exception class which should be inherited any other app exception
+    classes.
+
+    Attributes:
+        type (str): A URI reference that identifies the problem type.When this member is not present,
+                    its value is assumed to be "about:blank".
+        title (str): A short, human-readable summary of the problem type.
+        detail (str): A human-readable explanation specific to this occurrence of the problem.
+        status (int): The HTTP status code.
+    """
+    def __init__(self,
+        type: str = 'about:blank',
+        title: str = ErrorMessage.INTERNAL_SERVER_ERROR,
+        detail: str = ErrorMessage.INTERNAL_SERVER_ERROR,
+        status: int = HTTPStatus.INTERNAL_SERVER_ERROR,
+        log_message: str = None
+    ) -> None:
+        """
+        Intansiates the class.
+        """
+        self.type = type
+        self.title = title
+        self.detail = detail
+        self.status = status
+        self._log_message = log_message
+
+    def dict(self) -> dict:
+        return {
+            'type': self.type,
+            'title': self.title,
+            'detail': self.detail,
+            'status': ResponseStatusEnum.FAILURE.value
+        }
+
+    def __str__(self) -> str:
+        message = f'<{type(self).__name__}> {self._log_message or self.detail}'
+        if self.__cause__:
+            message += f' [CAUSE]: {self.__cause__}'
+
+        return message
+
+
+class InvalidParamsException(AppException):
+    """
+    This class represents invalid params exception which should be raised whenever a request parameters did not
+    validate.
+
+    Args:
+        invalid_params (list): A list of dict containing invalid field/param name and a reason.
+    """
+    def __init__(self,
+        invalid_params: list,
+        type: str = 'about:blank',
+        title: str = ErrorMessage.VALIDATION_ERROR,
+        detail: str = ErrorMessage.REQUEST_PARAMS_DID_NOT_VALIDATE,
+        status: int = HTTPStatus.BAD_REQUEST
+    ) -> None:
+        super().__init__(type, title, detail, status, invalid_params)
+        self.invalid_params = invalid_params
+
+    def dict(self) -> dict:
+        return {
+            **super().dict(),
+            'invalid_params': self.invalid_params
+        }
```

### Comparing `appscommon-0.0.1/src/appscommon/exception/handler.py` & `appscommon-0.0.2/src/appscommon/exception/handler.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-This module holds the class which is responsible for handling errors.
-"""
-
-from logging import getLogger
-from http import HTTPStatus
-
-from appscommon.exception import AppException
-from appscommon.exception.message import ErrorMessage
-
-
-_logger = getLogger(__name__)
-
-
-class ErrorHandler:
-    """
-    Holds the HTTP error handler functions.
-    """
-    @staticmethod
-    def page_not_found_handler(error: Exception) -> tuple:
-        """
-        Handles the Page not found error.
-
-        Args:
-            error (Exception):
-
-        Returns:
-            response_content (str), status (HttpStatus):
-        """
-        _logger.error(error)
-        return '404 page not found', HTTPStatus.NOT_FOUND
-
-    @staticmethod
-    def method_not_allowed_handler(error: Exception) -> tuple:
-        """
-        Handles the Page not found error.
-
-        Args:
-            error (Exception):
-
-        Returns:
-            response_dict (common.schemas.ErrorResponseSchema), status (HttpStatus):
-        """
-        exc = AppException(
-            title=ErrorMessage.INVALID_HTTP_METHOD,
-            detail=ErrorMessage.METHOD_NOT_ALLOWED,
-            status=HTTPStatus.METHOD_NOT_ALLOWED
-        )
-        exc.__cause__ = error
-        _logger.error(exc)
-        return exc.dict(), HTTPStatus.METHOD_NOT_ALLOWED
+"""
+This module holds the class which is responsible for handling errors.
+"""
+
+from logging import getLogger
+from http import HTTPStatus
+
+from appscommon.exception import AppException
+from appscommon.exception.message import ErrorMessage
+
+
+_logger = getLogger(__name__)
+
+
+class ErrorHandler:
+    """
+    Holds the HTTP error handler functions.
+    """
+    @staticmethod
+    def page_not_found_handler(error: Exception) -> tuple:
+        """
+        Handles the Page not found error.
+
+        Args:
+            error (Exception):
+
+        Returns:
+            response_content (str), status (HttpStatus):
+        """
+        _logger.error(error)
+        return '404 page not found', HTTPStatus.NOT_FOUND
+
+    @staticmethod
+    def method_not_allowed_handler(error: Exception) -> tuple:
+        """
+        Handles the Page not found error.
+
+        Args:
+            error (Exception):
+
+        Returns:
+            response_dict (common.schemas.ErrorResponseSchema), status (HttpStatus):
+        """
+        exc = AppException(
+            title=ErrorMessage.INVALID_HTTP_METHOD,
+            detail=ErrorMessage.METHOD_NOT_ALLOWED,
+            status=HTTPStatus.METHOD_NOT_ALLOWED
+        )
+        exc.__cause__ = error
+        _logger.error(exc)
+        return exc.dict(), HTTPStatus.METHOD_NOT_ALLOWED
```

### Comparing `appscommon-0.0.1/src/appscommon/flaskutils/confighelper.py` & `appscommon-0.0.2/src/appscommon/flaskutils/confighelper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import importlib
-import inspect
-from logging import getLogger
-from os import abort
-from typing import Callable, Dict
-from flask import Flask
-
-
-from appscommon.exception.handler import ErrorHandler
-
-
-_logger = getLogger(__name__)
-
-
-def ensure_configs(config: dict, required_configs: list) -> None:
-    """
-    Aborts application start up if there is any empty config values. It should be called at the application startup.
-
-    Args:
-        config (dict): A dictionary of configs.
-        required_configs (list): A list of must have configs.
-    """
-    _logger.info('Valdating configs...')
-    missing_configs = []
-    for key in required_configs:
-        value = config[key]
-        if value is None or str(value).strip() == '':
-            missing_configs.append(key)
-
-    if missing_configs:
-        _logger.critical(f'Aborting process due to missing configs: {missing_configs}')
-        abort()
-
-    _logger.info('Config validation was successful.')
-
-
-def inject_dependencies(dependents: Dict[str, Callable], providers: dict) -> dict:
-    """
-    Injects dependencies.
-
-    Args:
-        dependents (dict): Key can be any string which uniquely identifies the dependant and the value must be
-                           any callable.
-        providers (dict): Key should be name of the dependency and value should be the actual value which `dependents`
-                          depend upon.
-
-    Returns:
-        (dict): injected dependents.
-    """
-    _logger.info('Injecting dependencies....')
-    rescued_dependents = {}
-
-    for key, dependent in dependents.items():
-        injections = {}
-        for param in inspect.signature(dependent).parameters:
-            if param in providers:
-                injections[param] = providers[param]
-
-        rescued_dependents[key] = lambda *args, injections=injections, value=dependent: value(*args, **injections)
-
-    return rescued_dependents
-
-
-def register_blueprints(flask_app: Flask, module_paths: list) -> None:
-    """
-    Registers blueprints with the app instance.
-
-    Args:
-        flask_app (Flask): Instance of wsgi app.
-        route_modules (list): List of tuples/lists containing module path and name of blueprint attribute.
-    """
-    _logger.info('Registering routes/blueprints....')
-    for module, blueprint_attr in module_paths:
-        module = importlib.import_module(module)
-        blueprint = getattr(module, blueprint_attr)
-        flask_app.register_blueprint(blueprint)  # registering routes.
-
-
-def register_http_error_handlers(flask_app: Flask) -> None:
-    """
-    Registers error handlers.
-
-    Args:
-        flask_app (Flask): Instance of flask_app.
-    """
-    _logger.info('Registering http error handlers for flask app...')
-    flask_app.register_error_handler(404, ErrorHandler.page_not_found_handler)
-    flask_app.register_error_handler(405, ErrorHandler.method_not_allowed_handler)
+import importlib
+import inspect
+from logging import getLogger
+from os import abort
+from typing import Callable, Dict
+from flask import Flask
+
+
+from appscommon.exception.handler import ErrorHandler
+
+
+_logger = getLogger(__name__)
+
+
+def ensure_configs(config: dict, required_configs: list) -> None:
+    """
+    Aborts application start up if there is any empty config values. It should be called at the application startup.
+
+    Args:
+        config (dict): A dictionary of configs.
+        required_configs (list): A list of must have configs.
+    """
+    _logger.info('Valdating configs...')
+    missing_configs = []
+    for key in required_configs:
+        value = config[key]
+        if value is None or str(value).strip() == '':
+            missing_configs.append(key)
+
+    if missing_configs:
+        _logger.critical(f'Aborting process due to missing configs: {missing_configs}')
+        abort()
+
+    _logger.info('Config validation was successful.')
+
+
+def inject_dependencies(dependents: Dict[str, Callable], providers: dict) -> dict:
+    """
+    Injects dependencies.
+
+    Args:
+        dependents (dict): Key can be any string which uniquely identifies the dependant and the value must be
+                           any callable.
+        providers (dict): Key should be name of the dependency and value should be the actual value which `dependents`
+                          depend upon.
+
+    Returns:
+        (dict): injected dependents.
+    """
+    _logger.info('Injecting dependencies....')
+    rescued_dependents = {}
+
+    for key, dependent in dependents.items():
+        injections = {}
+        for param in inspect.signature(dependent).parameters:
+            if param in providers:
+                injections[param] = providers[param]
+
+        rescued_dependents[key] = lambda *args, injections=injections, value=dependent: value(*args, **injections)
+
+    return rescued_dependents
+
+
+def register_blueprints(flask_app: Flask, module_paths: list) -> None:
+    """
+    Registers blueprints with the app instance.
+
+    Args:
+        flask_app (Flask): Instance of wsgi app.
+        route_modules (list): List of tuples/lists containing module path and name of blueprint attribute.
+    """
+    _logger.info('Registering routes/blueprints....')
+    for module, blueprint_attr in module_paths:
+        module = importlib.import_module(module)
+        blueprint = getattr(module, blueprint_attr)
+        flask_app.register_blueprint(blueprint)  # registering routes.
+
+
+def register_http_error_handlers(flask_app: Flask) -> None:
+    """
+    Registers error handlers.
+
+    Args:
+        flask_app (Flask): Instance of flask_app.
+    """
+    _logger.info('Registering http error handlers for flask app...')
+    flask_app.register_error_handler(404, ErrorHandler.page_not_found_handler)
+    flask_app.register_error_handler(405, ErrorHandler.method_not_allowed_handler)
```

### Comparing `appscommon-0.0.1/src/appscommon/flaskutils/http/middleware/filters.py` & `appscommon-0.0.2/src/appscommon/flaskutils/http/middleware/filters.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from functools import wraps
-from logging import getLogger
-from time import perf_counter
-from flask import request
-from typing import Callable
-from http import HTTPStatus
-from werkzeug.exceptions import HTTPException
-
-from appscommon.exception import AppException, InvalidParamsException
-from pydantic import ValidationError
-
-
-_logger = getLogger(__name__)
-
-
-def error_filter(source: Callable) -> Callable:
-    @wraps(source)  # Helps to retain the metadata of the actual source function.
-    def wrapper(*args, **kwargs):
-        tic = perf_counter()
-        _logger.info(f'Starting to process {request.path}.')
-        try:
-            data = source(*args, **kwargs)
-        except Exception as err:
-            if isinstance(err, AppException):
-                exc = err
-            elif isinstance(err, HTTPException) and hasattr(err, 'response') and \
-                    err.response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-                errors = [
-                    {'field': err.pop('loc'), 'msg': err.pop('msg', 'unknown error.')}
-                    for err in err.response.json
-                ]
-                exc = InvalidParamsException(invalid_params=errors)
-                _logger.error(exc, exc_info=True)
-
-                return exc.dict(), exc.status
-            else:
-                exc = AppException()
-                exc.__cause__ = err
-
-            _logger.error(exc, exc_info=True)
-
-            return exc.dict(), exc.status
-        finally:
-            toc = perf_counter()
-            _logger.info(f'Completed processing {request.path} in {toc - tic:.3f} seconds.')
-
-        return data
-
-    return wrapper
+from functools import wraps
+from logging import getLogger
+from time import perf_counter
+from flask import request
+from typing import Callable
+from http import HTTPStatus
+from werkzeug.exceptions import HTTPException
+
+from appscommon.exception import AppException, InvalidParamsException
+from pydantic import ValidationError
+
+
+_logger = getLogger(__name__)
+
+
+def error_filter(source: Callable) -> Callable:
+    @wraps(source)  # Helps to retain the metadata of the actual source function.
+    def wrapper(*args, **kwargs):
+        tic = perf_counter()
+        _logger.info(f'Starting to process {request.path}.')
+        try:
+            data = source(*args, **kwargs)
+        except Exception as err:
+            if isinstance(err, AppException):
+                exc = err
+            elif isinstance(err, HTTPException) and hasattr(err, 'response') and \
+                    err.response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+                errors = [
+                    {'field': err.pop('loc'), 'msg': err.pop('msg', 'unknown error.')}
+                    for err in err.response.json
+                ]
+                exc = InvalidParamsException(invalid_params=errors)
+                _logger.error(exc, exc_info=True)
+
+                return exc.dict(), exc.status
+            else:
+                exc = AppException()
+                exc.__cause__ = err
+
+            _logger.error(exc, exc_info=True)
+
+            return exc.dict(), exc.status
+        finally:
+            toc = perf_counter()
+            _logger.info(f'Completed processing {request.path} in {toc - tic:.3f} seconds.')
+
+        return data
+
+    return wrapper
```

### Comparing `appscommon-0.0.1/src/appscommon/logconfig.py` & `appscommon-0.0.2/src/appscommon/logconfig.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-import logging
-import sys
-from uuid import uuid4
-
-from flask import has_request_context, g, request
-
-
-class RequestFormatter(logging.Formatter):
-    def format(self, record):
-        record.request_id = self.get_flask_request_id()
-
-        return super().format(record)
-
-    def get_flask_request_id(self):
-        if not has_request_context():
-            return ''
-
-        request_id = g.get('request_id')
-        if request_id:
-            return request_id
-
-        g.request_id = request.headers.get('x-request-id') or uuid4()
-
-        return g.get('request_id')
-
-
-def init_logging():
-    handler = logging.StreamHandler(sys.stdout)
-    handler.setFormatter(RequestFormatter(
-        '%(asctime)s.%(msecs)03d %(levelname)s %(request_id)s [%(name)s.%(funcName)s:%(lineno)d] %(message)s'
-    ))
-    logging.basicConfig(
-        level=logging.DEBUG,
-        datefmt='%d/%b/%Y %H:%M:%S',
-        handlers=[handler]
-    )
+"""
+This module contains logconfig.
+"""
+
+import logging
+import sys
+from uuid import uuid4
+
+from flask import has_request_context, g, request
+
+
+class RequestFormatter(logging.Formatter):
+    def format(self, record):
+        record.request_id = self.get_flask_request_id()
+
+        return super().format(record)
+
+    def get_flask_request_id(self):
+        if not has_request_context():
+            return ''
+
+        request_id = g.get('request_id')
+        if request_id:
+            return request_id
+
+        g.request_id = request.headers.get('x-request-id') or uuid4()
+
+        return g.get('request_id')
+
+
+def init_logging():
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setFormatter(RequestFormatter(
+        '%(asctime)s.%(msecs)03d %(levelname)s %(request_id)s [%(name)s.%(funcName)s:%(lineno)d] %(message)s'
+    ))
+    logging.basicConfig(
+        level=logging.DEBUG,
+        datefmt='%d/%b/%Y %H:%M:%S',
+        handlers=[handler]
+    )
```

### Comparing `appscommon-0.0.1/src/appscommon.egg-info/PKG-INFO` & `appscommon-0.0.2/src/appscommon.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: appscommon
-Version: 0.0.1
-Summary: Common utility package.
-Author-email: Danush Kumar Baskarraj <danushkumar.baskar@gmail.com>
-Project-URL: Homepage, https://github.com/danushk97/componenet-appscommon
-Project-URL: Bug Tracker, https://github.com/danushk97/componenet-appscommon/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# apputils Package
-
-All the common functionalities that are used project wide are maintained here.
+Metadata-Version: 2.1
+Name: appscommon
+Version: 0.0.2
+Summary: Common utility package.
+Author-email: Danush Kumar Baskarraj <danushkumar.baskar@gmail.com>
+Project-URL: Homepage, https://github.com/danushk97/componenet-appscommon
+Project-URL: Bug Tracker, https://github.com/danushk97/componenet-appscommon/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+# apputils Package
+
+All the common functionalities that are used project wide are maintained here.
```

### Comparing `appscommon-0.0.1/src/appscommon.egg-info/SOURCES.txt` & `appscommon-0.0.2/src/appscommon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/appscommon/__init__.py
 src/appscommon/logconfig.py
 src/appscommon/readonly.py
 src/appscommon/schemas.py
 src/appscommon.egg-info/PKG-INFO
 src/appscommon.egg-info/SOURCES.txt
 src/appscommon.egg-info/dependency_links.txt
+src/appscommon.egg-info/requires.txt
 src/appscommon.egg-info/top_level.txt
 src/appscommon/db/adapters/__init__.py
 src/appscommon/db/adapters/unit_of_work.py
 src/appscommon/db/interfaces/__init__.py
 src/appscommon/db/interfaces/repository.py
 src/appscommon/db/interfaces/unit_of_work.py
 src/appscommon/domain/__init__.py
```

