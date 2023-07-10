# Comparing `tmp/signhost_api_python_client-0.2.0.tar.gz` & `tmp/signhost_api_python_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signhost_api_python_client-0.2.0.tar", max compression
+gzip compressed data, was "signhost_api_python_client-0.3.0.tar", max compression
```

## Comparing `signhost_api_python_client-0.2.0.tar` & `signhost_api_python_client-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     3469 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/README.md
--rw-r--r--   0        0        0     2089 2023-04-21 13:49:39.525717 signhost_api_python_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/src/signhost/__init__.py
--rw-r--r--   0        0        0     3501 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/src/signhost/__main__.py
--rw-r--r--   0        0        0      147 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/src/signhost/client/__init__.py
--rw-r--r--   0        0        0    10688 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/client/client.py
--rw-r--r--   0        0        0      449 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/client/errors.py
--rw-r--r--   0        0        0       33 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/__init__.py
--rw-r--r--   0        0        0     1176 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/enums.py
--rw-r--r--   0        0        0    17297 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/generated.py
--rw-r--r--   0        0        0     5373 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/verifications.py
--rw-r--r--   0        0        0        0 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/py.typed
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 signhost_api_python_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-10 15:01:28.765344 signhost_api_python_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3712 2023-07-10 15:01:28.765344 signhost_api_python_client-0.3.0/README.md
+-rw-r--r--   0        0        0     2089 2023-07-10 15:01:51.553854 signhost_api_python_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/__init__.py
+-rw-r--r--   0        0        0     3493 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/__main__.py
+-rw-r--r--   0        0        0      285 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/client/__init__.py
+-rw-r--r--   0        0        0     4409 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/client/asyncio.py
+-rw-r--r--   0        0        0     2720 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/client/base.py
+-rw-r--r--   0        0        0     3759 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/client/default.py
+-rw-r--r--   0        0        0      449 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/client/errors.py
+-rw-r--r--   0        0        0      676 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/client/utils.py
+-rw-r--r--   0        0        0      145 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/models/__init__.py
+-rw-r--r--   0        0        0     1764 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/models/enums.py
+-rw-r--r--   0        0        0      969 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/models/forms.py
+-rw-r--r--   0        0        0    15018 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/models/generated.py
+-rw-r--r--   0        0        0     1514 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/models/location.py
+-rw-r--r--   0        0        0     4813 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/models/verifications.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:01:28.769345 signhost_api_python_client-0.3.0/src/signhost/py.typed
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 signhost_api_python_client-0.3.0/PKG-INFO
```

### Comparing `signhost_api_python_client-0.2.0/LICENSE` & `signhost_api_python_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signhost_api_python_client-0.2.0/README.md` & `signhost_api_python_client-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 - 100% test coverage
 
 ## Requirements
 
 - httpx
 - pydantic
-- attr
+- attrs
 - click
 
 ## Installation
 
 You can install _Signhost Api Python Client_ via [pip] from [PyPI]:
 
 ```console
@@ -61,14 +61,23 @@
 print("Sign the contract over here", transaction.Signers[0].SignUrl)
 
 signhost.transaction_get(transaction.Id)
 signhost.transaction_file_get(transaction.Id, "file.pdf")
 signhost.receipt_get(transaction.Id)
 ```
 
+### Async support
+
+```python
+from signhost.client import AsyncClient
+
+async with AsyncClient(api_key="str", app_key="str") as signhost:
+    signhost.transaction_get("xyz")
+```
+
 Please see the [Command-line Reference] for details.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
@@ -80,16 +89,17 @@
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
 ## Credits
 
-This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+This project was initiated by [dok.legal] and was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
 
+[dok.legal]: https://dok.legal/
 [@cjolowicz]: https://github.com/cjolowicz
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [file an issue]: https://github.com/foarsitter/signhost-api-python-client/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
```

### Comparing `signhost_api_python_client-0.2.0/pyproject.toml` & `signhost_api_python_client-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "signhost-api-python-client"
-version = "0.2.0"
+version = "0.3.0"
 description = "Signhost Api Python Client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/signhost-api-python-client"
 repository = "https://github.com/foarsitter/signhost-api-python-client"
 documentation = "https://signhost-api-python-client.readthedocs.io"
