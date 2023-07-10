# Comparing `tmp/autodistill-sam-clip-0.1.2.tar.gz` & `tmp/autodistill-sam-clip-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-sam-clip-0.1.2.tar", last modified: Thu Jun 29 13:46:33 2023, max compression
+gzip compressed data, was "autodistill-sam-clip-0.1.3.tar", last modified: Mon Jul 10 15:17:11 2023, max compression
```

## Comparing `autodistill-sam-clip-0.1.2.tar` & `autodistill-sam-clip-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:46:33.570834 autodistill-sam-clip-0.1.2/
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-09 18:33:41.000000 autodistill-sam-clip-0.1.2/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      491 2023-06-29 13:46:33.570680 autodistill-sam-clip-0.1.2/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1903 2023-06-29 13:44:02.000000 autodistill-sam-clip-0.1.2/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:46:33.569340 autodistill-sam-clip-0.1.2/autodistill_sam_clip/
--rw-r--r--   0 james      (501) staff       (20)       73 2023-06-29 13:46:14.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2798 2023-06-12 08:32:31.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip/helpers.py
--rw-r--r--   0 james      (501) staff       (20)     4528 2023-06-28 10:56:59.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip/sam_clip.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:46:33.570475 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      491 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      343 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      138 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       21 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 13:46:33.570895 autodistill-sam-clip-0.1.2/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1481 2023-06-29 13:43:39.000000 autodistill-sam-clip-0.1.2/setup.py
+drwxrwxr-x   0 arty      (1001) arty      (1002)        0 2023-07-10 15:17:11.176398 autodistill-sam-clip-0.1.3/
+-rw-rw-r--   0 arty      (1001) arty      (1002)    11356 2023-07-10 15:00:35.000000 autodistill-sam-clip-0.1.3/LICENSE
+-rw-rw-r--   0 arty      (1001) arty      (1002)      479 2023-07-10 15:17:11.172398 autodistill-sam-clip-0.1.3/PKG-INFO
+-rw-rw-r--   0 arty      (1001) arty      (1002)     1880 2023-07-10 15:00:35.000000 autodistill-sam-clip-0.1.3/README.md
+drwxrwxr-x   0 arty      (1001) arty      (1002)        0 2023-07-10 15:17:11.172398 autodistill-sam-clip-0.1.3/autodistill_sam_clip/
+-rw-rw-r--   0 arty      (1001) arty      (1002)       73 2023-07-10 15:05:53.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip/__init__.py
+-rw-rw-r--   0 arty      (1001) arty      (1002)     2798 2023-07-10 15:00:35.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip/helpers.py
+-rw-rw-r--   0 arty      (1001) arty      (1002)     5286 2023-07-10 15:00:35.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip/sam_clip.py
+drwxrwxr-x   0 arty      (1001) arty      (1002)        0 2023-07-10 15:17:11.172398 autodistill-sam-clip-0.1.3/autodistill_sam_clip.egg-info/
+-rw-rw-r--   0 arty      (1001) arty      (1002)      479 2023-07-10 15:17:11.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip.egg-info/PKG-INFO
+-rw-rw-r--   0 arty      (1001) arty      (1002)      343 2023-07-10 15:17:11.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip.egg-info/SOURCES.txt
+-rw-rw-r--   0 arty      (1001) arty      (1002)        1 2023-07-10 15:17:11.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip.egg-info/dependency_links.txt
+-rw-rw-r--   0 arty      (1001) arty      (1002)      138 2023-07-10 15:17:11.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip.egg-info/requires.txt
+-rw-rw-r--   0 arty      (1001) arty      (1002)       21 2023-07-10 15:17:11.000000 autodistill-sam-clip-0.1.3/autodistill_sam_clip.egg-info/top_level.txt
+-rw-rw-r--   0 arty      (1001) arty      (1002)       38 2023-07-10 15:17:11.176398 autodistill-sam-clip-0.1.3/setup.cfg
+-rw-rw-r--   0 arty      (1001) arty      (1002)     1469 2023-07-10 15:00:35.000000 autodistill-sam-clip-0.1.3/setup.py
```

### Comparing `autodistill-sam-clip-0.1.2/LICENSE` & `autodistill-sam-clip-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-sam-clip-0.1.2/README.md` & `autodistill-sam-clip-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 
 # label all images in a folder called `context_images`
 base_model.label("./context_images", extension=".jpeg")
 ```
 
 ## License
 
-SAM licensed under an [Apache 2.0 license](LICENSE). CLIP is licensed under an [MIT license](LICENSE).
+The code in this repository is licensed under an [Apache 2.0 license](LICENSE).
 
 ## 🏆 Contributing
 
 We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
```

### Comparing `autodistill-sam-clip-0.1.2/autodistill_sam_clip/helpers.py` & `autodistill-sam-clip-0.1.3/autodistill_sam_clip/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-sam-clip-0.1.2/autodistill_sam_clip/sam_clip.py` & `autodistill-sam-clip-0.1.3/autodistill_sam_clip/sam_clip.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,129 +25,149 @@
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
 @dataclass
 class SAMCLIP(DetectionBaseModel):
     ontology: CaptionOntology
     sam_predictor: SamAutomaticMaskGenerator
