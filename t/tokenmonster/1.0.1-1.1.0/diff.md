# Comparing `tmp/tokenmonster-1.0.1.tar.gz` & `tmp/tokenmonster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.0.1.tar", last modified: Tue Jul  4 14:27:30 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.0.tar", last modified: Mon Jul 10 16:12:50 2023, max compression
```

## Comparing `tokenmonster-1.0.1.tar` & `tokenmonster-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    13932 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14073 2023-07-04 14:20:37.000000 tokenmonster-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-04 14:26:38.000000 tokenmonster-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13932 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    36658 2023-07-04 14:07:40.000000 tokenmonster-1.0.1/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:12:50.975208 tokenmonster-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)    16110 2023-07-10 16:12:50.975208 tokenmonster-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-07-10 10:36:05.000000 tokenmonster-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 16:12:50.975208 tokenmonster-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-10 16:12:00.000000 tokenmonster-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:12:50.971208 tokenmonster-1.1.0/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16110 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    46197 2023-07-10 10:29:36.000000 tokenmonster-1.1.0/tokenmonster.py
```

### Comparing `tokenmonster-1.0.1/PKG-INFO` & `tokenmonster-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,108 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # TokenMonster
 
 1. [Usage](#usage)
-2. TokenMonster Methods
-    - [TokenMonster.\_\_init\_\_(path)](#tokenmonster__init__path)
-    - [TokenMonster.\_\_len\_\_()](#tokenmonster__len__)
-	- [vocab.save(fname)](#vocabsavefname)
+2. Loading & Exporting
+    - [tokenmonster.load(path)](#tokenmonsterloadpath)
+    - [tokenmonster.new(yaml)](#tokenmonsternewyaml)
+    - [vocab.save(fname)](#vocabsavefname)
+    - [vocab.export_yaml(order_by_score=False)](#vocabexport_yamlorder_by_scorefalse)
 3. Tokenization & Detokenization
-	- [vocab.tokenize(text)](#vocabtokenizetext)
-	- [vocab.decode(tokens)](#vocabdecodetokens)
+    - [vocab.tokenize(text)](#vocabtokenizetext)
+    - [vocab.decode(tokens)](#vocabdecodetokens)
     - [vocab.decoder()](#vocabdecoder)
     - [decoder.decode(tokens)](#decoderdecodetokens)
 4. Vocabulary Information
+    - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
-    - [vocab.capcode()](#vocabcapcode)
     - [vocab.charset()](#vocabcharset)
+    - [vocab.normalization()](#vocabnormalization)
+    - [vocab.capcode()](#vocabcapcode)
+    - [vocab.mode()](#vocabmode)
     - [vocab.unk_token_id()](#vocabunk_token_id)
     - [vocab.convert_ids_to_tokens(ids)](#vocabconvert_ids_to_tokensids)
     - [vocab.convert_ids_to_tokens_decoded(ids)](#vocabconvert_ids_to_tokens_decodedids)
     - [vocab.id_to_token(id)](#vocabid_to_tokenid)
     - [vocab.id_to_token_decoded(id)](#vocabid_to_token_decodedid)
     - [vocab.token_to_id(token)](#vocabtoken_to_idtoken)
     - [vocab.convert_tokens_to_ids(tokens)](#vocabconvert_tokens_to_idstokens)
 5. Vocabulary Modification
-    - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone)
+    - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone-reset_token_idsfalse)
     - [vocab.add_token(token)](#vocabadd_tokentoken)
     - [vocab.delete_token(token)](#vocabdelete_tokentoken)
+    - [vocab.delete_token_by_id(id)](#vocabdelete_token_by_idid)
     - [vocab.add_special_token(token)](#vocabadd_special_tokentoken)
-    - [vocab.resize(size)](#vocabresizesize)
+    - [vocab.resize(size)](#vocabresizesize-reset_token_idsfalse)
+    - [vocab.reset_token_ids()](#vocabreset_token_ids)
     - [vocab.enable_unk_token()](#vocabenable_unk_token)
     - [vocab.disable_unk_token()](#vocabdisable_unk_token)
-6. TokenMonster Class Methods
-    - [TokenMonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
-    - [TokenMonster.deserialize_tokens(binary_string)](#tokenmonsterdeserialize_tokensbinary_string)
-    - [TokenMonster.serialize_tokens(integer_list)](#tokenmonsterserialize_tokensinteger_list)
-    - [TokenMonster.disconnect()](#tokenmonsterdisconnect)
+6. Other
+    - [tokenmonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
+    - [tokenmonster.disconnect()](#tokenmonsterdisconnect)
+    - [vocab.serialize_tokens(integer_list)](#vocabserialize_tokensinteger_list)
+    - [vocab.deserialize_tokens(binary_string)](#vocabdeserialize_tokensbinary_string)
 
 ## Usage
 
-The main class is `TokenMonster`, which is initialized with a vocabulary from a file, URL or prebuilt vocabulary name.
-
 ```python
-vocab = TokenMonster("english-32000-balanced-v1")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 tokens = vocab.tokenize(str)
 decoded_string = vocab.decode(tokens)
 ```
 
 ## TokenMonster Methods
 
-### TokenMonster.\_\_init\_\_(path)
+### tokenmonster.load(path)
 
-Initialize the TokenMonster object with a vocabulary file or URL.
+Loads a TokenMonster vocabulary from file, URL or by name.
 
 #### Parameters
 
-- `path` (string): The path to the vocabulary file or URL.
+- `path` (string): A filepath, URL or pre-built vocabulary name.
+
+#### Returns
+
+- `Vocab`: An instance of tokenmonster.Vocab.
 
 #### Usage
 
 ```python
-vocab = TokenMonster("filename")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 ```
 
-### TokenMonster.\_\_len\_\_()
+### tokenmonster.new(yaml)
 
-Get the size of the vocabulary.
+Creates a new vocabulary from a YAML string.
+A sample YAML file can be found here: https://github.com/alasdairforsythe/tokenmonster/yaml_guide
+You should save it in the vocab format with `vocab.save()` for future use.
+
+#### Parameters
+
+- `yaml` (string or bytes string): The YAML file.
 
 #### Returns
 
-- `int`: The size of the vocabulary.
+- `Vocab`: An instance of tokenmonster.Vocab class.
 
 #### Usage
 
 ```python
-vocab = TokenMonster("filename")
-number_of_tokens = len(vocab)
+vocab = tokenmonster.new(yaml_string)
+vocab.save(filename)
 ```
 
 ### vocab.save(fname)
 
 Saves the current vocabulary to a file.
 
 The working directory is not the Python working directory but the TokenMonster default directory.
@@ -104,14 +118,34 @@
 
 #### Usage
 
 ```python
 vocab.save("test.vocab")
 ```
 
+### vocab.export_yaml(order_by_score=False)
+
+Exports the vocabulary as a YAML file, which is returned as a bytes string.
+
+#### Parameters
+
+- `order_by_score` (boolean): If true the tokens are order by score instead of alphabetically.
+
+#### Returns
+
+- `YAML` (bytes string): The vocabulary in YAML format.
+
+#### Usage
+
+```python
+yaml = vocab.export_yaml()
+with open(file_path, 'wb') as file:
+  file.write(yaml)
+```
+
 ## Tokenization & Detokenization
 
 ### vocab.tokenize(text)
 
 Tokenizes a string into tokens according to the vocabulary.
 
 You can pass a string or a list of strings. If you pass a list of strings they are tokenized
@@ -157,62 +191,103 @@
 
 ### vocab.decoder()
 
 Returns a new decoder instance used for decoding tokens into text.
 
 #### Returns
 
-- `TokenMonster.DecoderInstance`: A new decoder instance.
+- `tokenmonster.DecoderInstance`: A new decoder instance.
 
 #### Usage
 
 ```python
 decoder = vocab.decoder()
 ```
 
 ## Vocabulary Information
 
+### len(vocab)
+
+Get the size of the vocabulary.
+
+#### Returns
+
+- `int`: The size of the vocabulary.
+
+#### Usage
+
+```python
+vocab = tokenmonster.load("filename")
+number_of_tokens = len(vocab)
+```
+
 ### vocab.get_dictionary()
 
 Returns a dictionary of all tokens in the vocabulary.
 
-This returns a list where the index of the list is the token ID and the content of each is
-"token", "token_decoded", "type" and "score". Note that you should not attempt to use this to
-interpret tokenized sequences because the capcode encoded tokens can change the way the next
-tokens are decoded. Therefore you should always use one of the two "decode" methods.
+This returns a list of dictionaries with keys "id", "token", "token_decoded", "type" and "score".
+Note that you should not attempt to use this to interpret tokenized sequences because the capcode
+encoded tokens can change the way the next tokens are decoded. Therefore you should always use
+one of the two "decode" methods.
 
 #### Returns
 
 - `list`: A list of dictionaries where the index is the token ID and each is a dictionary with the following keys:
+  - `id` (int): The ID of the token.
   - `token` (string): The token including capcode encoding.
   - `token_decoded` (string): The same token decoded from its capcode form.
   - `type` (int): The type of token (0 = regular, 1 = byte, 2 = special, 3 = UNK).
   - `score` (float): The token's representation in the dataset used to train the vocabulary.
 
 #### Usage
 
 ```python
 tokens = vocab.get_dictionary()
 ```
 
+### vocab.charset()
+
+Returns the character set used by the vocabulary.
+
+#### Returns
+
+- `string`: The character set used by the vocabulary. Possible values are "UTF-8", "UTF-16", "None".
+
+### vocab.normalization()
+
+Returns the normalization of the vocabulary.
+
+#### Returns
+
+- `string`: The normalization of the vocabulary. Possible values are "NFD", "None".
+
 ### vocab.capcode()
 
-Returns true if the vocabulary has capcode enabled.
+Returns the capcode level of the vocabulary.
+- 0 = disabled
+- 1 = only deleteToken
+- 2 = enabled
 
 #### Returns
 
-- `bool`: True if capcode is enabled, False otherwise.
+- `int`: The capcode level (0-2).
 
-### vocab.charset()
+### vocab.mode()
 
-Returns the character set used by the vocabulary.
+Returns the optimization mode of the vocabulary.
+- 0 = unfiltered
+- 1 = clean
+- 2 = balanced
+- 3 = consistent
+- 4 = strict
+- 5 = (vocabulary was not trained with TokenMonster)
 
 #### Returns
 
-- `string`: The character set used by the vocabulary. Possible values are "UTF-8", "UTF-16", or "None".
+- `int`: The optimization mode (0-5).
 
 ### vocab.unk_token_id()
 
 Returns the ID of the UNK token, or 'None' type if there is no UNK token.
 
 #### Returns
 
@@ -292,38 +367,39 @@
 
 #### Returns
 
 - `list of ints`: The token IDs corresponding to the input tokens. None type for any tokens that are not in the vocabulary.
 
 ## Vocabulary Modification
 
-### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)
+### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None, reset_token_ids=False)
 
-Modifies the vocabulary. Doing so produces a new vocabulary with entirely different
-ID for each token, including special tokens. It therefore invalidates all decoder
-objects associated with the model before modification.
+Modifies the vocabulary. Doing so invalidates all decoder objects associated with the
+model before modification.
 
 Notes:
 - Special tokens are special in that they cannot be skipped. All regular tokens
   that contain specials tokens within them are deleted.
 - When resizing the vocabulary down, the worst performing tokens are deleted
-  ensuring the vocabulary remains efficient.
+  ensuring the vocabulary remains efficient. However, only regular tokens
+  with a score > 0 are can be removed by resizing.
 - A vocabulary can also be resized up. If any tokens have been removed by deleting
   or resizing, they can be restored by resizing the vocabulary to be larger.
 - After modifying you will need to "save" the vocabulary to a file or it'll be
   lost when the script ends.
 - delete_tokens can be in either raw or decoded form.
 
 #### Parameters
 
 - `add_special_tokens` (string or list of strings): Special tokens to add to the vocabulary.
 - `add_regular_tokens` (string or list of strings): Regular tokens to add to the vocabulary.
 - `delete_tokens` (string or list of strings): Regular or Special tokens to delete.
 - `resize` (int): Resizes the vocabulary to this size.
-- `change_unk` (Boolean): If set, it enables or disables the UNK token.
+- `change_unk` (boolean): If set, it enables or disables the UNK token.
+- `reset_token_ids` (boolean): If true the IDs are all reset starting from zero.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 #### Usage
 
@@ -332,82 +408,104 @@
 vocab.modify("<eos>")
 # adds the special token <eos> and keep the vocabulary at the current size
 vocab.modify("<eos>", None, None, len(vocab))
 ```
 
 ### vocab.add_token(token)
 
-Add one or more regular tokens. This also changes the token IDs. See "modify".
+Add one or more regular tokens.
 
 #### Parameters
 
 - `token` (string or list of strings): The regular tokens to add.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 ### vocab.delete_token(token)
 
-Delete one or more regular or special tokens. This also changes the token IDs. See "modify".
+Delete one or more regular or special tokens.
 You can give the token in either its encoded or decoded form.
 
 #### Parameters
 
 - `token` (string or list of strings): The tokens to delete.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
+### vocab.delete_token_by_id(id)
+
+Delete one or more regular or special token by specifying the token ID.
+
+#### Parameters
+
+- `id` (int or list of ints): The IDs of the tokens to delete.
+
+#### Returns
+
+- `int`: The new size of the vocabulary.
+
 ### vocab.add_special_token(token)
 
-Add one or more special tokens. This also changes the token IDs. See "modify".
+Add one or more special tokens.
 
 #### Parameters
 
 - `token` (string or list of strings): The special tokens to add.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
-### vocab.resize(size)
+### vocab.resize(size, reset_token_ids=False)
 
-Changes the size of the vocabulary. This also changes the token IDs. See "modify".
+Changes the size of the vocabulary and optionally resets the token IDs.
 
 A vocabulary can be enlarged as well reduced in size. Only the worst performing
 tokens are removed when reducing.
 
+Resizing only removes regular tokens that are not single byte token and have
+score > 0. If there are not enough of these, the new size may not match
+the target size.
+
 #### Parameters
 
 - `size` (int): The new size of the vocabulary.
+- `reset_token_ids` (boolean): If true, the IDs of all tokens are reset from zero.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
+### vocab.reset_token_ids()
+
+Resets the token IDs to be sequential beginning from zero.
+
+If tokens have been deleted from the vocabulary there will be gaps in the token IDs.
+Resetting the token IDs removes these gaps but all tokens will have new IDs.
+
 ### vocab.enable_unk_token()
 
 Enables the UNK token.
 
-The UNK token can be added or removed without affecting the rest of the vocabulary.
 If enabled, the UNK token appears whenever there is a character that is not in the vocabulary.
-Notethat the UNK token will not be enabled if all possible characters have tokens.
-Use get_unk_token to retrieve the ID for the UNK token.
+Note that the UNK token will not be enabled if all possible characters have tokens.
+Use `vocab.unk_token_id()` to retrieve the ID for the UNK token.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 ### vocab.disable_unk_token()
 
 Disables the UNK token.
 
-The UNK token can be added or removed without affecting the rest of the vocabulary.
 Without an UNK token, any character for which there is no token is ignored during tokenization.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 ## TokenMonster.DecoderInstance
@@ -415,15 +513,15 @@
 A nested class for decoding streams of tokens in sequence.
 
 This class takes tokens and decodes them to generate human-readable strings.
 
 ## Usage
 
 ```python
-vocab = TokenMonster("english-32000-balanced-v1")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ### decoder.decode(tokens)
 
@@ -442,60 +540,67 @@
 #### Returns
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
 ```python
-vocab = TokenMonster("english-32000-balanced-v1")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 decoder = vocab.Decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
-## TokenMonster Class Methods
+## Other
 
-### TokenMonster.set_local_directory(dir=None)
+### tokenmonster.set_local_directory(dir=None)
 
 Sets the local directory for TokenMonster.
 
 If no directory is specified, the default directory is ~/\_tokenmonster
 
 #### Parameters
 
 - `dir` (string): The local directory to use.
 
-### TokenMonster.deserialize_tokens(binary_string)
+#### Usage
 
-Deserializes a binary string back into a list of ints (tokens).
-The encoding_length needs to be recorded separately.
+```python
+tokenmonster.set_local_directory("/path/to/preferred")
+```
 
-#### Parameters
+### tokenmonster.disconnect()
 
-- `binary_string` (bytes): The binary string to deserialize.
+Disconnects and closes tokenmonsterserver.
 
 #### Returns
 
-- `list of ints`: The deserialized tokens.
+- `None`
 
-### TokenMonster.serialize_tokens(integer_list)
+### vocab.serialize_tokens(integer_list)
 
 Serializes tokens from a list of ints into a binary string.
-The encoding_length needs to be recorded separately.
+The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
 - `integer_list` (list of ints): The tokens to serialize.
 
 #### Returns
 
 - `bytes`: The serialized binary string.
 
-### TokenMonster.disconnect()
+### vocab.deserialize_tokens(binary_string)
 
-Disconnects and closes tokenmonsterserver.
+Deserializes a binary string back into a list of ints (tokens).
+The `encoding_length` used is from vocab.encoding_length.
+
+#### Parameters
+
+- `binary_string` (bytes): The binary string to deserialize.
 
 #### Returns
 
-- `None`
+- `list of ints`: The deserialized tokens.
 .
 
+
```

### Comparing `tokenmonster-1.0.1/setup.py` & `tokenmonster-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.0.1',
+    version='1.1.0',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.0.1/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.0/tokenmonster.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,108 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # TokenMonster
 
 1. [Usage](#usage)
-2. TokenMonster Methods
-    - [TokenMonster.\_\_init\_\_(path)](#tokenmonster__init__path)
-    - [TokenMonster.\_\_len\_\_()](#tokenmonster__len__)
-	- [vocab.save(fname)](#vocabsavefname)
+2. Loading & Exporting
+    - [tokenmonster.load(path)](#tokenmonsterloadpath)
+    - [tokenmonster.new(yaml)](#tokenmonsternewyaml)
+    - [vocab.save(fname)](#vocabsavefname)
+    - [vocab.export_yaml(order_by_score=False)](#vocabexport_yamlorder_by_scorefalse)
 3. Tokenization & Detokenization
-	- [vocab.tokenize(text)](#vocabtokenizetext)
-	- [vocab.decode(tokens)](#vocabdecodetokens)
+    - [vocab.tokenize(text)](#vocabtokenizetext)
+    - [vocab.decode(tokens)](#vocabdecodetokens)
     - [vocab.decoder()](#vocabdecoder)
     - [decoder.decode(tokens)](#decoderdecodetokens)
 4. Vocabulary Information
+    - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
-    - [vocab.capcode()](#vocabcapcode)
     - [vocab.charset()](#vocabcharset)
+    - [vocab.normalization()](#vocabnormalization)
+    - [vocab.capcode()](#vocabcapcode)
+    - [vocab.mode()](#vocabmode)
     - [vocab.unk_token_id()](#vocabunk_token_id)
     - [vocab.convert_ids_to_tokens(ids)](#vocabconvert_ids_to_tokensids)
     - [vocab.convert_ids_to_tokens_decoded(ids)](#vocabconvert_ids_to_tokens_decodedids)
     - [vocab.id_to_token(id)](#vocabid_to_tokenid)
     - [vocab.id_to_token_decoded(id)](#vocabid_to_token_decodedid)
     - [vocab.token_to_id(token)](#vocabtoken_to_idtoken)
     - [vocab.convert_tokens_to_ids(tokens)](#vocabconvert_tokens_to_idstokens)
 5. Vocabulary Modification
-    - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone)
+    - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone-reset_token_idsfalse)
     - [vocab.add_token(token)](#vocabadd_tokentoken)
     - [vocab.delete_token(token)](#vocabdelete_tokentoken)
+    - [vocab.delete_token_by_id(id)](#vocabdelete_token_by_idid)
     - [vocab.add_special_token(token)](#vocabadd_special_tokentoken)
-    - [vocab.resize(size)](#vocabresizesize)
+    - [vocab.resize(size)](#vocabresizesize-reset_token_idsfalse)
+    - [vocab.reset_token_ids()](#vocabreset_token_ids)
     - [vocab.enable_unk_token()](#vocabenable_unk_token)
     - [vocab.disable_unk_token()](#vocabdisable_unk_token)
-6. TokenMonster Class Methods
-    - [TokenMonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
-    - [TokenMonster.deserialize_tokens(binary_string)](#tokenmonsterdeserialize_tokensbinary_string)
-    - [TokenMonster.serialize_tokens(integer_list)](#tokenmonsterserialize_tokensinteger_list)
-    - [TokenMonster.disconnect()](#tokenmonsterdisconnect)
+6. Other
+    - [tokenmonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
+    - [tokenmonster.disconnect()](#tokenmonsterdisconnect)
+    - [vocab.serialize_tokens(integer_list)](#vocabserialize_tokensinteger_list)
+    - [vocab.deserialize_tokens(binary_string)](#vocabdeserialize_tokensbinary_string)
 
 ## Usage
 
-The main class is `TokenMonster`, which is initialized with a vocabulary from a file, URL or prebuilt vocabulary name.
-
 ```python
-vocab = TokenMonster("english-32000-balanced-v1")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 tokens = vocab.tokenize(str)
 decoded_string = vocab.decode(tokens)
 ```
 
 ## TokenMonster Methods
 
-### TokenMonster.\_\_init\_\_(path)
+### tokenmonster.load(path)
 
-Initialize the TokenMonster object with a vocabulary file or URL.
+Loads a TokenMonster vocabulary from file, URL or by name.
 
 #### Parameters
 
-- `path` (string): The path to the vocabulary file or URL.
+- `path` (string): A filepath, URL or pre-built vocabulary name.
+
+#### Returns
+
+- `Vocab`: An instance of tokenmonster.Vocab.
 
 #### Usage
 
 ```python
-vocab = TokenMonster("filename")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 ```
 
-### TokenMonster.\_\_len\_\_()
+### tokenmonster.new(yaml)
 
-Get the size of the vocabulary.
+Creates a new vocabulary from a YAML string.
+A sample YAML file can be found here: https://github.com/alasdairforsythe/tokenmonster/yaml_guide
+You should save it in the vocab format with `vocab.save()` for future use.
+
+#### Parameters
+
+- `yaml` (string or bytes string): The YAML file.
 
 #### Returns
 
-- `int`: The size of the vocabulary.
+- `Vocab`: An instance of tokenmonster.Vocab class.
 
 #### Usage
 
 ```python
-vocab = TokenMonster("filename")
-number_of_tokens = len(vocab)
+vocab = tokenmonster.new(yaml_string)
+vocab.save(filename)
 ```
 
 ### vocab.save(fname)
 
 Saves the current vocabulary to a file.
 
 The working directory is not the Python working directory but the TokenMonster default directory.
@@ -104,14 +118,34 @@
 
 #### Usage
 
 ```python
 vocab.save("test.vocab")
 ```
 
+### vocab.export_yaml(order_by_score=False)
+
+Exports the vocabulary as a YAML file, which is returned as a bytes string.
+
+#### Parameters
+
+- `order_by_score` (boolean): If true the tokens are order by score instead of alphabetically.
+
+#### Returns
+
+- `YAML` (bytes string): The vocabulary in YAML format.
+
+#### Usage
+
+```python
+yaml = vocab.export_yaml()
+with open(file_path, 'wb') as file:
+  file.write(yaml)
+```
+
 ## Tokenization & Detokenization
 
 ### vocab.tokenize(text)
 
 Tokenizes a string into tokens according to the vocabulary.
 
 You can pass a string or a list of strings. If you pass a list of strings they are tokenized
@@ -157,62 +191,103 @@
 
 ### vocab.decoder()
 
 Returns a new decoder instance used for decoding tokens into text.
 
 #### Returns
 
-- `TokenMonster.DecoderInstance`: A new decoder instance.
+- `tokenmonster.DecoderInstance`: A new decoder instance.
 
 #### Usage
 
 ```python
 decoder = vocab.decoder()
 ```
 
 ## Vocabulary Information
 
+### len(vocab)
+
+Get the size of the vocabulary.
+
+#### Returns
+
+- `int`: The size of the vocabulary.
+
+#### Usage
+
+```python
+vocab = tokenmonster.load("filename")
+number_of_tokens = len(vocab)
+```
+
 ### vocab.get_dictionary()
 
 Returns a dictionary of all tokens in the vocabulary.
 
-This returns a list where the index of the list is the token ID and the content of each is
-"token", "token_decoded", "type" and "score". Note that you should not attempt to use this to
-interpret tokenized sequences because the capcode encoded tokens can change the way the next
-tokens are decoded. Therefore you should always use one of the two "decode" methods.
+This returns a list of dictionaries with keys "id", "token", "token_decoded", "type" and "score".
+Note that you should not attempt to use this to interpret tokenized sequences because the capcode
+encoded tokens can change the way the next tokens are decoded. Therefore you should always use
+one of the two "decode" methods.
 
 #### Returns
 
 - `list`: A list of dictionaries where the index is the token ID and each is a dictionary with the following keys:
+  - `id` (int): The ID of the token.
   - `token` (string): The token including capcode encoding.
   - `token_decoded` (string): The same token decoded from its capcode form.
   - `type` (int): The type of token (0 = regular, 1 = byte, 2 = special, 3 = UNK).
   - `score` (float): The token's representation in the dataset used to train the vocabulary.
 
 #### Usage
 
 ```python
 tokens = vocab.get_dictionary()
 ```
 
+### vocab.charset()
+
+Returns the character set used by the vocabulary.
+
+#### Returns
+
+- `string`: The character set used by the vocabulary. Possible values are "UTF-8", "UTF-16", "None".
+
+### vocab.normalization()
+
+Returns the normalization of the vocabulary.
+
+#### Returns
+
+- `string`: The normalization of the vocabulary. Possible values are "NFD", "None".
+
 ### vocab.capcode()
 
-Returns true if the vocabulary has capcode enabled.
+Returns the capcode level of the vocabulary.
+- 0 = disabled
+- 1 = only deleteToken
+- 2 = enabled
 
 #### Returns
 
-- `bool`: True if capcode is enabled, False otherwise.
+- `int`: The capcode level (0-2).
 
-### vocab.charset()
+### vocab.mode()
 
-Returns the character set used by the vocabulary.
+Returns the optimization mode of the vocabulary.
+- 0 = unfiltered
+- 1 = clean
+- 2 = balanced
+- 3 = consistent
+- 4 = strict
+- 5 = (vocabulary was not trained with TokenMonster)
 
 #### Returns
 
-- `string`: The character set used by the vocabulary. Possible values are "UTF-8", "UTF-16", or "None".
+- `int`: The optimization mode (0-5).
 
 ### vocab.unk_token_id()
 
 Returns the ID of the UNK token, or 'None' type if there is no UNK token.
 
 #### Returns
 
@@ -292,38 +367,39 @@
 
 #### Returns
 
 - `list of ints`: The token IDs corresponding to the input tokens. None type for any tokens that are not in the vocabulary.
 
 ## Vocabulary Modification
 
-### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)
+### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None, reset_token_ids=False)
 
-Modifies the vocabulary. Doing so produces a new vocabulary with entirely different
-ID for each token, including special tokens. It therefore invalidates all decoder
-objects associated with the model before modification.
+Modifies the vocabulary. Doing so invalidates all decoder objects associated with the
+model before modification.
 
 Notes:
 - Special tokens are special in that they cannot be skipped. All regular tokens
   that contain specials tokens within them are deleted.
 - When resizing the vocabulary down, the worst performing tokens are deleted
-  ensuring the vocabulary remains efficient.
+  ensuring the vocabulary remains efficient. However, only regular tokens
+  with a score > 0 are can be removed by resizing.
 - A vocabulary can also be resized up. If any tokens have been removed by deleting
   or resizing, they can be restored by resizing the vocabulary to be larger.
 - After modifying you will need to "save" the vocabulary to a file or it'll be
   lost when the script ends.
 - delete_tokens can be in either raw or decoded form.
 
 #### Parameters
 
 - `add_special_tokens` (string or list of strings): Special tokens to add to the vocabulary.
 - `add_regular_tokens` (string or list of strings): Regular tokens to add to the vocabulary.
 - `delete_tokens` (string or list of strings): Regular or Special tokens to delete.
 - `resize` (int): Resizes the vocabulary to this size.
-- `change_unk` (Boolean): If set, it enables or disables the UNK token.
+- `change_unk` (boolean): If set, it enables or disables the UNK token.
+- `reset_token_ids` (boolean): If true the IDs are all reset starting from zero.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 #### Usage
 
@@ -332,82 +408,104 @@
 vocab.modify("<eos>")
 # adds the special token <eos> and keep the vocabulary at the current size
 vocab.modify("<eos>", None, None, len(vocab))
 ```
 
 ### vocab.add_token(token)
 
-Add one or more regular tokens. This also changes the token IDs. See "modify".
+Add one or more regular tokens.
 
 #### Parameters
 
 - `token` (string or list of strings): The regular tokens to add.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 ### vocab.delete_token(token)
 
-Delete one or more regular or special tokens. This also changes the token IDs. See "modify".
+Delete one or more regular or special tokens.
 You can give the token in either its encoded or decoded form.
 
 #### Parameters
 
 - `token` (string or list of strings): The tokens to delete.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
+### vocab.delete_token_by_id(id)
+
+Delete one or more regular or special token by specifying the token ID.
+
+#### Parameters
+
+- `id` (int or list of ints): The IDs of the tokens to delete.
+
+#### Returns
+
+- `int`: The new size of the vocabulary.
+
 ### vocab.add_special_token(token)
 
-Add one or more special tokens. This also changes the token IDs. See "modify".
+Add one or more special tokens.
 
 #### Parameters
 
 - `token` (string or list of strings): The special tokens to add.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
-### vocab.resize(size)
+### vocab.resize(size, reset_token_ids=False)
 
-Changes the size of the vocabulary. This also changes the token IDs. See "modify".
+Changes the size of the vocabulary and optionally resets the token IDs.
 
 A vocabulary can be enlarged as well reduced in size. Only the worst performing
 tokens are removed when reducing.
 
+Resizing only removes regular tokens that are not single byte token and have
+score > 0. If there are not enough of these, the new size may not match
+the target size.
+
 #### Parameters
 
 - `size` (int): The new size of the vocabulary.
+- `reset_token_ids` (boolean): If true, the IDs of all tokens are reset from zero.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
+### vocab.reset_token_ids()
+
+Resets the token IDs to be sequential beginning from zero.
+
+If tokens have been deleted from the vocabulary there will be gaps in the token IDs.
+Resetting the token IDs removes these gaps but all tokens will have new IDs.
+
 ### vocab.enable_unk_token()
 
 Enables the UNK token.
 
-The UNK token can be added or removed without affecting the rest of the vocabulary.
 If enabled, the UNK token appears whenever there is a character that is not in the vocabulary.
-Notethat the UNK token will not be enabled if all possible characters have tokens.
-Use get_unk_token to retrieve the ID for the UNK token.
+Note that the UNK token will not be enabled if all possible characters have tokens.
+Use `vocab.unk_token_id()` to retrieve the ID for the UNK token.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 ### vocab.disable_unk_token()
 
 Disables the UNK token.
 
-The UNK token can be added or removed without affecting the rest of the vocabulary.
 Without an UNK token, any character for which there is no token is ignored during tokenization.
 
 #### Returns
 
 - `int`: The new size of the vocabulary.
 
 ## TokenMonster.DecoderInstance
@@ -415,15 +513,15 @@
 A nested class for decoding streams of tokens in sequence.
 
 This class takes tokens and decodes them to generate human-readable strings.
 
 ## Usage
 
 ```python
-vocab = TokenMonster("english-32000-balanced-v1")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ### decoder.decode(tokens)
 
@@ -442,60 +540,67 @@
 #### Returns
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
 ```python
-vocab = TokenMonster("english-32000-balanced-v1")
+vocab = tokenmonster.load("english-32000-balanced-v1")
 decoder = vocab.Decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
-## TokenMonster Class Methods
+## Other
 
-### TokenMonster.set_local_directory(dir=None)
+### tokenmonster.set_local_directory(dir=None)
 
 Sets the local directory for TokenMonster.
 
 If no directory is specified, the default directory is ~/\_tokenmonster
 
 #### Parameters
 
 - `dir` (string): The local directory to use.
 
-### TokenMonster.deserialize_tokens(binary_string)
+#### Usage
 
-Deserializes a binary string back into a list of ints (tokens).
-The encoding_length needs to be recorded separately.
+```python
+tokenmonster.set_local_directory("/path/to/preferred")
+```
 
-#### Parameters
+### tokenmonster.disconnect()
 
-- `binary_string` (bytes): The binary string to deserialize.
+Disconnects and closes tokenmonsterserver.
 
 #### Returns
 
-- `list of ints`: The deserialized tokens.
+- `None`
 
-### TokenMonster.serialize_tokens(integer_list)
+### vocab.serialize_tokens(integer_list)
 
 Serializes tokens from a list of ints into a binary string.
-The encoding_length needs to be recorded separately.
+The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
 - `integer_list` (list of ints): The tokens to serialize.
 
 #### Returns
 
 - `bytes`: The serialized binary string.
 
-### TokenMonster.disconnect()
+### vocab.deserialize_tokens(binary_string)
 
-Disconnects and closes tokenmonsterserver.
+Deserializes a binary string back into a list of ints (tokens).
+The `encoding_length` used is from vocab.encoding_length.
+
+#### Parameters
+
+- `binary_string` (bytes): The binary string to deserialize.
 
 #### Returns
 
-- `None`
+- `list of ints`: The deserialized tokens.
 .
 
+
```

### Comparing `tokenmonster-1.0.1/tokenmonster.py` & `tokenmonster-1.1.0/tokenmonster.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,43 +4,119 @@
 import urllib.request
 import platform
 import sys
 from collections.abc import Iterable
 if platform.system() == 'Windows':
     import getpass
 
-class TokenMonster:
+def set_local_directory(path):
     """
-    Main class for token manipulation.
+    The default directory for TokenMonster is ~/_tokenmonster
+    Use this function to set the default directory elsewhere, before loading any vocabularies.
+    """
+    Vocab._set_local_directory(path)
+
+def disconnect():
+    """
+    Closes tokenmonsterserver subprocess.
+    """
+    Vocab._disconnect()
+
+def load(path):
+    """
+    Loads a TokenMonster vocabulary from file, URL or by name.
+
+    Parameters:
+        path (string): A filepath, URL or pre-built vocabulary name.
+
+    Returns:
+        Vocab: An instance of tokenmonster.Vocab.
+
+    Usage:
+        vocab = tokenmonster.load("english-32000-balanced-v1")
+        tokens = vocab.tokenize(str)
+        decoded_string = vocab.decode(tokens)
+    """
+    return Vocab(path)
+
+def new(yaml):
+    """
+    Creates a new vocabulary from a YAML string.
+    A sample YAML file can be found here: https://github.com/alasdairforsythe/tokenmonster/yaml_guide
+    You should save it in the vocab format with `vocab.save()` for future use.
+
+    Parameters:
+        yaml (string or bytes string): The YAML file.
+
+    Returns:
+        TokenMonster instance: An vocabulary instance of TokenMonster class.
+
+    Usage:
+        vocab = tokenmonster.new(yaml_string)
+        vocab.save(filename)
+    """
+    if not isinstance(yaml, bytes):
+        if isinstance(yaml, str):
+            yaml = yaml.encode('utf-8')
+        else:
+            raise ValueError("TokenMonster: Input to `tokenmonster.New()` must be a YAML string.")
+    Vocab._set_local_directory()
+    job_type = 18
+    response = Vocab._communicate(job_type, 0, len(yaml), yaml)
+    vocab = Vocab.__new__(Vocab)
+    vocab._capcode = response[0]
+    vocab._charset = response[1]
+    vocab._normalization = response[2]
+    vocab._mode = response[3]
+    vocab.vocab_size = _read_uint32(response[4:8])
+    vocab.id = _read_uint32(response[8:12])
+    unk = _read_uint32(response[12:16])
+    if unk == 16777215:
+        vocab.unk = None
+    else:
+         vocab.unk = unk
+    if vocab.vocab_size > 65536:
+        vocab.encoding_length = 4
+    else:
+        vocab.encoding_length = 2
+    vocab.fname = None
+    vocab.dictionary = None
+    vocab.token_to_id = None
+    vocab._modified_id = 0
+    vocab._decoders = []
+    return vocab
 
-    This class is initialized with a vocabulary from a file or URL.
+class Vocab:
+    """
+    Main class for TokenMonster.
 
     Usage:
-        vocab = TokenMonster("english-32000-balanced-v1")
+        vocab = tokenmonster.Load("english-32000-balanced-v1")
         tokens = vocab.tokenize(str)
         decoded_string = vocab.decode(tokens)
     """
 
     class DecoderInstance:
         """
         A nested class for decoding streams of tokens in sequence.
 
         This class takes tokens and decodes them to generate human-readable strings.
 
         Usage:
-            vocab = TokenMonster("english-32000-balanced-v1")
+            vocab = tokenmonster.Load("english-32000-balanced-v1")
             decoder = vocab.decoder()
             decoded_string = decoder.decode(tokens)
             decoded_string += decoder.decode(more_tokens)
         """
 
         def __init__(self, parent):
             self.parent = parent
-            self.id = TokenMonster._communicate(5, parent.id, 0)
+            self.id = Vocab._communicate(5, parent.id, 0)
             self._modified_id = parent._modified_id
+            parent._decoders.append(self.id)
         
         def decode(self, tokens):
             """
             A decoder object used for decoding token streams.
 
             This decoder object is used instead of the vocabulary decode method when you are
             decoding tokens in small segments, or one by one, that are part of a longer
@@ -51,106 +127,113 @@
             Parameters:
                 tokens (int or list of ints): A token ID or list of token IDs.
 
             Returns:
                 string: A human-readable string derived from the input tokens.
 
             Usage:
-                vocab = TokenMonster("english-32000-balanced-v1")
+                vocab = tokenmonster.Load("english-32000-balanced-v1")
                 decoder = vocab.Decoder()
                 decoded_string = decoder.decode(tokens)
                 decoded_string += decoder.decode(more_tokens)
             """
             if self.parent._modified_id != self._modified_id:
-                raise RuntimeError("Access denied to expired Decoder instance. The vocabulary was modified after Decoder instance was created.")
+                raise RuntimeError("Access denied to expired tokenmonster.Decoder instance.")
             if is_iterable(tokens):
                 if len(tokens) == 0:
                     return
             else:
                 if isinstance(tokens, int):
                     tokens = [tokens]
                 else:
                     raise ValueError("TokenMonster: Decoder decode accepts int or list of ints.")
             if is_iterable(tokens[0]):
                 raise ValueError("TokenMonster: You can't batch decode on a decoder object, use the vocab decoder for that.")
             payload = self.parent.serialize_tokens(tokens)
             job_type = self.parent.encoding_length + 5
-            response = TokenMonster._communicate(job_type, self.id, len(payload), payload)
+            response = Vocab._communicate(job_type, self.id, len(payload), payload)
             return self.parent._bytes_to_string(response)
         
         def _unload(self):
             if hasattr(self, 'id'):
                 if self.id is not None:
-                    TokenMonster._communicate(6, self.id, 0)
+                    if self.parent._modified_id != -1:
+                        Vocab._communicate(6, self.id, 0)
         
         def __del__(self):
             if not sys.is_finalizing():
                 self._unload()
 
     def __init__(self, path):
-        TokenMonster.set_local_directory()
+        Vocab._set_local_directory()
         if not any(char in path for char in "./\\"):
-            if TokenMonster._file_exists(path + ".vocab"):
-                path = os.path.join(TokenMonster._dir, path + ".vocab")
+            if Vocab._file_exists(path + ".vocab"):
+                path = os.path.join(Vocab._dir, path + ".vocab")
             else:
                 clean = path.replace("+", "")
-                if TokenMonster._file_exists(clean + ".vocab"):
-                    path = os.path.join(TokenMonster._dir, clean + ".vocab")
+                if Vocab._file_exists(clean + ".vocab"):
+                    path = os.path.join(Vocab._dir, clean + ".vocab")
                 else:
                     if _is_prebuilt(clean):
                         path = clean
-                        TokenMonster._download(_TOKENMONSTER_URL + "vocabs/" + path + ".vocab", path + ".vocab")
-                        if not TokenMonster._file_exists(path + ".vocab"):
+                        Vocab._download(_TOKENMONSTER_URL + "vocabs/" + path + ".vocab", path + ".vocab")
+                        if not Vocab._file_exists(path + ".vocab"):
                             raise RuntimeError("TokenMonster: Unable to download the prebuilt vocabulary, please check availability at huggingface.co/alasdairforsythe/tokenmonster")
         elif path.startswith("http://") or path.startswith("https://"):
             fname = os.path.basename(path)
-            if TokenMonster._file_exists(fname):
-                path = os.path.join(TokenMonster._dir, fname)
+            if Vocab._file_exists(fname):
+                path = os.path.join(Vocab._dir, fname)
             else:
-                TokenMonster._download(path, fname)
-                if TokenMonster._file_exists(fname):
-                    path = os.path.join(TokenMonster._dir, fname)
+                Vocab._download(path, fname)
+                if Vocab._file_exists(fname):
+                    path = os.path.join(Vocab._dir, fname)
                 else:
-                    raise FileNotFoundError("TokenMonster: Unable to download " + path + " to " + TokenMonster._dir)
+                    raise FileNotFoundError("TokenMonster: Unable to download " + path + " to " + Vocab._dir)
         elif os.path.isfile(path):
             pass
-        elif TokenMonster._file_exists(path + ".vocab"):
-            path = os.path.join(TokenMonster._dir, path + ".vocab")
-        elif TokenMonster._file_exists(path):
-            path = os.path.join(TokenMonster._dir, path)
+        elif Vocab._file_exists(path + ".vocab"):
+            path = os.path.join(Vocab._dir, path + ".vocab")
+        elif Vocab._file_exists(path):
+            path = os.path.join(Vocab._dir, path)
         else:
             raise FileNotFoundError("TokenMonster: Unable to locate " + path)
-
+        # Now read the vocabulary header
         with open(path, 'rb') as file:
-            vocab_header = file.read(9)
-        self.capcode = vocab_header[0] == 1
-        hasUnk = vocab_header[1] == 1
-        self.charset = vocab_header[2]
-        self.vocab_size = vocab_header[6] | (vocab_header[7] << 8) | (vocab_header[8] << 16)
-        self.unk = None
-        if hasUnk:
-            self.unk = self.vocab_size - 1
+            vocab_header = file.read(14)
+        self._capcode = vocab_header[0]
+        self._charset = vocab_header[1]
+        self._normalization = vocab_header[2]
+        self._mode = vocab_header[3]
+        unk = vocab_header[8] | (vocab_header[9] << 8) | (vocab_header[10] << 16)
+        self.vocab_size = vocab_header[11] | (vocab_header[12] << 8) | (vocab_header[13] << 16)
+        self.Unk = None
+        if unk != 16777215:
+            self.Unk = unk
         if self.vocab_size > 65536:
             self.encoding_length = 4
         else:
             self.encoding_length = 2
-        self.vocab = path
+        self.fname = path
         path_encoded = path.encode("utf-8")
         if len(path_encoded) > 255:
             raise RuntimeError("TokenMonster: Vocabulary filepath is too long, it must be less than 256 characters")
         payload = _write_uint8(len(path_encoded)) + path_encoded
-        self.id = TokenMonster._communicate(10, 0, len(payload), payload)
+        self.id = Vocab._communicate(10, 0, len(payload), payload)
         self.dictionary = None
         self.token_to_id = None
         self._modified_id = 0
+        self._decoders = []
 
     def _unload(self):
         if hasattr(self, 'id'):
             if self.id is not None:
-                TokenMonster._communicate(11, self.id, 0)
+                if self._modified_id != -1:
+                    for _, decoder_id in enumerate(self._decoders):
+                        Vocab._communicate(6, decoder_id, 0)
+                    Vocab._communicate(11, self.id, 0)
 
     def __del__(self):
         if not sys.is_finalizing():
             self._unload()
 
     def __len__(self):
         return self.vocab_size
@@ -159,28 +242,74 @@
         """
         Returns a new decoder instance used for decoding tokens into text.
         """
         return self.DecoderInstance(self)
     
     def capcode(self):
         """
-        Returns true if the vocabulary has capcode enabled.
+        Returns the capcode level of the vocabulary.
+        0 = disabled
+        1 = only deleteToken
+        2 = enabled
         """
-        return self.capcode
+        return self._capcode
     
     def charset(self):
         """
-        Returns one of "UTF-8", "UTF-16", or "None"
+        Returns one of "UTF-8", "UTF-16", "None"
         """
-        if self.charset == 1:
+        if self._charset == 1:
             return "UTF-8"
-        elif self.charset == 2:
+        elif self._charset == 2:
             return "UTF-16"
         return "None"
     
+    def mode(self):
+        """
+        Returns the optimization mode of the vocabulary.
+        """
+        if self._mode == 0:
+            return "unfiltered"
+        elif self._mode == 1:
+            return "clean"
+        elif self._mode == 2:
+            return "balanced"
+        elif self._mode == 3:
+            return "consistent"
+        elif self._mode == 4:
+            return "strict"
+        elif self._mode == 5:
+            return "n/a"
+    
+    def normalization(self):
+        """
+        Returns the normalization of the vocabulary, e.g. "NFD trim"
+        """
+        flag = self._normalization
+        s = ''
+        if flag == 0:
+            return 'None'
+        if flag & 1 != 0:
+            s = 'NFD '
+        if flag & 2 != 0:
+            s += 'Lowercase '
+        if flag & 4 != 0:
+            s += 'Accents '
+        if flag & 8 != 0:
+            s += 'Quotemarks '
+        if flag & 16 != 0:
+            s += 'Collapse '
+        if flag & 32 != 0:
+            s += 'Trim '
+        if flag & 64 != 0:
+            s += 'LeadingSpace '
+        if flag & 128 != 0:
+            s += 'NewLines '
+        return s.strip()
+    
     def decode(self, tokens):
         """
         Decodes tokens into a string.
 
         Only use this "decode" method if you are decoding a complete "batch" or complete "conversation".
         For decoding an incomplete batch sequentially (as the tokens become available) instead
         use the decoder object.
@@ -190,14 +319,16 @@
 
         Returns:
             string: The composed string from the input tokens.
 
         Usage:
             decoded_string = vocab.decode(tokens)
         """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         length = 4
         batch_size = 1
         payload = [b'']
         # Parse input
         if is_iterable(tokens):
             if len(tokens) == 0:
                 return
@@ -224,15 +355,15 @@
                 else:
                     raise ValueError("TokenMonster: Input to decode must be an int, a list of ints, or a list of list of ints.")
         else:
             raise ValueError("TokenMonster: Input to decode must be an int, a list of ints, or a list of list of ints.]")
         # Send
         job_type = self.encoding_length
         payload[0] = _write_uint32(batch_size)
-        response = TokenMonster._communicate(job_type, self.id, length, payload)
+        response = Vocab._communicate(job_type, self.id, length, payload)
         batches_reply = _read_uint32(response[0:4])
         if batches_reply != batch_size:
             raise RuntimeError("TokenMonster: batch size from response differs from request")
         decoded = [None] * batches_reply
         offset = 4
         for i in range(batch_size):
             batch_length = _read_uint64(response[offset:offset+8])
@@ -258,14 +389,16 @@
 
         Returns:
             tokens (int or list of int): The tokens to decode into a string
 
         Usage:
             tokens = vocab.tokenize(text)
         """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         length = 4
         batch_size = 1
         payload = [b'']
         single = False
         if isinstance(text, str):
             if len(text) == 0:
                 return
@@ -296,15 +429,15 @@
                 else:
                     raise ValueError("TokenMonster: Input to tokenize must be a string or a list of strings.")
         else:
             raise ValueError("TokenMonster: Input to tokenize must be a string or a list of strings.")
         # Send
         job_type = 1
         payload[0] = _write_uint32(batch_size)
-        response = TokenMonster._communicate(job_type, self.id, length, payload)
+        response = Vocab._communicate(job_type, self.id, length, payload)
         batches_reply = _read_uint32(response[0:4])
         if batches_reply != batch_size:
             raise RuntimeError("TokenMonster: batch size of response differs from request")
         tokens = [None] * batches_reply
         offset = 4
         for i in range(batch_size):
             batch_length = _read_uint64(response[offset:offset+8])
@@ -316,60 +449,63 @@
         else:
             return tokens
 
     def get_dictionary(self):
         """
         Returns a dictionary of all tokens in the vocabulary.
 
-        This returns a list where the index of the list is the token ID and the content of each is
-        "token", "token_decoded", "type" and "score". Note that you should not attempt to use this to
-        interpret tokenized sequences because the capcode encoded tokens can change the way the next
-        tokens are decoded. Therefore you should always use one of the two "decode" methods.
+        This returns a list of dictionaries with keys "id", "token", "token_decoded", "type" and "score".
+        Note that you should not attempt to use this to interpret tokenized sequences because the capcode
+        encoded tokens can change the way the next tokens are decoded. Therefore you should always use
+        one of the two "decode" methods.
 
         Parameters:
             string or list of strings: A string or bytes string, or list of strings or bytes strings.
 
         Returns:
-            list of dictionaries where the index is the token ID and each is a dictionary of:
+            list of dictionaries with keys are as follows:
+                id (int): the ID of the token
                 token (string): the token including capcode encoding
                 token_decoded (string): the same token decoded from it's capcode form
                 type (int): the type of token (0 = regular, 1 = byte, 2 = special, 3 = UNK)
                 score (float): token's representation in the dataset used to train the vocabulary
 
         Usage:
-            tokens = vocab.tokenize(text)
+            tokens = vocab.get_dictionary()
         """
         if self.dictionary is not None:
             return self.dictionary
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         job_type = 15
-        response = TokenMonster._communicate(job_type, self.id, 0)
+        response = Vocab._communicate(job_type, self.id, 0)
         size = _read_uint32(response[0:4])
         self.vocab_size = size # it should be already the same
         offset = 4
-        self.dictionary = []
+        self.dictionary = {}
         self.token_to_id = {}
+        self.unk = None
         types = ["regular", "single", "special", "unk"]
-        for i in range(size):
+        for _ in range(size):
+            id = _read_uint32(response[offset: offset + 4])
+            offset += 4
             len_token = response[offset]
             len_token_decoded = response[offset + 1]
             typ = response[offset + 2]
             score = _read_float32(response[offset + 3: offset + 7])
             offset += 7
             token = self._bytes_to_string(response[offset : offset + len_token])
             offset += len_token
             token_decoded = self._bytes_to_string(response[offset : offset + len_token_decoded])
             offset += len_token_decoded
-            self.dictionary.append({'token': token, 'token_decoded': token_decoded, 'type': types[typ], 'score': score})
-            if typ != 3:
-                self.token_to_id[token] = i
-                self.token_to_id[token_decoded] = i
-        if typ == 3:
-            self.unk = self.vocab_size - 1
-        else:
-            self.unk = None
+            self.dictionary[id] = {'id': id, 'token': token, 'token_decoded': token_decoded, 'type': types[typ], 'score': score}
+            self.token_to_id[token] = id
+            self.token_to_id[token_decoded] = id
+            if typ == 3:
+                self.unk = id
         return self.dictionary
     
     def convert_ids_to_tokens(self, ids):
         """
         Get the token string from any token ID, in it's capcode-encoded form.
 
         Parameters:
@@ -486,127 +622,200 @@
 
         Returns:
             int or None
         """
         if self.unk == False:
             self.get_dictionary()
         return self.unk
-        
 
-    def modify(self, add_special_tokens, add_regular_tokens = None, delete_tokens = None, resize = None, change_unk = None):
+    def modify(self, add_special_tokens, add_regular_tokens = None, delete_tokens = None, resize = None, change_unk = None, reset_token_ids = False):
         """
-        Modifies the vocabulary. Doing so produces a new vocabulary with entirely different
-        ID for each token, including special tokens. It therefore invalidates all decoder
-        objects associated with the model before modification.
+        Modifies the vocabulary. Doing so invalidates all decoder objects associated with the
+        model before modification.
 
         Notes:
             - Special tokens are special in that they cannot be skipped. All regular tokens
               that contain specials tokens within them are deleted.
             - When resizing the vocabulary down, the worst performing tokens are deleted
-              ensuring the vocabulary remains efficient.
+              ensuring the vocabulary remains efficient. However, only regular tokens
+              with a score > 0 are can be removed by resizing.
             - A vocabulary can also be resized up. If any tokens have been removed by deleting
               or resizing, they can be restored by resizing the vocabulary to be larger.
             - After modifying you will need to "save" the vocabulary to a file or it'll be
               lost when the script ends.
             - delete_tokens can be in either raw or decoded form.
 
         Parameters:
             add_special_tokens (string or list of strings): Special tokens to add to the vocabulary
             add_regular_tokens (string or list of strings): Regular tokens to add to the vocabulary
             delete_tokens (string or list of strings): Regular or Special tokens to delete
             resize (int): Resizes the vocabulary to this size
-            change_unk (Boolean): If set, it enables or disables the Unk token
+            change_unk (boolean): If set, it enables or disables the Unk token
+            reset_token_ids (boolean): If true the IDs are all reset starting from zero.
 
         Returns:
             int: The new size of the vocabulary.
 
         Usage:
             # adds the special token <eos>
             vocab.modify("<eos>")
             # adds the special token <eos> and keep the vocabulary at the current size
             vocab.modify("<eos>", None, None, len(vocab))
         """
         # Parse and format the inputs
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         add_special_tokens = self._format_list(add_special_tokens)
         add_regular_tokens = self._format_list(add_regular_tokens)
         delete_tokens = self._format_list(delete_tokens)
         if resize is None:
             resize = 0
         if change_unk == True:
             change_unk = 2
         elif change_unk == False:
             change_unk = 1
         else:
             change_unk = 0
         # Build request
-        payload = _write_uint8(change_unk) + _write_uint32(len(add_regular_tokens))
+        payload = _write_uint8(int(reset_token_ids)) + _write_uint8(change_unk) + _write_uint32(len(add_regular_tokens))
         for _, item in enumerate(add_regular_tokens):
             payload +=  _write_uint8(len(item)) + item
         payload += _write_uint32(len(delete_tokens))
         for _, item in enumerate(delete_tokens):
             payload += _write_uint8(len(item)) + item
         payload += _write_uint32(len(add_special_tokens))
         for _, item in enumerate(add_special_tokens):
             payload += _write_uint8(len(item)) + item
         payload += _write_uint32(resize)
         job_type = 14
-        self.vocab_size = TokenMonster._communicate(job_type, self.id, len(payload), payload)
-        self._modified_id += 1
-        self.dictionary = None
-        self.token_to_id = None
-        self.unk = False
-        if self.vocab_size > 65536:
-            self.encoding_length = 4
-        else:
-            self.encoding_length = 2
+        self.vocab_size = Vocab._communicate(job_type, self.id, len(payload), payload)
+        self._modified()
+        return self.vocab_size
+    
+    def modify_from_yaml(self, yaml):
+        """
+        Modifies the vocabulary using a YAML file.
+        A sample YAML file can be found here: https://github.com/alasdairforsythe/tokenmonster/yaml_guide
+
+        Parameters:
+            yaml (string or bytes string): The YAML file containing the modifications
+
+        Returns:
+            int: The new size of the vocabulary.
+
+        Usage:
+            # Example deletes 2 tokens, one with ID 127, and another token ' test'
+            vocab.modify_from_yaml("delete:\n  - id: 127\n  - token ' test'")
+
+        Returns:
+            int: The new size of the vocabulary.
+        """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
+        job_type = 17
+        self.vocab_size = Vocab._communicate(job_type, self.id, len(yaml), yaml)
+        self._modified()
         return self.vocab_size
 
     def add_token(self, token):
         """
-        Add one or more regular tokens. This also changes the token IDs. See "modify".
+        Add one or more regular tokens.
+
+        Returns:
+            int: The new size of the vocabulary.
         """
         return self.modify(None, token, None, 0)
 
     def delete_token(self, token):
         """
-        Delete one or more regular or special tokens. This also changes the token IDs. See "modify".
+        Delete one or more regular or special tokens.
         You can give the token in either its encoded or decoded form.
+
+        Returns:
+            int: The new size of the vocabulary.
         """
         return self.modify(None, None, token, 0)
+    
+    def delete_token_by_id(self, id):
+        """
+        Delete one or more regular or special token by specifying the token ID.
+
+        Returns:
+            int: The new size of the vocabulary.
+        """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
+        if isinstance(id, int):
+            id = [id]
+        else:
+            if not is_iterable(id):
+                raise ValueError("TokenMonster: Input to delete_token_by_id must be int or list of ints.")
+            if len(id) == 0:
+                return self.vocab_size
+            if not isinstance(id[0], int):
+                raise ValueError("TokenMonster: Input to delete_token_by_id must be int or list of ints.")
+        payload = _write_uint32(len(id)) + _pack_32bit_ints(id)
+        job_type = 16
+        self.vocab_size = Vocab._communicate(job_type, self.id, len(payload), payload)
+        self._modified()
+        return self.vocab_size
 
     def add_special_token(self, token):
         """
-        Add one or more special tokens. This also changes the token IDs. See "modify".
+        Add one or more special tokens.
+
+        Returns:
+            int: The new size of the vocabulary.
         """
         return self.modify(token, None, None, 0)
     
-    def resize(self, size):
+    def resize(self, size, reset_token_ids = False):
         """
-        Changes the size of the vocabulary. This also changes the token IDs. See "modify".
+        Changes the size of the vocabulary and optionally resets the token IDs.
 
         A vocabulary can be enlarged as well reduced in size. Only the worst performing
         tokens are removed when reducing.
+
+        Resizing only removes regular tokens that are not single byte token and have
+        score > 0. If there are not enough of these, the new size may not match
+        the target size.
+
+        Returns:
+            int: The new size of the vocabulary.
         """
-        return self.modify(None, None, None, size)
+        return self.modify(None, None, None, size, None, reset_token_ids)
+    
+    def reset_token_ids(self):
+        """
+        Resets the token IDs to be sequential beginning from zero.
+
+        If tokens have been deleted from the vocabulary there will be gaps in the token IDs.
+        Resetting the token IDs removes these gaps but all tokens will have new IDs.
+        """
+        return self.modify(None, None, None, None, None, True)
     
     def enable_unk_token(self):
         """
         Enables the UNK token.
-        The UNK token can be added or removed without affecting the rest of the vocabulary.
         If enabled, the UNK token appears whenever there is a character that is not in the vocabulary.
         Note that the UNK token will not be enabled if all possible characters have tokens.
-        Use get_unk_token to retrieve the ID for the UNK token.
+        Use `vocab.unk_token_id()` to retrieve the ID for the UNK token.
+
+        Returns:
+            int: The new size of the vocabulary.
         """
         return self.modify(None, None, None, 0, True)
     
     def disable_unk_token(self):
         """
         Disables the UNK token.
-        The UNK token can be added or removed without affecting the rest of the vocabulary.
         Without an UNK token, any character for which there is no token is ignored during tokenization
+
+        Returns:
+            int: The new size of the vocabulary.
         """
         return self.modify(None, None, None, 0, False)
 
     def save(self, fname):
         """
         Saves the current vocabulary to a file.
 
@@ -618,19 +827,42 @@
 
         Returns:
             Nothing (raises error on failure)
 
         Usage:
             vocab.save("test.vocab")
         """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         fname_encoded = fname.encode("utf-8")
         if len(fname_encoded) > 255:
             raise RuntimeError("TokenMonster: Vocabulary filepath is too long, it must be less than 256 characters")
         payload = _write_uint8(len(fname_encoded)) + fname_encoded
-        TokenMonster._communicate(12, 0, len(payload), payload)
+        Vocab._communicate(12, 0, len(payload), payload)
+
+    def export_yaml(self, order_by_score = False):
+        """
+        Exports the vocabulary as a YAML file, which is returned as a bytes string.
+
+        Parameters:
+            order_by_score (boolean): If true the tokens are order by score instead of alphabetically.
+
+        Returns:
+            bytes string: The vocabulary in YAML format.
+
+        Usage:
+            yaml = vocab.export_yaml()
+            with open(file_path, 'wb') as file:
+                file.write(yaml)
+        """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
+        payload = _write_uint8(int(order_by_score))
+        job_type = 19
+        return Vocab._communicate(job_type, self.id, 1, payload)
 
     def deserialize_tokens(self, binary_string):
         """
         Deserializes a binary string back into a list of ints (tokens).
         The encoding_length needs to be recorded separetely.
         """
         if self.encoding_length == 2:
@@ -694,38 +926,55 @@
                 for i, item in enumerate(data):
                     if isinstance(item, str):
                         if self.charset == 2:
                             data[i] = item.encode("utf-16-le")
                         else:
                             data[i] = item.encode("utf-8")
                     elif not isinstance(item, bytes):
-                        raise ValueError("TokenMonster: Invalid input")
+                        raise ValueError("TokenMonster: Invalid input for vocabulary modification. Input should be string or bytes string, or list thereof.")
         else:
-            raise ValueError("TokenMonster: Invalid input")
+            raise ValueError("TokenMonster: Invalid input for vocabulary modification. Input should be string or bytes string, or list thereof.")
+    
+    def _modified(self):
+        self._modified_id += 1
+        self.dictionary = None
+        self.token_to_id = None
+        self.unk = False
+        if self.vocab_size > 65536:
+            self.encoding_length = 4
+        else:
+            self.encoding_length = 2
+        # Unload all the decoder objects
+        for _, decoder_id in enumerate(self._decoders):
+            Vocab._communicate(6, decoder_id, 0)
+        self._decoders = []
 
     @classmethod
-    def set_local_directory(cls, dir=None):
+    def _set_local_directory(cls, dir=None):
         if dir is None:
             if cls._dir is not None:
                 return
             dir = os.path.join(os.path.expanduser("~"), "_tokenmonster")
         cls._os, cls._bin = _get_binary_filename()
         if not os.path.exists(dir):
             os.makedirs(dir)
             if not os.path.exists(dir):
                 raise RuntimeError("Unable to create directory: {}".format(dir))
         cls._dir = dir
 
     @classmethod
-    def disconnect(cls):
+    def _disconnect(cls):
         if cls.process is not None:
             cls.process.stdin.close()
             cls.process.stdout.close()
             cls.process.kill()
             cls.process = None
+            for i in range(len(cls._vocabs)):
+                cls._vocabs[i]._modified_id = -1
+            cls._vocabs = []
 
     @classmethod
     def _download(cls, url, fname):
         urllib.request.urlretrieve(url, os.path.join(cls._dir, fname))
 
     @classmethod
     def _file_exists(cls, fname):
@@ -738,21 +987,21 @@
         if data is not None:
             if isinstance(data, bytes):
                 cls._process.stdin.write(data)
             else:
                 for item in data:
                     cls._process.stdin.write(item)
         cls._process.stdin.flush()
-        response = TokenMonster._process.stdout.read(9)
+        response = Vocab._process.stdout.read(9)
         if len(response) == 0: # this happens when the app is shutting down
             return None
         status = response[0]
         if status == 0: # HEADER_IS_LENGTH
             length = _read_uint64(response[1:9])
-            return TokenMonster._process.stdout.read(length)
+            return Vocab._process.stdout.read(length)
         elif status == 1: # HEADER_IS_ID
             id = _read_uint32(response[1:5])
             return id
         elif status == 2: # HEADER_IS_EMPTY
             return None
         elif status == 10: # ERROR_ID_DOES_NOT_EXIST
             raise RuntimeError("tokenmonsterserver: This ID does not exist")
@@ -760,14 +1009,18 @@
             raise RuntimeError("tokenmonsterserver: This ID has already been unloaded")
         elif status == 12: # ERROR_FILE_CANNOT_OPEN
             raise RuntimeError("tokenmonsterserver: Cannot open or save vocabulary file, please check permissions")
         elif status == 13: # ERROR_NORMALIZATION_FAILED
             raise RuntimeError("tokenmonsterserver: An error occurred normalizing your text")
         elif status == 14: # ERROR_READ_FAILED
             raise RuntimeError("tokenmonsterserver: Read failed")
+        elif status == 15: # ERROR_INVALID_JOB
+            raise RuntimeError("tokenmonsterserver: Invalid job ID")
+        elif status == 16: # ERROR_INVALID_JOB
+            raise ValueError("TokenMonster: YAML is invalid")
         else:
             raise RuntimeError("tokenmonsterserver: Unknown error occurred")
 
     @classmethod
     def _start_process(cls):
         exe = os.path.join(cls._dir, cls._bin)
         pid = str(os.getpid())
@@ -778,39 +1031,57 @@
             return False
         else:
             if cls._process is None:
                 return False
             return True
 
     @classmethod
+    def _install_tokenmonsterserver(cls):
+        cls._download(_TOKENMONSTER_URL + "binaries/" + cls._os + "/" + cls._bin, cls._bin)
+        if not cls._file_exists(cls._bin):
+            raise FileNotFoundError("TokenMonster: Unable to download " + cls._bin + " to " + cls._dir + " from Hugging Face")
+        # attempt to add execute permission for this user
+        exe = os.path.join(cls._dir, cls._bin)
+        if cls._os.startswith("windows"):
+            try:
+                username = getpass.getuser()
+                subprocess.run(["icacls", exe, "/grant", f"{username}:(RX)"], check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            except Exception:
+                pass
+        else:
+            try:
+                os.chmod(exe, 0o700)
+            except Exception:
+                pass
+        if not cls._start_process():
+            sep = '=' * 64
+            raise RuntimeError("\n"+sep+"\n\n\tTo get started with TokenMonster please enable execute permissions for:\n\t"+exe+"\n\n"+sep+"\n")
+
+    @classmethod
     def _connect(cls):
         if cls._process is None:
+            for i in range(len(cls._vocabs)):
+                cls._vocabs[i]._modified_id = -1
+            cls._vocabs = []
             if cls._file_exists(cls._bin):
                 if not cls._start_process():
                     raise RuntimeError("TokenMonster: Unable to start tokenmonsterserver, please give execute permission to " + os.path.join(cls._dir, cls._bin))
             else:
-                cls._download(_TOKENMONSTER_URL + "binaries/" + cls._os + "/" + cls._bin, cls._bin)
-                if not cls._file_exists(cls._bin):
-                    raise FileNotFoundError("TokenMonster: Unable to download " + cls._bin + " to " + cls._dir + " from Hugging Face")
-                # attempt to add execute permission for this user
-                exe = os.path.join(cls._dir, cls._bin)
-                if cls._os.startswith("windows"):
-                    try:
-                        username = getpass.getuser()
-                        subprocess.run(["icacls", exe, "/grant", f"{username}:(RX)"], check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-                    except Exception:
-                        pass
-                else:
-                    try:
-                        os.chmod(exe, 0o700)
-                    except Exception:
-                        pass
-                if not cls._start_process():
-                    sep = '=' * 64
-                    raise RuntimeError("\n"+sep+"\n\n\tTo get started with TokenMonster please enable execute permissions for:\n\t"+exe+"\n\n"+sep+"\n")
+                cls._install_tokenmonsterserver()
+            # Now check verison number
+            tms_version = cls._communicate(0, 0, 0)
+            if tms_version < _TMS_VERSION_ID:
+                cls._disconnect()
+                cls._install_tokenmonsterserver()
+                tms_version = cls._communicate(0, 0, 0)
+                if tms_version < _TMS_VERSION_ID:
+                    raise RuntimeError("TokenMonster: tokenmonsterserver version does not match Python library version")
+            if tms_version > _TMS_VERSION_ID:
+                cls.disconnect()
+                raise RuntimeError("TokenMonster: Version mismatch. Please update tokenmonster with `pip install --upgrade`")
 
     #@classmethod
     #def _reconnect(cls):
     #    cls._close()
     #    cls._connect()
 
     #@classmethod
@@ -818,14 +1089,15 @@
     #    cls._process.stdout.read()
 
     # class level variables
     _dir = None
     _os = None
     _bin = None
     _process = None
+    _vocabs = []
 
 
 ### Helper Functions
 
 def _is_prebuilt(name):
     parts = name.split("-")
     if len(parts) < 4 or len(parts) > 5:
@@ -926,7 +1198,8 @@
 
 def is_iterable(obj):
     if isinstance(obj, (str, bytes)):
         return False
     return isinstance(obj, Iterable)
 
 _TOKENMONSTER_URL = "https://huggingface.co/alasdairforsythe/tokenmonster/resolve/main/"
+_TMS_VERSION_ID = 1
```