@@ -17,17 +17,17 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/foarsitter/signhost-api-python-client/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=8.0.1"
-httpx = "^0.23.3"
-pydantic = "^1.10.4"
-attrs = "^22.2.0"
+httpx = "^0.24.1"
+pydantic = ">=2.0.1"
+attrs = "^23.1.0"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `signhost_api_python_client-0.2.0/src/signhost/__main__.py` & `signhost_api_python_client-0.3.0/src/signhost/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 from json import JSONDecodeError
 from pathlib import Path
 
 import click
 import httpx
 
+from signhost.client import DefaultClient
 from signhost.client import RequestFixtures
-from signhost.client.client import DefaultClient
 from signhost.models import Signer
 from signhost.models import Transaction
 from signhost.models import verifications
 from signhost.models.enums import Language
 
 
 @click.group()
@@ -106,15 +106,14 @@
 
 
 class ResponseStorage:
     def __init__(self) -> None:
         self.responses: RequestFixtures = {}
 
     def __call__(self, response: httpx.Response) -> None:
-
         response.read()
 
         try:
             data = response.json()
         except (JSONDecodeError, UnicodeDecodeError):
             data = {"binary": True}
```

### Comparing `signhost_api_python_client-0.2.0/src/signhost/models/enums.py` & `signhost_api_python_client-0.3.0/src/signhost/models/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,7 +61,31 @@
 
 
 class FormSetType(Enum):
     Seal = "Seal"
     Signature = "Signature"
     Check = "Check"
     SingleLine = "SingleLine"
+
+
+class VerificationType(Enum):
+    Consent = "Consent"
+    DigiD = "DigiD"
+    eHerkenning = "eHerkenning"
+    eIDAS_Login = "eIDAS Login"
+    iDeal = "iDeal"
+    iDIN = "iDIN"
+    itsme_Identification = "itsme Identification"
+    PhoneNumber = "PhoneNumber"
+    Scribble = "Scribble"
+    itsme_sign = "itsme sign"
+    SigningCertificate = "SigningCertificate"
+    SURFnet = "SURFnet"
+    ZealiD_Qualified = "ZealiD Qualified"
+    IPAddress = "IPAddress"
+
+
+class Betrouwbaarheidsniveau(Enum):
+    Basis = "Basis"
+    Midden = "Midden"
+    Substantieel = "Substantieel"
+    Hoog = "Hoog"
```

### Comparing `signhost_api_python_client-0.2.0/src/signhost/models/generated.py` & `signhost_api_python_client-0.3.0/src/signhost/models/generated.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,23 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
-from signhost.models.enums import Betrouwbaarheidsniveau1
-from signhost.models.enums import Code
-from signhost.models.enums import FormSetType
-from signhost.models.enums import Language
-from signhost.models.enums import Rel
-from signhost.models.enums import Status
-from signhost.models.enums import Type
+from signhost.models import enums
+from signhost.models import forms
 from signhost.models.verifications import Verification
 from signhost.models.verifications import VerificationAnnotatedType
 
 
 class Activity(BaseModel):
     Id: Optional[str] = None
