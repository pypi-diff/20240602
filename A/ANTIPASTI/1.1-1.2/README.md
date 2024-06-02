# Comparing `tmp/ANTIPASTI-1.1.tar.gz` & `tmp/antipasti-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANTIPASTI-1.1.tar", last modified: Mon Jan 22 14:49:33 2024, max compression
+gzip compressed data, was "antipasti-1.2.tar", last modified: Sun Jun  2 16:25:42 2024, max compression
```

## Comparing `ANTIPASTI-1.1.tar` & `antipasti-1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-01-22 14:49:33.874645 ANTIPASTI-1.1/
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-01-22 14:49:33.874145 ANTIPASTI-1.1/ANTIPASTI.egg-info/
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4151 2024-01-22 14:49:33.000000 ANTIPASTI-1.1/ANTIPASTI.egg-info/PKG-INFO
--rw-r--r--   0 kevinmicha   (501) staff       (20)      534 2024-01-22 14:49:33.000000 ANTIPASTI-1.1/ANTIPASTI.egg-info/SOURCES.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)        1 2024-01-22 14:49:33.000000 ANTIPASTI-1.1/ANTIPASTI.egg-info/dependency_links.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)      131 2024-01-22 14:49:33.000000 ANTIPASTI-1.1/ANTIPASTI.egg-info/requires.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)       10 2024-01-22 14:49:33.000000 ANTIPASTI-1.1/ANTIPASTI.egg-info/top_level.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)      618 2023-12-08 15:45:41.000000 ANTIPASTI-1.1/AUTHORS.md
--rw-r--r--   0 kevinmicha   (501) staff       (20)     1074 2023-01-26 16:59:11.000000 ANTIPASTI-1.1/LICENSE
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4151 2024-01-22 14:49:33.874425 ANTIPASTI-1.1/PKG-INFO
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3496 2024-01-22 14:37:43.000000 ANTIPASTI-1.1/README.md
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-01-22 14:49:33.870373 ANTIPASTI-1.1/antipasti/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      347 2023-05-16 11:55:02.000000 ANTIPASTI-1.1/antipasti/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)      487 2023-05-02 16:30:11.000000 ANTIPASTI-1.1/antipasti/config.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-01-22 14:49:33.870937 ANTIPASTI-1.1/antipasti/model/
--rw-r--r--   0 kevinmicha   (501) staff       (20)       72 2023-04-28 09:46:56.000000 ANTIPASTI-1.1/antipasti/model/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     2490 2024-01-20 21:10:57.000000 ANTIPASTI-1.1/antipasti/model/model.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-01-22 14:49:33.871537 ANTIPASTI-1.1/antipasti/preprocessing/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      100 2023-04-28 09:47:02.000000 ANTIPASTI-1.1/antipasti/preprocessing/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    25771 2024-01-22 12:51:10.000000 ANTIPASTI-1.1/antipasti/preprocessing/preprocessing.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-01-22 14:49:33.873668 ANTIPASTI-1.1/antipasti/utils/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      134 2023-06-30 10:16:40.000000 ANTIPASTI-1.1/antipasti/utils/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4500 2023-12-12 18:18:23.000000 ANTIPASTI-1.1/antipasti/utils/biology_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    31229 2023-12-12 18:33:06.000000 ANTIPASTI-1.1/antipasti/utils/explaining_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)      268 2023-08-04 09:42:12.000000 ANTIPASTI-1.1/antipasti/utils/generic_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    10922 2024-01-22 12:51:27.000000 ANTIPASTI-1.1/antipasti/utils/torch_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)       38 2024-01-22 14:49:33.874692 ANTIPASTI-1.1/setup.cfg
--rw-r--r--   0 kevinmicha   (501) staff       (20)     1215 2024-01-22 14:42:15.000000 ANTIPASTI-1.1/setup.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-06-02 16:25:42.224268 antipasti-1.2/
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-06-02 16:25:42.223898 antipasti-1.2/ANTIPASTI.egg-info/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4213 2024-06-02 16:25:42.000000 antipasti-1.2/ANTIPASTI.egg-info/PKG-INFO
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      534 2024-06-02 16:25:42.000000 antipasti-1.2/ANTIPASTI.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)        1 2024-06-02 16:25:42.000000 antipasti-1.2/ANTIPASTI.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      131 2024-06-02 16:25:42.000000 antipasti-1.2/ANTIPASTI.egg-info/requires.txt
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)       10 2024-06-02 16:25:42.000000 antipasti-1.2/ANTIPASTI.egg-info/top_level.txt
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      618 2023-12-08 15:45:41.000000 antipasti-1.2/AUTHORS.md
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)     1074 2023-01-26 16:59:11.000000 antipasti-1.2/LICENSE
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4213 2024-06-02 16:25:42.224102 antipasti-1.2/PKG-INFO
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)     3558 2024-05-27 17:07:28.000000 antipasti-1.2/README.md
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-06-02 16:25:42.220508 antipasti-1.2/antipasti/
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      347 2023-05-16 11:55:02.000000 antipasti-1.2/antipasti/__init__.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      487 2024-02-11 17:26:50.000000 antipasti-1.2/antipasti/config.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-06-02 16:25:42.221111 antipasti-1.2/antipasti/model/
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)       72 2023-04-28 09:46:56.000000 antipasti-1.2/antipasti/model/__init__.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)     2492 2024-03-26 12:23:49.000000 antipasti-1.2/antipasti/model/model.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-06-02 16:25:42.221542 antipasti-1.2/antipasti/preprocessing/
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      100 2023-04-28 09:47:02.000000 antipasti-1.2/antipasti/preprocessing/__init__.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)    27994 2024-05-27 17:38:01.000000 antipasti-1.2/antipasti/preprocessing/preprocessing.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2024-06-02 16:25:42.223459 antipasti-1.2/antipasti/utils/
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      134 2023-06-30 10:16:40.000000 antipasti-1.2/antipasti/utils/__init__.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)     9819 2024-05-27 18:20:10.000000 antipasti-1.2/antipasti/utils/biology_utils.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)    32016 2024-05-27 16:36:15.000000 antipasti-1.2/antipasti/utils/explaining_utils.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)      268 2023-08-04 09:42:12.000000 antipasti-1.2/antipasti/utils/generic_utils.py
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)    12488 2024-05-27 16:18:51.000000 antipasti-1.2/antipasti/utils/torch_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)       38 2024-06-02 16:25:42.224317 antipasti-1.2/setup.cfg
+-rwxrwxrwx   0 kevinmicha   (501) staff       (20)     1215 2024-06-02 16:18:05.000000 antipasti-1.2/setup.py
```

### Comparing `ANTIPASTI-1.1/ANTIPASTI.egg-info/PKG-INFO` & `antipasti-1.2/ANTIPASTI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANTIPASTI
-Version: 1.1
+Version: 1.2
 Summary: Deep Learning model that predicts the binding affinity of antibodies from their three-dimensional structure.
 Author: Kevin Michalewicz
 Author-email: k.michalewicz22@imperial.ac.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: adabelief-pytorch
