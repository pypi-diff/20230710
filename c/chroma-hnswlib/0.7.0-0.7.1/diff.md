# Comparing `tmp/chroma-hnswlib-0.7.0.tar.gz` & `tmp/chroma-hnswlib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroma-hnswlib-0.7.0.tar", last modified: Fri Jun  9 23:23:09 2023, max compression
+gzip compressed data, was "chroma-hnswlib-0.7.1.tar", last modified: Mon Jul 10 19:23:00 2023, max compression
```

## Comparing `chroma-hnswlib-0.7.0.tar` & `chroma-hnswlib-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-06-09 23:23:09.185303 chroma-hnswlib-0.7.0/
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)       36 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/MANIFEST.in
--rw-r--r--   0 hammad     (501) staff       (20)      231 2023-06-09 23:23:09.184790 chroma-hnswlib-0.7.0/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)    15342 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/README.md
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-06-09 23:23:09.178135 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      231 2023-06-09 23:23:09.000000 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      617 2023-06-09 23:23:09.000000 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-06-09 23:23:09.000000 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-06-09 21:41:48.000000 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/not-zip-safe
--rw-r--r--   0 hammad     (501) staff       (20)        6 2023-06-09 23:23:09.000000 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        8 2023-06-09 23:23:09.000000 chroma-hnswlib-0.7.0/chroma_hnswlib.egg-info/top_level.txt
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-06-09 23:23:09.179262 chroma-hnswlib-0.7.0/hnswlib/
--rw-r--r--   0 hammad     (501) staff       (20)     5791 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/hnswlib/bruteforce.h
--rw-r--r--   0 hammad     (501) staff       (20)    53929 2023-06-08 23:17:12.000000 chroma-hnswlib-0.7.0/hnswlib/hnswalg.h
--rw-r--r--   0 hammad     (501) staff       (20)     5199 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/hnswlib/hnswlib.h
--rw-r--r--   0 hammad     (501) staff       (20)    10855 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/hnswlib/space_ip.h
--rw-r--r--   0 hammad     (501) staff       (20)     8561 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/hnswlib/space_l2.h
--rw-r--r--   0 hammad     (501) staff       (20)     1790 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/hnswlib/visited_list_pool.h
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-06-09 23:23:09.184119 chroma-hnswlib-0.7.0/hnswlib.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      224 2023-06-09 22:19:32.000000 chroma-hnswlib-0.7.0/hnswlib.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      391 2023-06-09 22:19:32.000000 chroma-hnswlib-0.7.0/hnswlib.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-06-09 22:19:32.000000 chroma-hnswlib-0.7.0/hnswlib.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-06-07 17:22:06.000000 chroma-hnswlib-0.7.0/hnswlib.egg-info/not-zip-safe
--rw-r--r--   0 hammad     (501) staff       (20)        6 2023-06-09 22:19:32.000000 chroma-hnswlib-0.7.0/hnswlib.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        8 2023-06-09 22:19:32.000000 chroma-hnswlib-0.7.0/hnswlib.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)      148 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.0/pyproject.toml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-06-09 23:23:09.176955 chroma-hnswlib-0.7.0/python_bindings/
--rw-r--r--   0 hammad     (501) staff       (20)    37619 2023-06-08 23:11:29.000000 chroma-hnswlib-0.7.0/python_bindings/bindings.cpp
--rw-r--r--   0 hammad     (501) staff       (20)       38 2023-06-09 23:23:09.185418 chroma-hnswlib-0.7.0/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)     3671 2023-06-09 22:48:25.000000 chroma-hnswlib-0.7.0/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.296464 chroma-hnswlib-0.7.1/
+-rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/LICENSE
+-rw-r--r--   0 hammad     (501) staff       (20)       36 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/MANIFEST.in
+-rw-r--r--   0 hammad     (501) staff       (20)      231 2023-07-10 19:23:00.296309 chroma-hnswlib-0.7.1/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      109 2023-07-10 19:13:46.000000 chroma-hnswlib-0.7.1/README.md
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.294023 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      231 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      433 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-06-29 14:19:20.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/not-zip-safe
+-rw-r--r--   0 hammad     (501) staff       (20)        6 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        8 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.296055 chroma-hnswlib-0.7.1/hnswlib/
+-rw-r--r--   0 hammad     (501) staff       (20)     5791 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/bruteforce.h
+-rw-r--r--   0 hammad     (501) staff       (20)    66429 2023-07-10 19:12:05.000000 chroma-hnswlib-0.7.1/hnswlib/hnswalg.h
+-rw-r--r--   0 hammad     (501) staff       (20)     5199 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/hnswlib.h
+-rw-r--r--   0 hammad     (501) staff       (20)    10855 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/space_ip.h
+-rw-r--r--   0 hammad     (501) staff       (20)     8561 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/space_l2.h
+-rw-r--r--   0 hammad     (501) staff       (20)     1790 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/visited_list_pool.h
+-rw-r--r--   0 hammad     (501) staff       (20)      148 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/pyproject.toml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.290136 chroma-hnswlib-0.7.1/python_bindings/
+-rw-r--r--   0 hammad     (501) staff       (20)    38066 2023-07-10 19:12:05.000000 chroma-hnswlib-0.7.1/python_bindings/bindings.cpp
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2023-07-10 19:23:00.296512 chroma-hnswlib-0.7.1/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)     3671 2023-07-10 19:14:10.000000 chroma-hnswlib-0.7.1/setup.py
```

### Comparing `chroma-hnswlib-0.7.0/LICENSE` & `chroma-hnswlib-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.0/hnswlib/bruteforce.h` & `chroma-hnswlib-0.7.1/hnswlib/bruteforce.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.0/hnswlib/hnswalg.h` & `chroma-hnswlib-0.7.1/hnswlib/hnswalg.h`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 #include "visited_list_pool.h"
 #include "hnswlib.h"
 #include <atomic>
 #include <random>
 #include <stdlib.h>
 #include <assert.h>
 #include <unordered_set>
+#include <set>
 #include <list>
 
 namespace hnswlib {
 typedef unsigned int tableint;
 typedef unsigned int linklistsizeint;
+const int PERSISTENCE_VERSION = 1; // Used by persistent indices to check if the index on disk is compatible with the code
 
 template<typename dist_t>
 class HierarchicalNSW : public AlgorithmInterface<dist_t> {
  public:
     static const tableint MAX_LABEL_OPERATION_LOCKS = 65536;
     static const unsigned char DELETE_MARK = 0x01;
 
@@ -68,44 +70,66 @@
     bool allow_replace_deleted_ = false;  // flag to replace deleted elements (marked as deleted) during insertions
     bool normalize_ = false;  // flag to normalize vectors before insertion
 
     std::mutex deleted_elements_lock;  // lock for deleted_elements
     std::unordered_set<tableint> deleted_elements;  // contains internal ids of deleted elements
 
 
+    bool persist_on_write_ = false;
+    std::string persist_location_;
+    std::mutex elements_to_persist_lock_; // lock for elements_to_persist_
+    std::set<tableint> elements_to_persist_; // dirty elements to persist
+    // File handles for persistence
+    std::ofstream output_header_; // output stream for header
+    std::ofstream output_data_level0_; // output stream for data level 0
+    std::ofstream output_length_; // output stream for length
+    std::ofstream output_link_lists_; // output stream for link lists
+
     HierarchicalNSW(SpaceInterface<dist_t> *s) {
     }
 
 
     HierarchicalNSW(
         SpaceInterface<dist_t> *s,
         const std::string &location,
         bool nmslib = false,
         size_t max_elements = 0,
         bool allow_replace_deleted = false,
-        bool normalize = false)
+        bool normalize = false,
+        bool persist_on_write = false)
         : allow_replace_deleted_(allow_replace_deleted), 
-            normalize_(normalize) {
-        loadIndex(location, s, max_elements);
+            normalize_(normalize),
+            persist_on_write_(persist_on_write),
+            persist_location_(location) {
+        // Persisted indices are stored differently
+        if (persist_on_write_){
+            loadPersistedIndex(s, max_elements);
+        } else {
+            loadIndex(location, s, max_elements);
+        }
     }
 
 
     HierarchicalNSW(
         SpaceInterface<dist_t> *s,
         size_t max_elements,
         size_t M = 16,
         size_t ef_construction = 200,
         size_t random_seed = 100,
         bool allow_replace_deleted = false,
-        bool normalize = false)
+        bool normalize = false,
+        bool persist_on_write = false,
+        const std::string &persist_location = "")
         : link_list_locks_(max_elements),
             label_op_locks_(MAX_LABEL_OPERATION_LOCKS),
             element_levels_(max_elements),
             allow_replace_deleted_(allow_replace_deleted),
-            normalize_(normalize) {
+            normalize_(normalize),
+            persist_on_write_(persist_on_write),
+            persist_location_(persist_location) {
         max_elements_ = max_elements;
         num_deleted_ = 0;
         data_size_ = s->get_data_size();
         fstdistfunc_ = s->get_dist_func();
         dist_func_param_ = s->get_dist_func_param();
         M_ = M;
         maxM_ = M_;
@@ -140,26 +164,34 @@
 
         linkLists_ = (char **) malloc(sizeof(void *) * max_elements_);
         if (linkLists_ == nullptr)
             throw std::runtime_error("Not enough memory: HierarchicalNSW failed to allocate linklists");
         size_links_per_element_ = maxM_ * sizeof(tableint) + sizeof(linklistsizeint);
         mult_ = 1 / log(1.0 * M_);
         revSize_ = 1.0 / mult_;
+
+        if (persist_on_write_) {
+            if (persist_location_.empty()) {
+                throw std::runtime_error("persist_location_ is empty");
+            }
+           initPersistentIndex();
+        }
     }
 
 
     ~HierarchicalNSW() {
         free(data_level0_memory_);
         for (tableint i = 0; i < cur_element_count; i++) {
             if (element_levels_[i] > 0)
                 free(linkLists_[i]);
         }
         free(linkLists_);
         free(length_memory_);
         delete visited_list_pool_;
+        closePersistentIndexFileHandles();
     }
 
 
     struct CompareByFirst {
         constexpr bool operator()(std::pair<dist_t, tableint> const& a,
             std::pair<dist_t, tableint> const& b) const noexcept {
             return a.first < b.first;
@@ -460,21 +492,30 @@
     }
 
 
     linklistsizeint *get_linklist_at_level(tableint internal_id, int level) const {
         return level == 0 ? get_linklist0(internal_id) : get_linklist(internal_id, level);
     }
 
+    void markElementToPersist(tableint internal_id) {
+        std::unique_lock <std::mutex> lock_elements_to_persist(elements_to_persist_lock_);
+        elements_to_persist_.insert(internal_id);
+    }
+
 
     tableint mutuallyConnectNewElement(
         const void *data_point,
         tableint cur_c,
         std::priority_queue<std::pair<dist_t, tableint>, std::vector<std::pair<dist_t, tableint>>, CompareByFirst> &top_candidates,
         int level,
         bool isUpdate) {
+
+        // mark cur_c as dirty
+        markElementToPersist(cur_c);
+
         size_t Mcurmax = level ? maxM_ : maxM0_;
         getNeighborsByHeuristic2(top_candidates, M_);
         if (top_candidates.size() > M_)
             throw std::runtime_error("Should be not be more than M_ candidates returned by the heuristic");
 
         std::vector<tableint> selectedNeighbors;
         selectedNeighbors.reserve(M_);
@@ -510,14 +551,17 @@
                     throw std::runtime_error("Trying to make a link on a non-existent level");
 
                 data[idx] = selectedNeighbors[idx];
             }
         }
 
         for (size_t idx = 0; idx < selectedNeighbors.size(); idx++) {
+            // Note: We may want to lock _elements_to_persist outside the loop. Should profile this to see if it matters.
+            markElementToPersist(selectedNeighbors[idx]);
+
             std::unique_lock <std::mutex> lock(link_list_locks_[selectedNeighbors[idx]]);
 
             linklistsizeint *ll_other;
             if (level == 0)
                 ll_other = get_linklist0(selectedNeighbors[idx]);
             else
                 ll_other = get_linklist(selectedNeighbors[idx], level);
@@ -652,14 +696,295 @@
             writeBinaryPOD(output, linkListSize);
             if (linkListSize)
                 output.write(linkLists_[i], linkListSize);
         }
         output.close();
     }
 
+    std::string getHeaderLocation() {
+        return persist_location_ + "/header.bin";
+    }
+
+    std::string getDataLevel0Location() {
+        return persist_location_ + "/data_level0.bin";
+    }
+
+    std::string getLengthLocation() {
+        return persist_location_ + "/length.bin";
+    }
+
+    std::string getLinkListLocation() {
+        return persist_location_ + "/link_lists.bin";
+    }
+
+    // #pragma region PersistentIndex
+    void setupPersistentIndexFileHandles() {
+        this->output_header_ = std::ofstream(this->getHeaderLocation(), std::ios::in|std::ios::out|std::ios::binary);
+        if(!this->output_header_.is_open()) {
+            std::runtime_error("Cannot open file: " + this->getHeaderLocation());
+        }
+
+        this->output_data_level0_ = std::ofstream(this->getDataLevel0Location(), std::ios::in|std::ios::out|std::ios::binary);
+        if(!this->output_data_level0_.is_open()) {
+            std::runtime_error("Cannot open file: " + this->getDataLevel0Location());
+        }
+
+        this->output_length_ = std::ofstream(this->getLengthLocation(), std::ios::in|std::ios::out|std::ios::binary);
+        if(!this->output_length_.is_open()) {
+            std::runtime_error("Cannot open file: " + this->getLengthLocation());
+        }
+
+        this->output_link_lists_ = std::ofstream(this->getLinkListLocation(), std::ios::in|std::ios::out|std::ios::binary);
+        if(!this->output_link_lists_.is_open()) {
+            std::runtime_error("Cannot open file: " + this->getLinkListLocation());
+        }
+    }
+
+    void closePersistentIndexFileHandles() {
+        this->output_header_.close();
+        this->output_data_level0_.close();
+        this->output_length_.close();
+        this->output_link_lists_.close();
+    }
+
+    void initPersistentIndex() {
+        // A persisted index is stored as four files
+        // The latter 3 files are stored seperately so that they can each grow as the index grows 
+        // 1. The header
+        // 2. The data_level_0
+        // 3. length_memory_
+        // 4. linkLists
+
+        if(!persist_on_write_){
+            throw std::runtime_error("initPersistentIndex called for an index that is not set to persist on write");
+        }
+
+        // Create the file handles for initial write
+        std::ofstream output_header(this->getHeaderLocation(), std::ios::binary);
+        std::ofstream output_data_level0(this->getDataLevel0Location(), std::ios::binary);
+        std::ofstream output_length(this->getLengthLocation(), std::ios::binary);
+        std::ofstream output_link_lists(this->getLinkListLocation(), std::ios::binary);
+
+        // Write header
+        persistHeader(output_header);
+
+        // Write data_level0
+        output_data_level0.seekp(0, std::ios::beg);
+        output_data_level0.write(data_level0_memory_, max_elements_ * size_data_per_element_);
+        output_data_level0.flush();
+
+        // Write lengths
+        output_length.seekp(0, std::ios::beg);
+        output_length.write(length_memory_, max_elements_ * sizeof(float));
+        output_length.flush();
+
+        // Close file handles
+        output_header.close();
+        output_data_level0.close();
+        output_length.close();
+        output_link_lists.close();
+
+        // Create file handles for further writing
+        setupPersistentIndexFileHandles();
+    }
+
+    void persistHeader(std::ofstream &output_header) {
+        if (!persist_on_write_){
+            throw std::runtime_error("persistHeader called for an index that is not set to persist on write");
+        }
+
+        output_header.seekp(0, std::ios::beg);
+        writeBinaryPOD(output_header, PERSISTENCE_VERSION);
+        writeBinaryPOD(output_header, offsetLevel0_);
+        writeBinaryPOD(output_header, max_elements_);
+        writeBinaryPOD(output_header, cur_element_count); // needs to be updated
+        writeBinaryPOD(output_header, size_data_per_element_);
+        writeBinaryPOD(output_header, label_offset_);
+        writeBinaryPOD(output_header, offsetData_);
+        writeBinaryPOD(output_header, maxlevel_); // needs to be updated
+        writeBinaryPOD(output_header, enterpoint_node_); // does this need to be updated?
+        writeBinaryPOD(output_header, maxM_);
+
+        writeBinaryPOD(output_header, maxM0_);
+        writeBinaryPOD(output_header, M_);
+        writeBinaryPOD(output_header, mult_); // does this need to be updated?
+        writeBinaryPOD(output_header, ef_construction_);
+
+        output_header.flush();
+    }
+
+    // Persistence functions
+    void persistDirty() {
+        if (elements_to_persist_.size() == 0) {
+            return;
+        }
+
+        if (!persist_on_write_){
+            throw std::runtime_error("persistDirty called for an index that is not set to persist on write");
+        }
+        
+        persistHeader(this->output_header_);
+
+        // Note: We could benefit a lot from async IO here. Either via classic POSIX AIO or via libaio
+        // Generally, this storage scheme is a bit naive, and we could do a lot better in terms of disk access patterns
+        this->output_data_level0_.seekp(0, std::ios::beg);
+        for (const auto& id : elements_to_persist_) {
+            // Write the _data_level0_memory
+            // Each element is stored in a contiguous block of size_data_per_element_
+            // Where each element is the the size of llist, the llist, the data, and the label
+            this->output_data_level0_.seekp(id * size_data_per_element_, this->output_data_level0_.beg);
+            this->output_data_level0_.write(data_level0_memory_ + id * size_data_per_element_, size_data_per_element_);
+        }
+        this->output_data_level0_.flush();
+
+        // Write the dirty lengths
+        this->output_length_.seekp(0, std::ios::beg);
+        for (const auto& id : elements_to_persist_) {
+            // Write the _length_memory
+            this->output_length_.seekp(id * sizeof(float), this->output_length_.beg);
+            writeBinaryPOD(this->output_length_, ((float*)length_memory_)[id]);
+        }
+        this->output_length_.flush();
+
+        // Write the dirty link lists
+        this->output_link_lists_.seekp(0, std::ios::beg);
+        auto dirty_elements_iter = elements_to_persist_.begin();
+        // TODO: don't need to iterate over potentially all elements, could store it or memoize
+        for (size_t i = 0; i < cur_element_count && dirty_elements_iter != elements_to_persist_.end(); i++) {
+            unsigned int linkListSize = element_levels_[i] > 0 ? size_links_per_element_ * element_levels_[i] : 0;
+            if (i == *dirty_elements_iter) {
+                writeBinaryPOD(this->output_link_lists_, linkListSize);
+                if (linkListSize)
+                    this->output_link_lists_.write(linkLists_[i], linkListSize);
+                dirty_elements_iter = std::next(dirty_elements_iter);
+            } else {
+                this->output_link_lists_.seekp(linkListSize + sizeof(unsigned int), this->output_link_lists_.cur);
+            }
+        }
+        this->output_link_lists_.flush();
+
+        // Note: It would make sense to do a fsync here
+        elements_to_persist_.clear();
+    }
+
+    void loadPersistedIndex(SpaceInterface<dist_t> *s, size_t max_elements_i = 0){
+        std::ifstream input_header(this->getHeaderLocation(), std::ios::binary);
+        if (!input_header.is_open())
+            throw std::runtime_error("Cannot open header file");
+
+        // Read the header
+        int persisted_version;
+        readBinaryPOD(input_header, persisted_version);
+        // For now, version is a simple equality check, we may add backwards compatibility later
+        if (persisted_version != PERSISTENCE_VERSION)
+            throw std::runtime_error("Cannot read persisted index: wrong persistence version");
+        
+        readBinaryPOD(input_header, offsetLevel0_);
+        readBinaryPOD(input_header, max_elements_);
+        readBinaryPOD(input_header, cur_element_count);
+
+        size_t max_elements = max_elements_i;
+        if (max_elements < cur_element_count)
+            max_elements = max_elements_;
+        max_elements_ = max_elements;
+        readBinaryPOD(input_header, size_data_per_element_);
+        readBinaryPOD(input_header, label_offset_);
+        readBinaryPOD(input_header, offsetData_);
+        readBinaryPOD(input_header, maxlevel_);
+        readBinaryPOD(input_header, enterpoint_node_);
+
+        readBinaryPOD(input_header, maxM_);
+        readBinaryPOD(input_header, maxM0_);
+        readBinaryPOD(input_header, M_);
+        readBinaryPOD(input_header, mult_);
+        readBinaryPOD(input_header, ef_construction_);
+        input_header.close();
+
+        data_size_ = s->get_data_size();
+        fstdistfunc_ = s->get_dist_func();
+        dist_func_param_ = s->get_dist_func_param();
+
+
+        // Read data_level0_memory_
+        std::ifstream input_data_level0(this->getDataLevel0Location(), std::ios::binary);
+        if (!input_data_level0.is_open())
+            throw std::runtime_error("Cannot open data_level0 file");
+
+        data_level0_memory_ = (char *) malloc(max_elements * size_data_per_element_);
+        if (data_level0_memory_ == nullptr)
+            throw std::runtime_error("Not enough memory: loadPersistedIndex failed to allocate level0");
+        input_data_level0.read(data_level0_memory_, max_elements * size_data_per_element_);
+        input_data_level0.close();
+
+        // Read length_memory_
+        std::ifstream input_length(this->getLengthLocation(), std::ios::binary);
+        if (!input_length.is_open())
+            throw std::runtime_error("Cannot open length file");
+
+        length_memory_ =  (char *) malloc(max_elements * sizeof(float));
+        if (length_memory_ == nullptr)
+            throw std::runtime_error("Not enough memory: loadPersistedIndex failed to allocate length_memory_");
+        input_length.read(length_memory_, max_elements * sizeof(float));
+        input_length.close();
+
+        // Read the linkLists
+        std::ifstream input_link_list(this->getLinkListLocation(), std::ios::binary);
+        if (!input_link_list.is_open())
+            throw std::runtime_error("Cannot open link list file");
+        loadLinkLists(input_link_list);
+        input_link_list.close();
+
+        loadDeleted();
+
+        setupPersistentIndexFileHandles();
+        return;
+    }
+    // #pragma endregion
+
+    void loadLinkLists(std::ifstream& input_link_list) {
+        // Init link lists / visited lists pool
+        size_links_per_element_ = maxM_ * sizeof(tableint) + sizeof(linklistsizeint);
+        size_links_level0_ = maxM0_ * sizeof(tableint) + sizeof(linklistsizeint);
+
+        std::vector<std::mutex>(max_elements_).swap(link_list_locks_);
+        std::vector<std::mutex>(MAX_LABEL_OPERATION_LOCKS).swap(label_op_locks_);
+
+        visited_list_pool_ = new VisitedListPool(1, max_elements_);
+
+        linkLists_ = (char **) malloc(sizeof(void *) * max_elements_);
+        if (linkLists_ == nullptr)
+            throw std::runtime_error("Not enough memory: loadPersistedIndex failed to allocate linklists");
+        element_levels_ = std::vector<int>(max_elements_);
+        revSize_ = 1.0 / mult_;
+        ef_ = 10;
+        for (size_t i = 0; i < cur_element_count; i++) {
+            label_lookup_[getExternalLabel(i)] = i;
+            unsigned int linkListSize;
+            readBinaryPOD(input_link_list, linkListSize);
+            if (linkListSize == 0) {
+                element_levels_[i] = 0;
+                linkLists_[i] = nullptr;
+            } else {
+                element_levels_[i] = linkListSize / size_links_per_element_;
+                linkLists_[i] = (char *) malloc(linkListSize);
+                if (linkLists_[i] == nullptr)
+                    throw std::runtime_error("Not enough memory: loadIndex failed to allocate linklist");
+                input_link_list.read(linkLists_[i], linkListSize);
+            }
+        }
+    }
+
+    void loadDeleted(){
+         for (size_t i = 0; i < cur_element_count; i++) {
+            if (isMarkedDeleted(i)) {
+                num_deleted_ += 1;
+                if (allow_replace_deleted_) deleted_elements.insert(i);
+            }
+        }
+    }
 
     void loadIndex(const std::string &location, SpaceInterface<dist_t> *s, size_t max_elements_i = 0) {
         std::ifstream input(location, std::ios::binary);
 
         if (!input.is_open())
             throw std::runtime_error("Cannot open file");
 
@@ -723,50 +1048,16 @@
         input.read(data_level0_memory_, cur_element_count * size_data_per_element_);
 
         length_memory_ =  (char *) malloc(max_elements * sizeof(float));
         if (length_memory_ == nullptr)
             throw std::runtime_error("Not enough memory: loadIndex failed to allocate length_memory_");
         input.read(length_memory_, cur_element_count * sizeof(float));
 
-        size_links_per_element_ = maxM_ * sizeof(tableint) + sizeof(linklistsizeint);
-
-        size_links_level0_ = maxM0_ * sizeof(tableint) + sizeof(linklistsizeint);
-        std::vector<std::mutex>(max_elements).swap(link_list_locks_);
-        std::vector<std::mutex>(MAX_LABEL_OPERATION_LOCKS).swap(label_op_locks_);
-
-        visited_list_pool_ = new VisitedListPool(1, max_elements);
-
-        linkLists_ = (char **) malloc(sizeof(void *) * max_elements);
-        if (linkLists_ == nullptr)
-            throw std::runtime_error("Not enough memory: loadIndex failed to allocate linklists");
-        element_levels_ = std::vector<int>(max_elements);
-        revSize_ = 1.0 / mult_;
-        ef_ = 10;
-        for (size_t i = 0; i < cur_element_count; i++) {
-            label_lookup_[getExternalLabel(i)] = i;
-            unsigned int linkListSize;
-            readBinaryPOD(input, linkListSize);
-            if (linkListSize == 0) {
-                element_levels_[i] = 0;
-                linkLists_[i] = nullptr;
-            } else {
-                element_levels_[i] = linkListSize / size_links_per_element_;
-                linkLists_[i] = (char *) malloc(linkListSize);
-                if (linkLists_[i] == nullptr)
-                    throw std::runtime_error("Not enough memory: loadIndex failed to allocate linklist");
-                input.read(linkLists_[i], linkListSize);
-            }
-        }
-
-        for (size_t i = 0; i < cur_element_count; i++) {
-            if (isMarkedDeleted(i)) {
-                num_deleted_ += 1;
-                if (allow_replace_deleted_) deleted_elements.insert(i);
-            }
-        }
+        loadLinkLists(input);
+        loadDeleted();
 
         input.close();
 
         return;
     }
 
 
@@ -815,14 +1106,15 @@
         if (search == label_lookup_.end()) {
             throw std::runtime_error("Label not found");
         }
         tableint internalId = search->second;
         lock_table.unlock();
 
         markDeletedInternal(internalId);
+        markElementToPersist(internalId);
     }
 
 
     /*
     * Uses the last 16 bits of the memory for the linked list size to store the mark,
     * whereas maxM0_ has to be limited to the lower 16 bits, however, still large enough in almost all cases.
     */
@@ -857,14 +1149,15 @@
         if (search == label_lookup_.end()) {
             throw std::runtime_error("Label not found");
         }
         tableint internalId = search->second;
         lock_table.unlock();
 
         unmarkDeletedInternal(internalId);
+        markElementToPersist(internalId);
     }
 
 
 
     /*
     * Remove the deleted mark of the node.
     */
@@ -1252,15 +1545,14 @@
         dist_t curdist = fstdistfunc_(query_data, getDataByInternalId(enterpoint_node_), dist_func_param_);
 
         for (int level = maxlevel_; level > 0; level--) {
             bool changed = true;
             while (changed) {
                 changed = false;
                 unsigned int *data;
-
                 data = (unsigned int *) get_linklist(currObj, level);
                 int size = getListCount(data);
                 metric_hops++;
                 metric_distance_computations+=size;
 
                 tableint *datal = (tableint *) (data + 1);
                 for (int i = 0; i < size; i++) {
```