-    Code: Optional[Code] = Field(
+    Code: Optional[enums.Code] = Field(
         None,
         description="* 101 -\tInvitation sent\n"
         "* 102 -\tReceived\n"
         "* 103 -\tOpened\n"
         "* 104 -\tReminder sent\n"
         "* 105 -\tDocument opened, Info property contains the file id of the opened document.\n"
         "* 201 -\tCancelled\n"
@@ -75,93 +70,37 @@
         None,
         description="Any valid json object which we will return back to you when "
         "doing a GET on the transaction or when we send a postback.",
     )
 
 
 class Authentication(BaseModel):
-    Type: Type = Field(
+    Type: enums.Type = Field(
         ...,
         description="Type of the authentication object.\n"
         "The `Type` property **must** be the first property in the json!\n\n"
         "The order in which the authentications are provided determine "
         "in which order the signer will have to perform the specified method.\n",
     )
 
 
 class Link(BaseModel):
-    Rel: Optional[Rel] = Field(None, description="The type of file you can download.")
+    Rel: Optional[enums.Rel] = Field(
+        None, description="The type of file you can download."
+    )
     Type: Optional[str] = Field(
         None,
         description="The type of the file you can expect to download. "
         "Include this in your 'Accept' header when requesting the file.",
     )
     Link: Optional[str] = Field(
         None, description="Url containing the link to the file."
     )
 
 
-class Signers(BaseModel):
-    FormSets: Optional[List[str]] = Field(
-        None, description="List of formset keys to be assigned to this signer."
-    )
-
-
-class Location(BaseModel):
-    Search: Optional[str] = Field(
-        None,
-        description="The text to search in the pdf document to use as "
-        "the position for the field. For example `{{Signer1}}`.",
-    )
-    Occurence: Optional[int] = Field(
-        None, description="When using text search, only match this matched occurence."
-    )
-    Top: Optional[int] = Field(
-        None, description="Offset from the top of the search text or the page"
-    )
-    Right: Optional[int] = Field(
-        None, description="Offset from the right of the search or the page"
-    )
-    Bottom: Optional[int] = Field(
-        None, description="Offset from the bottom of the search or the page"
-    )
-    Left: Optional[int] = Field(
-        None, description="Offset from the left of the search or the page"
-    )
-    Width: Optional[int] = Field(
-        None,
-        description="The width of the field, can’t be used when both Left and Right are specified.\n"
-        "For signature and seal fields we suggest a width of 140.\n",
-    )
-    Height: Optional[int] = Field(
-        None,
-        description="The height of the field, can’t be used when both Bottom and Top are specified.\n"
-        "For signature and seal fields we suggest a height of 70.\n",
-    )
-    PageNumber: Optional[int] = Field(
-        None, description="On which page the field should be placed."
-    )
-
-
-class FormSets(BaseModel):
-    Type: Optional[FormSetType] = Field(
-        None,
-        description="Field type to create.\n"
-        "\n"
-        "* Seal is not yet implemented, this will specify the properties of a seal.\n"
-        "* Signature, specifies a signature field\n"
-        "* Check, specifies a checkbox. You'll have to set the `value` property\n"
-        "* SingleLine, specifies a single line textbox\n",
-    )
-    Location: Optional[Location] = Field(
-        None,
-        description="Specify where the field should be placed within the document.",
-    )
-
-
 class FileMetaData(BaseModel):
     DisplayOrder: Optional[int] = Field(
         None, description="With what order number we'll display the file to the signer"
     )
     DisplayName: Optional[str] = Field(
         None, description="With what name we'll display the file to the signer"
     )
@@ -170,19 +109,19 @@
         description=(
             "Places a copy of the signer's scribble image on the bottom right of every page where no signature is "
             "present.\n"
             "Note: due to the nature of advanced or qualified digital signatures, paraphs are merely a cosmetic "
             "addition.\n"
         ),
     )
-    Signers: Optional[Dict[str, Signers]] = Field(
+    Signers: Optional[Dict[str, forms.Signers]] = Field(
         None,
         description="Map of array of formsets.\nEach key should be a valid signer id.\n",
     )
-    FormSets: Optional[Dict[str, Dict[str, FormSets]]] = Field(
+    FormSets: Optional[Dict[str, Dict[str, forms.FormSets]]] = Field(
         None,
         description="Map of one or more form set definitions.\n"
         "The key of the map will be the formset name.\n"
         "The value will be the formset definition\n",
     )
 
 
@@ -194,29 +133,29 @@
 
 class DigiDAuthentication(Authentication):
     Bsn: Optional[str] = Field(
         None,
         description="The provided value must match the BSN of the credentials returned by DigiD.\n"
         "The BSN is required to match an '11-proef'.\n",
     )
-    Betrouwbaarheidsniveau: Optional[Betrouwbaarheidsniveau1] = Field(
+    Betrouwbaarheidsniveau: Optional[enums.Betrouwbaarheidsniveau1] = Field(
         None,
         description="The level of confidence with which the identity of the signer has been determined.\n"
         "For further information, please refer to [Logius](https://www.logius.nl/diensten/digid/hoe-werkt-het).\n",
     )
 
 
 class PhoneNumberAuthentication(Authentication):
     Number: Optional[str] = Field(
         None,
         description="The mobile phone number of the signer.\n"
         "Must conform to E.164,\n"
         "[the international public telecommunication numbering plan](https://en.wikipedia.org/wiki/E.164),\n"
         "which requires the country calling code (e.g. +31).\n",
-        example="+31123456789",
+        examples=["+31123456789"],
     )
 
 
 class EIDASLogin(Verification):
     Uid: Optional[str] = Field(
         None, description="The unique identifier returned by eIDAS Login."
     )
@@ -240,15 +179,15 @@
 class ItsmeIdentification(Verification):
     PhoneNumber: Optional[str] = Field(
         None,
         description="The mobile phone number of the signer.\n"
         "Must be conform E.164,\n"
         "[the international public telecommunication numbering plan](https://en.wikipedia.org/wiki/E.164),\n"
         "which requires the country calling code (Only the Belgian country calling code is supported: +32).\n",
-        example="+32123456789",
+        examples=["+32123456789"],
     )
     Attributes: Optional[List[str]] = Field(
         None,
         description="Contains all available itsme Identification attributes.\n"
         "These attributes may change, therefore we cannot guarantee the availability of any of these attributes.\n",
     )
 
@@ -270,15 +209,15 @@
         None,
         description="The id of the signer, must be unique within a transaction.\n"
         "If you don't provide an id we will generate one for you.\n",
     )
     Email: str = Field(
         ...,
         description="The e-mail address of the signer",
-        example="john.doe@example.com",
+        examples=["john.doe@example.com"],
     )
     IntroText: Optional[str] = Field(
         None,
         description="An intro text to show to the user during the sign proces.\n"
         "This will be shown on the first screen to the signer and supports limitted markdown markup.\n\n"
         "The following markup is supported:"
         "\n- `# Headings`"
@@ -331,16 +270,16 @@
         "\nRequired if `SendSignRequest` is true\n",
     )
     SendSignConfirmation: Optional[bool] = Field(
         None,
         description="Send the sign confirmation to the signer his e-mail address."
         "\nDefault value is the value of `SendSignRequest`\n",
     )
-    Language: Optional[Language] = Field(
-        Language.NL,
+    Language: Optional[enums.Language] = Field(
+        enums.Language.NL,
         description="The language of the receiving user, "
         "only de-DE, en-US, es-ES, fr-FR, it-IT, pl-PL and nl-NL are allowed.",
     )
     ScribbleName: Optional[str] = Field(
         None,
         description="The name of the signer, this will be pre filled in the scribble form.",
     )
@@ -388,15 +327,15 @@
         None,
         description="The id of the transaction.\n"
         "Currently this property is read only but this may change in the future.\n",
     )
     Files: Optional[Dict[str, FileEntry]] = Field(
         None, description="A map of files attached to this transaction."
     )
-    Language: Optional[Language] = Field(
+    Language: Optional[enums.Language] = Field(
         None,
         description="The language of the sender notifications and the receipt,"
         " only de-DE, en-US, es-ES, fr-FR, it-IT, pl-PL and nl-NL are allowed.",
     )
     Seal: Optional[bool] = Field(
         False, description="Seal the document before sending to the signers."
     )
@@ -416,15 +355,15 @@
     )
     DaysToExpire: Optional[int] = Field(
         60, description="Amount of days before expiration. Max 90 days."
     )
     SendEmailNotifications: Optional[bool] = Field(
         True, description="Send e-mail notifications to the sender."
     )
-    Status: Optional[Status] = Field(
+    Status: Optional[enums.Status] = Field(
         None,
         description="Current transaction status.\n\n"
         "* 5 - Waiting for document\n"
         "* 10 - Waiting for signer\n"
         "* 20 - In progress\n"
         "* 30 - Signed (end state)\n"
         "* 40 - Rejected (end state)\n"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `signhost_api_python_client-0.2.0/src/signhost/models/verifications.py` & `signhost_api_python_client-0.3.0/src/signhost/models/verifications.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,21 @@
 # flake8: noqa
 from __future__ import annotations
 
 from datetime import date
-from enum import Enum
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
 from typing_extensions import Annotated
 
-
-class VerificationType(Enum):
-    Consent = "Consent"
-    DigiD = "DigiD"
-    eHerkenning = "eHerkenning"
-    eIDAS_Login = "eIDAS Login"
-    iDeal = "iDeal"
-    iDIN = "iDIN"
-    itsme_Identification = "itsme Identification"
-    PhoneNumber = "PhoneNumber"
-    Scribble = "Scribble"
-    itsme_sign = "itsme sign"
-    SigningCertificate = "SigningCertificate"
-    SURFnet = "SURFnet"
-    ZealiD_Qualified = "ZealiD Qualified"
-    IPAddress = "IPAddress"
-
-
-class Betrouwbaarheidsniveau(Enum):
-    Basis = "Basis"
-    Midden = "Midden"
-    Substantieel = "Substantieel"
-    Hoog = "Hoog"
+from signhost.models import enums
 
 
 class Verification(BaseModel):
     pass
 
 
 class Consent(Verification):
@@ -48,15 +25,15 @@
 class DigiD(Verification):
     Type: Literal["DigiD"] = "DigiD"
     Bsn: Optional[str] = Field(
         None,
         description="When provided, the provided value must match the BSN of the credentials returned by DigiD.\nThe BSN is required to match an '11-proef'.\n",
         # noqa
     )
-    Betrouwbaarheidsniveau: Optional[Betrouwbaarheidsniveau] = Field(
+    Betrouwbaarheidsniveau: Optional[enums.Betrouwbaarheidsniveau] = Field(
         None,
         description="The level of confidence with which the identity of the signer has been determined.\nFor further information, please refer to [Logius](https://www.logius.nl/diensten/digid/hoe-werkt-het).\n",
         # noqa
     )
 
 
 class EHerkenning(Verification):
@@ -70,15 +47,15 @@
 
 class IDeal(Verification):
     Type: Literal["iDeal"] = "iDeal"
     Iban: Optional[str] = Field(
         None,
         description="The IBAN of the signer.\nWhen provided during the creation of the transaction this IBAN is\nverified during the verification flow to make sure these and the actual IBAN number match.\n",
         # noqa
-        example="NL13TEST0123456789",
+        examples=["NL13TEST0123456789"],
     )
     AccountHolderName: Optional[str] = None
     AccountHolderCity: Optional[str] = None
 
 
 class IDIN(Verification):
     Type: Literal["iDIN"] = "iDIN"
@@ -87,15 +64,15 @@
         description="Name of the idin consumer / signer.\nCurrently we don't support supplying a value in this property to ensure the expected account holder name matches.\nThis could change in the future.\n",
     )
     AccountHolderAddress1: Optional[str] = None
     AccountHolderAddress2: Optional[str] = None
     AccountHolderDateOfBirth: Optional[date] = Field(
         None,
         description="Date of birth of idin consumer / signer",
-        example="2001-12-31",
+        examples=["2001-12-31"],
     )
     Attributes: Optional[List[str]] = Field(
         None,
         description="Contains all available iDIN attributes.\nThese attributes may change, therefore we cannot guarantee the availability of any of these attributes.\n",
         # noqa
     )
 
@@ -109,15 +86,15 @@
     Type: Literal["PhoneNumber"] = "PhoneNumber"
     Number: Optional[str] = Field(
         None,
         description="The mobile phone number of the signer.\n"
         "Must conform to E.164,\n"
         "[the international public telecommunication numbering plan](https://en.wikipedia.org/wiki/E.164),\n"
         "which requires the country calling code (e.g. +31).\n",
-        example="+31123456789",
+        examples=["+31123456789"],
     )
 
 
 class Scribble(Verification):
     Type: Literal["Scribble"] = "Scribble"
     RequireHandsignature: Optional[bool] = Field(
         False,
```

### Comparing `signhost_api_python_client-0.2.0/PKG-INFO` & `signhost_api_python_client-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: signhost-api-python-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: Signhost Api Python Client
 Home-page: https://github.com/foarsitter/signhost-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: click (>=8.0.1)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: pydantic (>=2.0.1)
 Project-URL: Changelog, https://github.com/foarsitter/signhost-api-python-client/releases
 Project-URL: Documentation, https://signhost-api-python-client.readthedocs.io
 Project-URL: Repository, https://github.com/foarsitter/signhost-api-python-client
 Description-Content-Type: text/markdown
 
 # Signhost Api Python Client
 
@@ -51,15 +51,15 @@
 
 - 100% test coverage
 
 ## Requirements
 
 - httpx
 - pydantic
-- attr
+- attrs
 - click
 
 ## Installation
 
 You can install _Signhost Api Python Client_ via [pip] from [PyPI]:
 
 ```console
@@ -87,14 +87,23 @@
 print("Sign the contract over here", transaction.Signers[0].SignUrl)
 
 signhost.transaction_get(transaction.Id)
 signhost.transaction_file_get(transaction.Id, "file.pdf")
 signhost.receipt_get(transaction.Id)
 ```
 
+### Async support
+
+```python
+from signhost.client import AsyncClient
+
+async with AsyncClient(api_key="str", app_key="str") as signhost:
+    signhost.transaction_get("xyz")
+```
+
 Please see the [Command-line Reference] for details.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
@@ -106,16 +115,17 @@
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
 ## Credits
 
-This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+This project was initiated by [dok.legal] and was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
 
+[dok.legal]: https://dok.legal/
 [@cjolowicz]: https://github.com/cjolowicz
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [file an issue]: https://github.com/foarsitter/signhost-api-python-client/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
```

