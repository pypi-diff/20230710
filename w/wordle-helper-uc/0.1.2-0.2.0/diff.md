# Comparing `tmp/wordle_helper_uc-0.1.2.tar.gz` & `tmp/wordle_helper_uc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordle_helper_uc-0.1.2.tar", max compression
+gzip compressed data, was "wordle_helper_uc-0.2.0.tar", max compression
```

## Comparing `wordle_helper_uc-0.1.2.tar` & `wordle_helper_uc-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1116 2023-07-06 07:10:16.358498 wordle_helper_uc-0.1.2/README.md
--rw-r--r--   0        0        0      401 2023-07-06 07:05:11.330754 wordle_helper_uc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 06:32:02.572224 wordle_helper_uc-0.1.2/wordle_helper_uc/__init__.py
--rwxr-xr-x   0        0        0    10360 2023-07-06 07:04:31.296061 wordle_helper_uc-0.1.2/wordle_helper_uc/__main__.py
--rw-r--r--   0        0        0   788627 2023-07-06 07:00:57.376317 wordle_helper_uc-0.1.2/wordle_helper_uc/words.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 wordle_helper_uc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1471 2023-07-10 14:44:01.043579 wordle_helper_uc-0.2.0/README.md
+-rw-r--r--   0        0        0      401 2023-07-10 14:42:07.794180 wordle_helper_uc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 06:32:02.572224 wordle_helper_uc-0.2.0/wordle_helper_uc/__init__.py
+-rwxr-xr-x   0        0        0    12869 2023-07-10 14:42:22.095721 wordle_helper_uc-0.2.0/wordle_helper_uc/__main__.py
+-rw-r--r--   0        0        0   788627 2023-07-06 07:00:57.376317 wordle_helper_uc-0.2.0/wordle_helper_uc/words.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 wordle_helper_uc-0.2.0/PKG-INFO
```

### Comparing `wordle_helper_uc-0.1.2/README.md` & `wordle_helper_uc-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 GitHub repository: https://github.com/Parzival1918/WordleHelper
 
 Input the correct letters and misplaced ones and program spits all words that comply with that.
 
 Word list taken from https://github.com/tabatkins/wordle-list.
 
+## Installation
+
+* `pipx install wordle-helper-uc`. You must install `pipx` first if you don't have it already.
+* Run with `wordle-helper` in your terminal.
+
 ### Dependencies
 
 * argparse
 * json
 * os
 
 ## wordle-helper.py Args
@@ -42,7 +47,15 @@
 ### *-j, --json-output*
 
 Output the result in json format
 
 ### *-s, -sorted*
 
 Sort the possible words by their usage in the english language. Information taken from https://www.kaggle.com/datasets/rtatman/english-word-frequency
+
+### *--version*
+
+Print the version of the program.
+
+### *--definition*
+
+Print the definition of the first word of the list. Information taken from https://api.dictionaryapi.dev/api/v2/entries/en/.
```

### Comparing `wordle_helper_uc-0.1.2/wordle_helper_uc/__main__.py` & `wordle_helper_uc-0.2.0/wordle_helper_uc/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,15 +39,15 @@
    YELLOW = '\033[1;33;48m'
    RED = '\033[1;31;48m'
    BLACK = '\033[1;30;48m'
    UNDERLINE = '\033[4;37;48m'
    END = '\033[1;37;0m'
     
 #Function to print possible words
-def printPossibleWords(possibleWords: list, output_json: bool, user_input: str, correctLetters: list, misplacedLetters: list, wrong_letters: str, sort_output: bool):
+def printPossibleWords(args, possibleWords: list, output_json: bool, user_input: str, correctLetters: list, misplacedLetters: list, wrong_letters: str, sort_output: bool):
     if output_json:
         addToInput = ""
         if wrong_letters != None:
             addToInput = " -w " + wrong_letters.lower()
         wrongOutput = ""
         if wrong_letters != None:
             wrongOutput = wrong_letters.lower()
@@ -82,22 +82,66 @@
             else:
                 print(TextColour.PURPLE + " > " + TextColour.END + word.rstrip(), end="")
             wordCount += 1
 
         #if (wordCount) % wordChunksperColumn != 0:
         print() #For new line
 