### Comparing `chroma-hnswlib-0.7.0/hnswlib/hnswlib.h` & `chroma-hnswlib-0.7.1/hnswlib/hnswlib.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.0/hnswlib/space_ip.h` & `chroma-hnswlib-0.7.1/hnswlib/space_ip.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.0/hnswlib/space_l2.h` & `chroma-hnswlib-0.7.1/hnswlib/space_l2.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.0/hnswlib/visited_list_pool.h` & `chroma-hnswlib-0.7.1/hnswlib/visited_list_pool.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.0/python_bindings/bindings.cpp` & `chroma-hnswlib-0.7.1/python_bindings/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -190,20 +190,22 @@
 
 
     void init_new_index(
         size_t maxElements,
         size_t M,
         size_t efConstruction,
         size_t random_seed,
-        bool allow_replace_deleted) {
+        bool allow_replace_deleted,
+        bool is_persistent_index,
+        std::string persistence_location) {
         if (appr_alg) {
             throw std::runtime_error("The index is already initiated.");
         }
         cur_l = 0;
-        appr_alg = new hnswlib::HierarchicalNSW<dist_t>(l2space, maxElements, M, efConstruction, random_seed, allow_replace_deleted, normalize);
+        appr_alg = new hnswlib::HierarchicalNSW<dist_t>(l2space, maxElements, M, efConstruction, random_seed, allow_replace_deleted, normalize, is_persistent_index, persistence_location);
         index_inited = true;
         ep_added = false;
         appr_alg->ef_ = default_ef;
         seed = random_seed;
     }
 
 