+    DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     def __init__(self, ontology: CaptionOntology):
         self.ontology = ontology
         self.sam_predictor = load_SAM()
 
         if not os.path.exists(f"{HOME}/.cache/autodistill/clip"):
             os.makedirs(f"{HOME}/.cache/autodistill/clip")
 
             os.system("pip install ftfy regex tqdm")
             os.system(
                 f"cd {HOME}/.cache/autodistill/clip && pip install git+https://github.com/openai/CLIP.git"
             )
 
-        # add clip path to user path
+        # add clip path to path
         sys.path.insert(0, f"{HOME}/.cache/autodistill/clip/CLIP")
 
         import clip
 
         model, preprocess = clip.load("ViT-B/32", device=DEVICE)
 
         self.clip_model = model
         self.clip_preprocess = preprocess
         self.tokenize = clip.tokenize
 
     def predict(self, input: str, confidence: int = 0.5) -> sv.Detections:
         image_bgr = cv2.imread(input)
         image_rgb = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2RGB)
 
+        # SAM Predictions
         sam_result = self.sam_predictor.generate(image_rgb)
 
+        # mask_annotator = sv.MaskAnnotator()
+
+        # annotated_image = mask_annotator.annotate(
+        #     scene=image_bgr, detections=sv.Detections.from_sam(sam_result)
+        # )
+
+        # cv2.imshow("image", annotated_image)
+        # cv2.waitKey(0)
+
         valid_detections = []
 
         labels = self.ontology.prompts()
 
         nms_data = []
 
         if len(sam_result) == 0:
             return sv.Detections.empty()
 
-        if "background" not in [l.lower() for l in labels]:
-            labels.append("background")
+        labels.append("background")
 
         for mask in sam_result:
             mask_item = mask["segmentation"]
 
             image = image_rgb.copy()
 
-            bbox = mask["bbox"]
+            # image[mask_item == 0] = 0
 
-            xyxy = [bbox[0], bbox[1], bbox[0] + bbox[2], bbox[1] + bbox[3]]
-
-            # cut out mask from image using numpy indexing
-            image[mask_item == 0] = 0
+            # transform box from xywh to xyxy
+            mask["bbox"] = [
+                mask["bbox"][0],
+                mask["bbox"][1],
+                mask["bbox"][0] + mask["bbox"][2],
+                mask["bbox"][1] + mask["bbox"][3],
+            ]
+
+            # cut out bbox
+            image = image[
+                int(mask["bbox"][1]) : int(mask["bbox"][3]),
+                int(mask["bbox"][0]) : int(mask["bbox"][2]),
+            ]
 
             # fix ValueError: tile cannot extend outside image
             if image.shape[0] == 0 or image.shape[1] == 0:
                 continue
 
             # show me the bbox
             image = Image.fromarray(image)
 
             image = self.clip_preprocess(image).unsqueeze(0).to(DEVICE)
 
-            with torch.no_grad():
-                image_features = self.clip_model.encode_image(image)
+            cosime_sims = []
 
+            with torch.no_grad():
+                image_features = self.clip_model.encode_image(image).to(DEVICE)
                 image_features /= image_features.norm(dim=-1, keepdim=True)
 
-                text = self.tokenize(labels)
-
-                text_features = self.clip_model.encode_text(text)
-
+                text = self.tokenize(labels).to(DEVICE)
+                text_features = self.clip_model.encode_text(text).to(DEVICE)
                 text_features /= text_features.norm(dim=-1, keepdim=True)
+                # get cosine similarity between image and text features
 
                 similarity = (100.0 * image_features @ text_features.T).softmax(dim=-1)
 
-                if similarity.shape[0] == 0:
-                    continue
+                print(similarity)
+
+                cosime_sims.append(similarity[0][0].item())
 
-                max_prob, max_idx = similarity[0].max(dim=0)
+            max_prob = None
+            max_idx = None
 
-                if max_prob < confidence:
-                    continue
+            values, indices = torch.topk(torch.tensor(cosime_sims), 1)
 
-                if labels[max_idx] == "background":
-                    continue
+            max_prob = values[0].item()
+            max_idx = indices[0].item()
 
+            if max_prob > confidence:
                 valid_detections.append(
                     sv.Detections(
-                        xyxy=np.array([xyxy]),
+                        xyxy=np.array([mask["bbox"]]),
                         confidence=np.array([max_prob]),
                         mask=np.array([mask_item]),
                         class_id=np.array([max_idx]),
                     )
                 )
-
                 # (x_min, y_min, x_max, y_max, score, class)
                 nms_data.append(
                     (
                         mask["bbox"][0],
                         mask["bbox"][1],
                         mask["bbox"][2],
                         mask["bbox"][3],
                         max_prob,
                         max_idx,
                     )
                 )
 
-        nms = sv.non_max_suppression(np.array(nms_data), 0.5)
+        final_detections = valid_detections
 
-        print(nms)
+        nms = sv.non_max_suppression(np.array(nms_data), 0.5)
 
         final_detections = []
-        ids = []
 
         # nms is list of bools
         for idx, is_valid in enumerate(nms):
             if is_valid:
                 final_detections.append(valid_detections[idx])
-                ids.append(valid_detections[idx].class_id[0])
 
-        return combine_detections(final_detections, overwrite_class_ids=ids)
+        return combine_detections(
+            final_detections, overwrite_class_ids=[0] * len(final_detections)
+        )
```

### Comparing `autodistill-sam-clip-0.1.2/setup.py` & `autodistill-sam-clip-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,12 +38,12 @@
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