+        if args.definition:
+            url = "https://api.dictionaryapi.dev/api/v2/entries/en/" + possibleWords[0] #Get the first word
+            import requests
+            try:
+                response = requests.get(url, timeout=2)
+                response.raise_for_status()
+            except requests.exceptions.HTTPError as errh:
+                print(TextColour.RED + "Http Error:" + TextColour.END,errh)
+                return
+            except requests.exceptions.ConnectionError as errc:
+                print(TextColour.RED + "Error Connecting:" + TextColour.END,errc)
+                return
+            except requests.exceptions.Timeout as errt:
+                print(TextColour.RED + "Timeout Error:" + TextColour.END,errt)
+                return
+            except requests.exceptions.RequestException as err:
+                print(TextColour.RED + "Oops: Something Else" + TextColour.END,err)
+                return
+            
+            data = response.json()
+
+            if len(data) == 0:
+                print(TextColour.RED + "No definition found" + TextColour.END)
+                return
+            
+            #Print the definition and extra info
+            print(TextColour.GREEN + "Definition: " + TextColour.YELLOW + possibleWords[0] + TextColour.END)
+            #Phonetic
+            if "phonetic" in data[0]:
+                print(TextColour.CYAN + "   Phonetic: " + TextColour.YELLOW + data[0]["phonetic"] + TextColour.END)
+            #Origin
+            if "origin" in data[0]:
+                print(TextColour.CYAN + "   Origin: " + TextColour.YELLOW + data[0]["origin"] + TextColour.END)
+            #Meanings
+            if "meanings" in data[0]:
+                for pos,meaning in enumerate(data[0]["meanings"]):
+                    print(TextColour.CYAN + f"   ({pos+1}, {meaning['partOfSpeech']}): " + TextColour.YELLOW + meaning["definitions"][0]["definition"] + TextColour.END)
+                    #Example
+                    if "example" in meaning["definitions"][0]:
+                        print(TextColour.CYAN + "       |-> Example: " + TextColour.GREEN + TextColour.UNDERLINE + meaning["definitions"][0]["example"] + TextColour.END)
+
+
 def main():
-    parser = ap.ArgumentParser()
+    parser = ap.ArgumentParser(prog="wordle-helper", description="Program to help you find the Wordle of the day", epilog="Made by Pedro Juan Royo")
 
     #Parser arguments
     parser.add_argument("-i", "--input", help="Words you tried in wordle", type=str, required=True, nargs='*')
     parser.add_argument("-w", "--wrong", help="All wrong letters", type=str)
     parser.add_argument("-j", "--json-output", help="Output the results in json format", action="store_true")
     parser.add_argument("-s", "--sorted", help="Sort output by word usage", action="store_true")
+    parser.add_argument("--definition", help="Get the definition of the first word.", action="store_true")
+    parser.add_argument('--version', action='version', version='%(prog)s 0.2.0')
 
     args = parser.parse_args()
 
     #Ask for user input
     #user_input = input("Enter the word you tried in wordle: ")
     user_inputs = args.input
     wrong_letters = args.wrong
@@ -271,11 +315,11 @@
             if word not in wordUsageDict:
                 wordUsageDict[word] = 0
 
         possibleWords.sort(key=lambda x: wordUsageDict[x], reverse=True)
         # print(wordUsageDict[possibleWords[0]])
         # print(wordUsageDict[possibleWords[-1]])
 
-    printPossibleWords(possibleWords, output_json, user_inputs, correctLetters, misplacedLetters, wrong_letters, sort_output)
+    printPossibleWords(args, possibleWords, output_json, user_inputs, correctLetters, misplacedLetters, wrong_letters, sort_output)
 
 if __name__ == "__main__":
     main()
```

### Comparing `wordle_helper_uc-0.1.2/wordle_helper_uc/words.py` & `wordle_helper_uc-0.2.0/wordle_helper_uc/words.py`

 * *Files identical despite different names*

### Comparing `wordle_helper_uc-0.1.2/PKG-INFO` & `wordle_helper_uc-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordle-helper-uc
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Author: Pedro Juan Royo
 Author-email: pedro.juan.royo@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -13,14 +13,19 @@
 
 GitHub repository: https://github.com/Parzival1918/WordleHelper
 
 Input the correct letters and misplaced ones and program spits all words that comply with that.
 
 Word list taken from https://github.com/tabatkins/wordle-list.
 
+## Installation
+
+* `pipx install wordle-helper-uc`. You must install `pipx` first if you don't have it already.
+* Run with `wordle-helper` in your terminal.
+
 ### Dependencies
 
 * argparse
 * json
 * os
 
 ## wordle-helper.py Args
@@ -54,7 +59,14 @@
 
 Output the result in json format
 
 ### *-s, -sorted*
 
 Sort the possible words by their usage in the english language. Information taken from https://www.kaggle.com/datasets/rtatman/english-word-frequency
 
+### *--version*
+
+Print the version of the program.
+
+### *--definition*
+
+Print the definition of the first word of the list. Information taken from https://api.dictionaryapi.dev/api/v2/entries/en/.
```