@@ -220,24 +222,27 @@
 
 
     void saveIndex(const std::string &path_to_index) {
         appr_alg->saveIndex(path_to_index);
     }
 
 
-    void loadIndex(const std::string &path_to_index, size_t max_elements, bool allow_replace_deleted) {
+    void loadIndex(const std::string &path_to_index, size_t max_elements, bool allow_replace_deleted, bool is_persistent_index) {
       if (appr_alg) {
           std::cerr << "Warning: Calling load_index for an already inited index. Old index is being deallocated." << std::endl;
           delete appr_alg;
       }
-      appr_alg = new hnswlib::HierarchicalNSW<dist_t>(l2space, path_to_index, false, max_elements, allow_replace_deleted, normalize);
+      appr_alg = new hnswlib::HierarchicalNSW<dist_t>(l2space, path_to_index, false, max_elements, allow_replace_deleted, normalize, is_persistent_index);
       cur_l = appr_alg->cur_element_count;
       index_inited = true;
     }
 
+    void persistDirty() {
+        appr_alg->persistDirty();
+    }
 
     void normalize_vector(float* data, float* norm_array) {
         float norm = 0.0f;
         for (int i = 0; i < dim; i++)
             norm += data[i] * data[i];
         norm = 1.0f / (sqrtf(norm) + 1e-30f);
         for (int i = 0; i < dim; i++)
@@ -871,15 +876,17 @@
         .def(py::init<const std::string &, const int>(), py::arg("space"), py::arg("dim"))
         .def("init_index",
             &Index<float>::init_new_index,
             py::arg("max_elements"),
             py::arg("M") = 16,
             py::arg("ef_construction") = 200,
             py::arg("random_seed") = 100,
-            py::arg("allow_replace_deleted") = false)
+            py::arg("allow_replace_deleted") = false,
+            py::arg("is_persistent_index") = false,
+            py::arg("persistence_location") = "./")
         .def("knn_query",
             &Index<float>::knnQuery_return_numpy,
             py::arg("data"),
             py::arg("k") = 1,
             py::arg("num_threads") = -1,
             py::arg("filter") = py::none())
         .def("add_items",
@@ -893,15 +900,17 @@
         .def("set_ef", &Index<float>::set_ef, py::arg("ef"))
         .def("set_num_threads", &Index<float>::set_num_threads, py::arg("num_threads"))
         .def("save_index", &Index<float>::saveIndex, py::arg("path_to_index"))
         .def("load_index",
             &Index<float>::loadIndex,
             py::arg("path_to_index"),
             py::arg("max_elements") = 0,
-            py::arg("allow_replace_deleted") = false)
+            py::arg("allow_replace_deleted") = false,
+            py::arg("is_persistent_index") = false)
+        .def("persist_dirty", &Index<float>::persistDirty)
         .def("mark_deleted", &Index<float>::markDeleted, py::arg("label"))
         .def("unmark_deleted", &Index<float>::unmarkDeleted, py::arg("label"))
         .def("resize_index", &Index<float>::resizeIndex, py::arg("new_size"))
         .def("get_max_elements", &Index<float>::getMaxElements)
         .def("get_current_count", &Index<float>::getCurrentCount)
         .def_readonly("space", &Index<float>::space_name)
         .def_readonly("dim", &Index<float>::dim)
```

### Comparing `chroma-hnswlib-0.7.0/setup.py` & `chroma-hnswlib-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import pybind11
 import setuptools
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 
 include_dirs = [
     pybind11.get_include(),
     np.get_include(),
 ]
```