@@ -94,12 +94,12 @@
 
 Example notebooks are located in the [notebooks](https://github.com/kevinmicha/ANTIPASTI/tree/main/notebooks) folder:
 * [[Tutorial] Training ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Training%20ANTIPASTI.ipynb)
 * [[Tutorial] Predicting affinity using ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Predicting%20affinity%20using%20ANTIPASTI.ipynb)
 * [[Tutorial] Explaining binding affinity with ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Explaining%20binding%20affinity%20with%20ANTIPASTI.ipynb)
 * [[Tutorial] Combining AlphaFold and ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Combining%20AlphaFold%20and%20ANTIPASTI.ipynb)
 
-You can download the data used for the paper [here](https://drive.google.com/drive/folders/1E8-GwQq9GHBE0A6r2t8dblAzP7qf0seQ?usp=sharing) and place it in `data/cov_maps_full_ags_all`.
+You can download normal mode correlation maps computed at atomistic scale (instead of residue scale) [here](https://drive.google.com/drive/folders/1E8-GwQq9GHBE0A6r2t8dblAzP7qf0seQ?usp=sharing) and place them in `data/dccm_maps_full_ags_all_aa`.
 
 ## Attribution
 
 If you use this code, please cite the [paper](https://kevinmicha.github.io/ANTIPASTI/citing.html) indicated in the documentation.
```

### Comparing `ANTIPASTI-1.1/ANTIPASTI.egg-info/SOURCES.txt` & `antipasti-1.2/ANTIPASTI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANTIPASTI-1.1/AUTHORS.md` & `antipasti-1.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `ANTIPASTI-1.1/LICENSE` & `antipasti-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ANTIPASTI-1.1/PKG-INFO` & `antipasti-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANTIPASTI
-Version: 1.1
+Version: 1.2
 Summary: Deep Learning model that predicts the binding affinity of antibodies from their three-dimensional structure.
 Author: Kevin Michalewicz
 Author-email: k.michalewicz22@imperial.ac.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: adabelief-pytorch
@@ -94,12 +94,12 @@
 
 Example notebooks are located in the [notebooks](https://github.com/kevinmicha/ANTIPASTI/tree/main/notebooks) folder:
 * [[Tutorial] Training ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Training%20ANTIPASTI.ipynb)
 * [[Tutorial] Predicting affinity using ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Predicting%20affinity%20using%20ANTIPASTI.ipynb)
 * [[Tutorial] Explaining binding affinity with ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Explaining%20binding%20affinity%20with%20ANTIPASTI.ipynb)
 * [[Tutorial] Combining AlphaFold and ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Combining%20AlphaFold%20and%20ANTIPASTI.ipynb)
 
-You can download the data used for the paper [here](https://drive.google.com/drive/folders/1E8-GwQq9GHBE0A6r2t8dblAzP7qf0seQ?usp=sharing) and place it in `data/cov_maps_full_ags_all`.
+You can download normal mode correlation maps computed at atomistic scale (instead of residue scale) [here](https://drive.google.com/drive/folders/1E8-GwQq9GHBE0A6r2t8dblAzP7qf0seQ?usp=sharing) and place them in `data/dccm_maps_full_ags_all_aa`.
 
 ## Attribution
 
 If you use this code, please cite the [paper](https://kevinmicha.github.io/ANTIPASTI/citing.html) indicated in the documentation.
```

### Comparing `ANTIPASTI-1.1/README.md` & `antipasti-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,12 +71,12 @@
 
 Example notebooks are located in the [notebooks](https://github.com/kevinmicha/ANTIPASTI/tree/main/notebooks) folder:
 * [[Tutorial] Training ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Training%20ANTIPASTI.ipynb)
 * [[Tutorial] Predicting affinity using ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Predicting%20affinity%20using%20ANTIPASTI.ipynb)
 * [[Tutorial] Explaining binding affinity with ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Explaining%20binding%20affinity%20with%20ANTIPASTI.ipynb)
 * [[Tutorial] Combining AlphaFold and ANTIPASTI](https://github.com/kevinmicha/ANTIPASTI/blob/main/notebooks/%5BTutorial%5D%20Combining%20AlphaFold%20and%20ANTIPASTI.ipynb)
 
-You can download the data used for the paper [here](https://drive.google.com/drive/folders/1E8-GwQq9GHBE0A6r2t8dblAzP7qf0seQ?usp=sharing) and place it in `data/cov_maps_full_ags_all`.
+You can download normal mode correlation maps computed at atomistic scale (instead of residue scale) [here](https://drive.google.com/drive/folders/1E8-GwQq9GHBE0A6r2t8dblAzP7qf0seQ?usp=sharing) and place them in `data/dccm_maps_full_ags_all_aa`.
 
 ## Attribution
 
 If you use this code, please cite the [paper](https://kevinmicha.github.io/ANTIPASTI/citing.html) indicated in the documentation.
```

### Comparing `ANTIPASTI-1.1/antipasti/model/model.py` & `antipasti-1.2/antipasti/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.filter_size = filter_size
         self.pooling_size = pooling_size
         self.input_shape = input_shape
         self.mode = mode
         if self.mode == 'full':
             self.fully_connected_input = n_filters * ((input_shape-filter_size+1)//pooling_size) ** 2
             self.conv1 = Conv2d(1, n_filters, filter_size)
-            self.pool = MaxPool2d(pooling_size, pooling_size)
+            self.pool = MaxPool2d((pooling_size, pooling_size))
             self.relu = ReLU()
         else:
             self.fully_connected_input = self.input_shape ** 2
         self.fc1 = Linear(self.fully_connected_input, 1, bias=False)
         self.l1_lambda = l1_lambda
 
     def forward(self, x):
```

### Comparing `ANTIPASTI-1.1/antipasti/preprocessing/preprocessing.py` & `antipasti-1.2/antipasti/preprocessing/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,26 +179,33 @@
             The names of each residue are stored in ``self.residues_path``.
         upsymchain: int
             Upper limit of heavy chain residues due to a change in the numbering convention. Only useful when using ``AlphaFold``.
         lupsymchain: int
             Upper limit of light chain residues due to a change in the numbering convention. Only useful when using ``AlphaFold``.
 
         """
+
+        amino_acid_dictionary = {'CYS': 'C', 'ASP': 'D', 'SER': 'S', 'GLN': 'Q', 'LYS': 'K',
+        'ILE': 'I', 'PRO': 'P', 'THR': 'T', 'PHE': 'F', 'ASN': 'N', 'GLY': 'G', 'HIS': 'H', 
+        'LEU': 'L', 'ARG': 'R', 'TRP': 'W', 'ALA': 'A', 'VAL':'V', 'GLU': 'E', 'TYR': 'Y', 'MET': 'M'}
+
+
         if self.stage == 'training':
             rpath = self.residues_path
         else:
             rpath = self.test_residues_path
-        list_residues = ['START']
+        list_residues = ['START-Ab']
 
         with open(path, 'r') as f: # needs to be Chothia-numbered
             content = f.readlines()
             header_lines_important = range(4)
             header_lines = [content[i][0]=='R' for i in range(len(content))].count(True)
             h_range = range(1, 114)
             l_range = range(1, 108)
+            residue_type_range = slice(17, 20)
             start_chain = 21
             chain_range = slice(start_chain, start_chain+1)
             res_range = slice(23, 26)
             res_extra_letter = 26 #sometimes includes a letter 'A', 'B', 'C', ...
             h_chain_key = 'HCHAIN'
             l_chain_key = 'LCHAIN'
             antigen_chain_key = 'AGCHAIN'
@@ -268,14 +275,15 @@
                         idx_list.append(i+header_lines)
                         if lresidues == True:
                             full_res = line[res_range] + line[res_extra_letter]
                             if pathologic:
                                 full_res = new_hchain + full_res
                             else:
                                 full_res = line[chain_range] + full_res
+                            full_res = amino_acid_dictionary[line[residue_type_range]] + full_res
                             if full_res != list_residues[-1]:
                                 list_residues.append(full_res)
 
             # This separation ensures that heavy chain residues are enlisted first
             if l_chain is not None:
                 for i, line in enumerate(content[header_lines:]):
                     if line[chain_range].find(l_chain) != -1 and int(line[res_range]) in l_range:
@@ -283,25 +291,33 @@
                             idx_list_l.append(i+header_lines)
                             if lresidues == True:
                                 full_res = line[res_range] + line[res_extra_letter]
                                 if pathologic:
                                     full_res = new_lchain + full_res
                                 else:
                                     full_res = line[chain_range] + full_res
+                                full_res = amino_acid_dictionary[line[residue_type_range]] + full_res
                                 if full_res != list_residues[-1]:
                                     list_residues.append(full_res)                   
         
+            if lresidues == True:
+                list_residues.append('END-Ab')
+
             # Obtaining antigen(s)
             for i, line in enumerate(content[header_lines:]):
                 if any(line[chain_range] in agc for agc in antigen_chains) and h_chain not in antigen_chains and l_chain not in antigen_chains:
                     idx_list_antigen.append(i+header_lines)
+                    if lresidues == True:
+                        full_res = line[chain_range] + line[res_range] + line[res_extra_letter]
+                        if line[residue_type_range] in amino_acid_dictionary:
+                            full_res = amino_acid_dictionary[line[residue_type_range]] + full_res
+                            if full_res != list_residues[-1]:
+                                list_residues.append(full_res)    
 
         # List with name of every residue is saved if selected
-        if lresidues == True:
-            list_residues.append('END')
             saving_path = rpath + path[-8:-4] + '.npy'
             #if not os.path.exists(saving_path):
             np.save(saving_path, list_residues)
             
         # Creating new file
         with open(new_path, 'w') as f_new:
             f_new.writelines([content[l] for l in idx_list[:header_lines_important[-1]]])
@@ -322,16 +338,19 @@
 
         """
         for i, entry in enumerate(self.entries):
             file_name = entry + self.selection
             path = self.structures_path + file_name + self.file_type_input
             new_path = self.dccm_map_path + entry
             self.generate_fv_pdb(self.structures_path+entry+self.file_type_input, lresidues=True) 
-            if not self.cmaps:
+            if not self.cmaps: # and len(np.load(self.residues_path + path[-11:-7] + '.npy')) > 500:
                 subprocess.call(['/usr/local/bin/RScript', str(self.scripts_path)+'pdb_to_dccm.r', str(path), str(new_path), str(self.modes)], shell=True, stdout=open(os.devnull, 'wb'))
+            #elif not self.cmaps:
+            #    print(path[-11:-7])
+            #    subprocess.call(['/usr/local/bin/RScript', str(self.scripts_path)+'pdb_to_dccm_aa.r', str(path), str(new_path), str(self.modes)], stdout=open(os.devnull, 'wb'))
             else:
                 subprocess.call(['python', str(self.scripts_path)+'generate_contact_maps.py', str(path), str(new_path), str(self.cmaps_thr)], stdout=open(os.devnull, 'wb'))
             if os.path.exists(path):
                 os.remove(path)
             
             if i % 25 == 0: 
                 print('Map ' + str(i+1) + ' out of ' + str(len(self.entries)) + ' processed.')
@@ -359,56 +378,69 @@
 
         if self.stage == 'training':
             rpath = self.residues_path
         else:
             rpath = self.test_residues_path
 
         for entry in selected_entries:
-            list_of_residues = np.load(rpath+entry+'.npy')[1:-1]
-            h_chain = list_of_residues[0][0]
-            l_chain = list_of_residues[-1][0]
+            list_of_residues = list(np.load(rpath+entry+'.npy'))[1:]
+            chain_pos = 0
+            if 'END-Ab' in list_of_residues:
+                list_of_residues = list_of_residues[:list_of_residues.index('END-Ab')]
+                chain_pos = 1
+            else:
+                list_of_residues = list_of_residues[:-1]
 
-            heavy.append(len([idx for idx in list_of_residues if idx[0] == h_chain]))
+            h_chain = list_of_residues[0][chain_pos]
+            l_chain = list_of_residues[-1][chain_pos]
+
+            heavy.append(len([idx for idx in list_of_residues if idx[chain_pos] == h_chain]))
             if h_chain != l_chain:
-                light.append(len([idx for idx in list_of_residues if idx[0] == l_chain]))
+                light.append(len([idx for idx in list_of_residues if idx[chain_pos] == l_chain]))
             else:
                 light.append(0)
 
         return heavy, light, selected_entries
 
     def get_max_min_chains(self):
         r"""Returns the longest and shortest possible chains.
 
         """
         max_res_list_h = []
         max_res_list_l = []
 
         for f in self.file_residues_paths:
+            shift = 0
+            if 'END-Ab' in np.load(f):
+                shift = 1
             idx = self.selected_entries.index(f[-8:-4])
             current_list_h = np.load(f)[1:self.heavy[idx]+1]
             current_list_l = np.load(f)[self.heavy[idx]+1:self.heavy[idx]+self.light[idx]+1]
-            current_list_h = [x[1:] for x in current_list_h]
-            current_list_l = [x[1:] for x in current_list_l]
+            current_list_h = [x[1+shift:] for x in current_list_h]
+            current_list_l = [x[1+shift:] for x in current_list_l]
             max_res_list_h += list(set(current_list_h).difference(max_res_list_h))
             max_res_list_l += list(set(current_list_l).difference(max_res_list_l))
             
         max_res_list_h = sorted(max_res_list_h, key=remove_abc)
         min_res_list_h = list(dict.fromkeys([x for x in max_res_list_h]))
         max_res_list_h = [x.strip() for x in max_res_list_h]
 
         max_res_list_l = sorted(max_res_list_l, key=remove_abc)
         min_res_list_l = list(dict.fromkeys([x for x in max_res_list_l]))
         max_res_list_l = [x.strip() for x in max_res_list_l]
 
         for f in self.file_residues_paths:
+            shift = 0
+            if 'END-Ab' in f:
+                shift = 1
             idx = self.selected_entries.index(f[-8:-4])
             current_list_h = np.load(f)[1:self.heavy[idx]+1]
             current_list_l = np.load(f)[self.heavy[idx]+1:self.heavy[idx]+self.light[idx]+1]
-            current_list_h = [x[1:] for x in current_list_h]
-            current_list_l = [x[1:] for x in current_list_l]
+            current_list_h = [x[1+shift:] for x in current_list_h]
+            current_list_l = [x[1+shift:] for x in current_list_l]
             min_res_list_h = sorted(list(set(current_list_h).intersection(min_res_list_h)))
             min_res_list_l = sorted(list(set(current_list_l).intersection(min_res_list_l)))
 
         min_res_list_h = [x.strip() for x in min_res_list_h]
         min_res_list_l = [x.strip() for x in min_res_list_l]
 
         return max_res_list_h, max_res_list_l, min_res_list_h, min_res_list_l
@@ -449,15 +481,17 @@
         else:
             heavy = np.load(self.chain_lengths_path+'heavy_lengths.npy').astype(int)
             light = np.load(self.chain_lengths_path+'light_lengths.npy').astype(int)
 
         assert list(np.load(self.chain_lengths_path+'selected_entries.npy')) == selected_entries
 
         for entry in selected_entries:
-            assert len(np.load(self.residues_path+entry+'.npy'))-2 == heavy[selected_entries.index(entry)] + light[selected_entries.index(entry)]
+            residues = list(np.load(self.residues_path+entry+'.npy'))
+            if 'END-Ab' in residues:
+                assert len(residues[:residues.index('END-Ab')])-1 == heavy[selected_entries.index(entry)] + light[selected_entries.index(entry)]
 
         return heavy, light, selected_entries
 
     def generate_masked_image(self, img, idx, test_h=None, test_l=None):
         r"""Generates a masked normal mode correlation map
 
         Parameters
@@ -483,14 +517,18 @@
             f = self.file_residues_paths[idx]
         elif self.alphafold is False:
             f = sorted(glob.glob(os.path.join(self.test_residues_path, '*'+self.test_pdb_id+'.npy')))[0]
         else:
             f = sorted(glob.glob(os.path.join(self.test_residues_path, '*'+self.test_pdb_id[:-3]+'.npy')))[0] # removing '_af' suffix
         antigen_max_pixels = self.ag_residues
         f_res = np.load(f)
+
+        # We force unique elements
+        self.max_res_list_h = list(dict.fromkeys(self.max_res_list_h))
+        self.max_res_list_l = list(dict.fromkeys(self.max_res_list_l))
         max_res_h = len(self.max_res_list_h)
         max_res_l = len(self.max_res_list_l)
         max_res = max_res_h + max_res_l 
         masked = np.zeros((max_res+antigen_max_pixels, max_res+antigen_max_pixels))
         mask = np.zeros((max_res+antigen_max_pixels, max_res+antigen_max_pixels))
         
         if self.stage != 'training':
@@ -498,17 +536,18 @@
             l = test_l
         else:
             current_idx = self.selected_entries.index(f[-8:-4])
             h = self.heavy[current_idx]
             l = self.light[current_idx]
 
         current_list_h = f_res[1:h+1]
-        current_list_h = [x[1:].strip() for x in current_list_h]
+        shift = len(f_res[1][:f_res[1].find(' ')])
+        current_list_h = [x[shift:].strip() for x in current_list_h] # First letter is the type of amino acid and second letter is the chain ID
         current_list_l = f_res[h+1:h+l+1]
-        current_list_l = [x[1:].strip() for x in current_list_l]    
+        current_list_l = [x[shift:].strip() for x in current_list_l]    
 
         idx_list = [i for i in range(max_res_h) if self.max_res_list_h[i] in current_list_h]
         idx_list += [i+max_res_h for i in range(max_res_l) if self.max_res_list_l[i] in current_list_l]
         idx_list += [i+max_res_h+max_res_l for i in range(min(antigen_max_pixels, img.shape[-1]-(h+l)))]
         for k, i in enumerate(idx_list):
             for l, j in enumerate(idx_list):
                 masked[i, j] = img[k, l]
```

### Comparing `ANTIPASTI-1.1/antipasti/utils/explaining_utils.py` & `antipasti-1.2/antipasti/utils/explaining_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import cv2
-import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import torch
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 import umap
@@ -69,14 +68,22 @@
 
     """
     input_shape = preprocessed_data.test_x.shape[-1]
     each_img_enl = np.zeros((preprocessed_data.train_x.shape[0], input_shape**2))
     size_le = int(np.sqrt(model.fc1.weight.data.numpy().shape[-1] / model.n_filters))
     offset = np.zeros((input_shape**2))
 
+    # Border effects
+    preprocessed_data.train_x[:,:,0] = 0
+    preprocessed_data.train_x[:,0,:] = 0
+    preprocessed_data.train_x[:,:,len(preprocessed_data.max_res_list_h)-1:len(preprocessed_data.max_res_list_h)+1] = 0
+    preprocessed_data.train_x[:,len(preprocessed_data.max_res_list_h)-1:len(preprocessed_data.max_res_list_h)+1, :] = 0
+    preprocessed_data.train_x[:,:,-1] = 0
+    preprocessed_data.train_x[:,-1,:] = 0
+
     inter_filter_off = model(torch.from_numpy(np.zeros((input_shape, input_shape)).reshape(1, 1, input_shape, input_shape).astype(np.float32)))[1].detach().numpy()
     for i in range(model.n_filters):
         offset += cv2.resize(np.multiply(inter_filter_off[0,i], model.fc1.weight.data.numpy().reshape(model.n_filters, size_le**2)[i].reshape(size_le, size_le)), dsize=(input_shape, input_shape)).reshape((input_shape**2))
 
     for j in range(preprocessed_data.train_x.shape[0]):
         inter_filter_item = model(torch.from_numpy(preprocessed_data.train_x[j].reshape(1, 1, input_shape, input_shape).astype(np.float32)))[1].detach().numpy()
         for i in range(model.n_filters):
@@ -239,16 +246,20 @@
     if scheme in db.columns:
         db = db.loc[:,['pdb', scheme]]
 
     # Obtaining the labels and the output layer representations
     for j in range(train_x.shape[0]):
         if scheme in db.columns:
             labels.append(str(db[db['pdb'] == pdb_codes[j]].iloc[-1][scheme]))
+    #         if pdb_codes[j] in nanobodies:
+    #             labels.pop()
+    #             labels.append('nanobodies')
     each_img_enl = get_output_representations(preprocessed_data, model)
-
+    # each_img_enl = each_img_enl.reshape(-1, train_x.shape[-1], train_x.shape[-1])[:, :len(preprocessed_data.max_res_list_h), :len(preprocessed_data.max_res_list_h)].reshape(-1, len(preprocessed_data.max_res_list_h)**2)
+    
     # UMAP fitting 
     scaled_each_img = StandardScaler().fit_transform(each_img_enl)
     embedding = reducer.fit_transform(scaled_each_img)
 
     if exclude_nanobodies:
         pdb_codes, _, embedding, labels, numerical_values = remove_nanobodies(pdb_codes, train_x, embedding, labels, numerical_values)
 
@@ -298,14 +309,15 @@
 
         elif scheme == 'antigen_type':
             cdict = {'protein': 0,
                 'peptide': 1,
                 'Hapten': 2,
                 'protein | protein': 3,
                 'carbohydrate': 4,
+        #       'nanobodies': 5,
                 'Other': 5}
             scheme = 'Type of antigen'
         else:
             cdict = external_cdict
 
         for i in range(len(labels)):
             if labels[i] in cdict:
@@ -323,15 +335,15 @@
                 colours.append(float(item))
             else:
                 embedding = np.delete(embedding, i-deleted_items, axis=0)
                 pdb_codes = np.delete(pdb_codes, i-deleted_items, axis=0)
                 deleted_items += 1
     plot_umap(embedding=embedding, colours=colours, scheme=scheme, pdb_codes=pdb_codes, categorical=categorical, include_ellipses=include_ellipses, cdict=cdict, interactive=interactive)
 
-    return colours, pdb_codes
+    return colours, pdb_codes, embedding
 
 
 def plot_umap(embedding, colours, scheme, pdb_codes, categorical=True, include_ellipses=False, cdict=None, interactive=False):
     r"""Plots UMAP maps.
 
     Parameters
     ----------
@@ -353,17 +365,17 @@
         Set to ``True`` when running a script or ``pytest``.
 
     """
     fig = plt.figure(figsize=(20,20))
     ax = fig.add_subplot()
 
     if categorical:
-        cmap = matplotlib.colormaps.get_cmap('tab10')
+        cmap = plt.get_cmap('tab10')
     else:
-        cmap = matplotlib.colormaps.get_cmap('Purples')
+        cmap = plt.get_cmap('Purples')
     unique_colours = list(set(colours))
     norm = plt.Normalize(np.min(colours), np.max(colours))
     legend_patches = [patches.Patch(color=cmap(norm(color))) for color in unique_colours]
     im = ax.scatter(embedding[:, 0], embedding[:, 1] , s=50, c=colours, cmap=cmap)
 
     for i in range(len(pdb_codes)):
         if i % 1 == 0:
@@ -440,15 +452,15 @@
 
     """
 
     labels = ['FR-H1', 'CDR-H1', 'FR-H2', 'CDR-H2', 'FR-H3', 'CDR-H3', 'FR-H4', 'FR-L1', 'CDR-L1', 'FR-L2', 'CDR-L2', 'FR-L3', 'CDR-L3', 'FR-L4']
     mapping_dict = {0: 0, 1: 2, 2: 1, 3: 5}
 
     sorted_indices = np.argsort(importance_factor)[::-1]  # Reverse order
-    cmap = matplotlib.colormaps.get_cmap('tab10')
+    cmap = plt.get_cmap('tab10')
 
     # Create bars for each class
     fig, ax = plt.subplots()
     y_pos = np.arange(len(labels))
 
     bar1 = ax.barh(y_pos, np.array(importance_factor_ob)[sorted_indices], align='center', color=cmap(mapping_dict[antigen_type]), label=f'Inter-{mode}')
     bar2 = ax.barh(y_pos, np.array([importance_factor[i]-importance_factor_ob[i] for i in range(len(labels))])[sorted_indices], align='center', alpha=0.6, left=np.array(importance_factor_ob)[sorted_indices], color=cmap(mapping_dict[antigen_type]), label=f'Intra-{mode}')
@@ -504,15 +516,15 @@
     interactive: bool
         Set to ``True`` when running a script or ``pytest``.
 
     """
 
     res_labels = add_region_based_on_range(preprocessed_data.max_res_list_h+preprocessed_data.max_res_list_l)
     mapping_dict = {0: 0, 1: 2, 2: 1, 3: 5}
-    cmap = matplotlib.colormaps.get_cmap('tab10')
+    cmap = plt.get_cmap('tab10')
 
     fig, ax = plt.subplots()
     y_pos = np.arange(len(res_labels[:30]))
     bar1 = ax.barh(y_pos, sorted(importance_factor, reverse=True)[:30], align='center', alpha=0.9, color=cmap(mapping_dict[antigen_type]))
 
     # Show top 30
     ax.set_xlabel('Importance (%)')
@@ -568,15 +580,15 @@
         else:
             colours.append(cdict['Other'])
             clusters[i] = 'Other'
 
     return colours 
 
 def compute_region_importance(preprocessed_data, model, type_of_antigen, nanobodies, mode='region', interactive=False):
-    r"""Computes the importance factors (0-100) of all the Fv antibody regions.
+    r"""Computes the importance factors (0-100) of all the Fv antibody regions. Returns the importance for each region.
 
     Parameters
     ----------
     preprocessed_data: antipasti.preprocessing.preprocessing.Preprocessing
         The ``Preprocessing`` class.
     model: antipasti.model.model.ANTIPASTI
         The model class, i.e., ``ANTIPASTI``.
@@ -592,66 +604,70 @@
     """
 
     colours = get_colours_ag_type(preprocessed_data)
     each_img_enl = get_output_representations(preprocessed_data, model)
 
     train_x = preprocessed_data.train_x
     input_shape = preprocessed_data.test_x.shape[-1]
+    labels = preprocessed_data.labels
+    train_y = preprocessed_data.train_y
 
     colours = [0 if c == 5 else c for c in colours]
     all_mse_without_region = []
     all_mse_without_region_intra = []
     all_mse_without_region_ob = []
 
     new_coord = np.array([range(0, 26), range(26, 38), range(38, 57), range(57, 67), range(67, 116), range(116, 142), range(142, 153),
                         range(153, 176), range(176, 195), range(195, 210), range(210, 225), range(225, 265), range(265, 279), range(279, 292)], dtype=object)
     
     for j in range(len(new_coord)+1):
-        train_y_ = np.array([preprocessed_data.train_y[i] for i in range(train_x.shape[0]) if colours[i] == type_of_antigen and preprocessed_data.labels[i] not in nanobodies])
+        train_y_ = np.array([train_y[i] for i in range(each_img_enl.shape[0]) if colours[i] == type_of_antigen and labels[i] not in nanobodies])
         if j != len(new_coord):
             
             sums_without_region = np.array([
                 each_img_enl[i].reshape((input_shape, input_shape)).sum()-(each_img_enl[i].reshape((input_shape, input_shape))[new_coord[j][0]:new_coord[j][-1] + 1, :]).sum()
-                for i in range(train_x.shape[0]) if colours[i] == type_of_antigen and preprocessed_data.labels[i] not in nanobodies])
+                for i in range(each_img_enl.shape[0]) if colours[i] == type_of_antigen and labels[i] not in nanobodies])
 
             if mode == 'region':
                 sums_without_region_divided = np.array([
                         each_img_enl[i].reshape((input_shape, input_shape)).sum()-np.array([(each_img_enl[i].reshape((input_shape, input_shape))[new_coord[j][0]:new_coord[j][-1] + 1, new_coord[0][0]:new_coord[j][0]]).sum()
                                                                     +(each_img_enl[i].reshape((input_shape, input_shape))[new_coord[j][0]:new_coord[j][-1] + 1, new_coord[j][-1] + 1:new_coord[-1][-1] + 1]).sum(),
                                                                     (each_img_enl[i].reshape((input_shape, input_shape))[new_coord[j][0]:new_coord[j][-1] + 1, new_coord[j][0]:new_coord[j][-1] + 1]).sum()])
-                        for i in range(train_x.shape[0]) if colours[i] == type_of_antigen and preprocessed_data.labels[i] not in nanobodies])
+                        for i in range(each_img_enl.shape[0]) if colours[i] == type_of_antigen and labels[i] not in nanobodies])
 
                 all_mse_without_region_intra.append(np.mean((sums_without_region_divided[:,1] - train_y_)**2))
                 all_mse_without_region_ob.append(np.mean((sums_without_region_divided[:,0] - train_y_)**2))
             
             else:
                 sums_without_region_divided = np.array([
                         each_img_enl[i].reshape((input_shape, input_shape)).sum()-np.array([(each_img_enl[i].reshape((input_shape, input_shape))[new_coord[j][0]:new_coord[j][-1] + 1, :len(preprocessed_data.max_res_list_h)]).sum(),
                                                                     (each_img_enl[i].reshape((input_shape, input_shape))[new_coord[j][0]:new_coord[j][-1] + 1, len(preprocessed_data.max_res_list_h):]).sum()])
-                        for i in range(train_x.shape[0]) if colours[i] == type_of_antigen and preprocessed_data.labels[i] not in nanobodies])
+                        for i in range(each_img_enl.shape[0]) if colours[i] == type_of_antigen and labels[i] not in nanobodies])
 
                 index = 0 if j < 7 else 1
                 all_mse_without_region_intra.append(np.mean((sums_without_region_divided[:, index] - train_y_)**2))
                 all_mse_without_region_ob.append(np.mean((sums_without_region_divided[:, 1 - index] - train_y_)**2))
         else:
             sums_without_region = np.array([
                     each_img_enl[i].reshape((input_shape, input_shape)).sum()
-                    for i in range(train_x.shape[0]) if colours[i] == type_of_antigen and preprocessed_data.labels[i] not in nanobodies])
+                    for i in range(each_img_enl.shape[0]) if colours[i] == type_of_antigen and labels[i] not in nanobodies])
 
         all_mse_without_region.append(np.mean((sums_without_region - train_y_)**2))
     total_mse = all_mse_without_region[-1]
     all_mse_without_region.pop(-1)
 
     region_mean_lengths = np.array([24, 7.1, 19, 6, 41, 11.3, 10, 21.7, 12.7, 14.9, 7, 32.9, 9.2, 9.1])
     idx_best_normalised_mean_length = np.argmax(abs(all_mse_without_region-total_mse)/region_mean_lengths)
 
     tot = 100*region_mean_lengths[idx_best_normalised_mean_length] * abs(all_mse_without_region-total_mse) / abs(all_mse_without_region[idx_best_normalised_mean_length]-total_mse)/region_mean_lengths
     ob = tot - tot * abs(all_mse_without_region_intra-total_mse) / (abs(all_mse_without_region_intra-total_mse)+abs(all_mse_without_region_ob-total_mse))
     plot_region_importance(tot, ob, type_of_antigen, mode, interactive=interactive)
 
+    return tot, ob
+
 def compute_residue_importance(preprocessed_data, model, type_of_antigen, nanobodies, interactive=False):
     r"""Computes the importance factors (0-100) of all the amino acids of the antibody variable region.
 
     Parameters
     ----------
     preprocessed_data: antipasti.preprocessing.preprocessing.Preprocessing
         The ``Preprocessing`` class.
```

### Comparing `ANTIPASTI-1.1/antipasti/utils/torch_utils.py` & `antipasti-1.2/antipasti/utils/torch_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,75 @@
 import numpy as np
 import torch
+import os
 
 from adabelief_pytorch import AdaBelief
 from sklearn.model_selection import train_test_split
 from torch.autograd import Variable
 
 from antipasti.model.model import ANTIPASTI
+from antipasti.utils.biology_utils import check_train_test_identity 
+from config import DATA_DIR
 
-def create_test_set(train_x, train_y, test_size=None, random_state=0):
+def create_test_set(preprocessed_data, test_size=None, random_state=0, residues_path=DATA_DIR+'lists_of_residues/'):
     r"""Creates the test set given a set of input images and their corresponding labels.
 
     Parameters
     ----------
-    train_x: numpy.ndarray
-        Input normal mode correlation maps.
-    train_y: numpy.ndarray
-        Labels.
+    preprocessed_data: antipasti.preprocessing.Preprocessed
+        An instance of the Preprocessed class.
     test_size: float
         Fraction of original samples to be included in the test set.
     random_state: int
         Set lot number.
-
+    residues_path: str
+        Path to the folder containing the list of residues per entry.
+        
     Returns
     -------
     train_x: torch.Tensor
         Training inputs.
     test_x: torch.Tensor
         Test inputs.
     train_y: torch.Tensor
         Training labels. 
     test_y: torch.Tensor
         Test labels.
 
     """
 
     # Splitting
-    indices = np.arange(len(train_x))
-    train_x, test_x, train_y, test_y, indices_train, indices_test = train_test_split(train_x, train_y, indices, test_size=0.023, random_state=23)
+    indices_train = list(np.arange(len(preprocessed_data.train_x)))
+    #train_x, test_x, train_y, test_y, indices_train, indices_test = train_test_split(preprocessed_data.train_x, preprocessed_data.train_y, indices, test_size=0.023, random_state=random_state)
+    indices_test = []
+
+    np.random.seed(random_state)
+    random_order = indices_train.copy()
+    np.random.shuffle(random_order)
+
+    for i in range(int(len(indices_train)*test_size)):
+        test_idx = random_order[i]
+        indices_train.remove(test_idx)
+
+        if isinstance(preprocessed_data.labels[test_idx], str): # Check if first added
+            test_instance = [preprocessed_data.labels[test_idx]]
+        else:
+            test_instance = list(np.array(preprocessed_data.labels)[test_idx])
+
+        if check_train_test_identity(list(np.array(preprocessed_data.labels)[indices_train]), test_instance, preprocessed_data.max_res_list_h, preprocessed_data.max_res_list_l, threshold=0.9, residues_path=residues_path):
+            indices_test.append(test_idx)
+        else:
+            i -= 1
+            indices_train.append(test_idx)
+
+    
+    train_x = preprocessed_data.train_x[indices_train]
+    test_x = preprocessed_data.train_x[indices_test]
+    train_y = preprocessed_data.train_y[indices_train]
+    test_y = preprocessed_data.train_y[indices_test]
 
     # Converting to tensors
     train_x = train_x.reshape(train_x.shape[0], 1, train_x.shape[1], train_x.shape[1])
     train_x = train_x.astype(np.float32)
     train_x  = torch.from_numpy(train_x)
     train_y = train_y.astype(np.float32).reshape(train_y.shape[0], 1)
     train_y = torch.from_numpy(train_y)
@@ -108,26 +137,31 @@
     if model.mode != 'full':
         inter_filter = np.zeros((x_train.size()[0], 1, model.input_shape, model.input_shape))
     permutation = torch.randperm(x_train.size()[0])
 
     for i in range(0, x_train.size()[0], batch_size):
         indices = permutation[i:i+batch_size]
         batch_x, batch_y = x_train[indices], y_train[indices]
-        
+        #batch_weights = weights[indices]
+
         # Training output
         output_train, inter_filters = model(batch_x)
         
         # Picking the appropriate filters before the fully-connected layer
         inter_filters_detached = inter_filters.detach().clone()
         inter_filter[i:i+batch_size] = inter_filters_detached.numpy()
 
         # Training loss, clearing gradients and updating weights
         optimiser.zero_grad()
         l1_loss = model.l1_regularization_loss()
-        mse_loss = criterion(output_train[:, 0], batch_y[:, 0])
+
+        # Compute the mean of the weighted squared differences
+        mse_loss = torch.mean((output_train[:, 0] - batch_y[:, 0])**2)
+
+        #mse_loss = criterion(output_train[:, 0], batch_y[:, 0])
         loss_train = mse_loss + l1_loss
         if verbose:
             print(l1_loss)
         loss_train.backward()
         optimiser.step()
         # Adding batch contribution to training loss
         tr_loss += loss_train.item() * batch_size / x_train.size()[0]
```

### Comparing `ANTIPASTI-1.1/setup.py` & `antipasti-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
 setup(
     name='ANTIPASTI',
-    version='1.1',
+    version='1.2',
     author='Kevin Michalewicz',
     author_email='k.michalewicz22@imperial.ac.uk',
     description='Deep Learning model that predicts the binding affinity of antibodies from their three-dimensional structure.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['antipasti', 'antipasti.model', 'antipasti.preprocessing', 'antipasti.utils'],
     install_requires=['adabelief-pytorch', 'biopython', 'matplotlib', 'numpy', 'opencv-python', 'optuna', 'pandas', 'requests', 'scikit-learn', 'scipy', 'torch', 'torchmetrics', 'umap-learn'],
```

