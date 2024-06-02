# Comparing `tmp/pyRealtor-0.1.4-py3-none-any.whl.zip` & `tmp/pyRealtor-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11403 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      367 b- defN 24-Feb-25 03:00 pyRealtor/__init__.py
--rw-rw-rw-  2.0 fat     4612 b- defN 24-Feb-26 06:25 pyRealtor/facade.py
+Zip file size: 11649 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      367 b- defN 24-Mar-03 04:03 pyRealtor/__init__.py
+-rw-rw-rw-  2.0 fat     5422 b- defN 24-Mar-03 04:27 pyRealtor/facade.py
 -rw-rw-rw-  2.0 fat     2568 b- defN 24-Feb-25 03:15 pyRealtor/geo.py
 -rw-rw-rw-  2.0 fat     1953 b- defN 24-Feb-24 21:05 pyRealtor/proxy.py
--rw-rw-rw-  2.0 fat    10250 b- defN 24-Feb-24 08:31 pyRealtor/realtor.py
+-rw-rw-rw-  2.0 fat    10498 b- defN 24-Mar-03 03:43 pyRealtor/realtor.py
 -rw-rw-rw-  2.0 fat     3594 b- defN 24-Feb-26 06:14 pyRealtor/report.py
 -rw-rw-rw-  2.0 fat      810 b- defN 24-Feb-24 08:07 pyRealtor/config/column_mapping_cfg.json
--rw-rw-rw-  2.0 fat     1137 b- defN 24-Feb-26 07:09 pyRealtor-0.1.4.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     4311 b- defN 24-Feb-26 07:09 pyRealtor-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-26 07:09 pyRealtor-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Feb-26 07:09 pyRealtor-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      950 b- defN 24-Feb-26 07:09 pyRealtor-0.1.4.dist-info/RECORD
-12 files, 30654 bytes uncompressed, 9819 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat     1137 b- defN 24-Mar-03 04:35 pyRealtor-0.1.5.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     4311 b- defN 24-Mar-03 04:35 pyRealtor-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-03 04:35 pyRealtor-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-03 04:35 pyRealtor-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      950 b- defN 24-Mar-03 04:35 pyRealtor-0.1.5.dist-info/RECORD
+12 files, 31712 bytes uncompressed, 10065 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pyRealtor/report.py
 Comment: 
 
 Filename: pyRealtor/config/column_mapping_cfg.json
 Comment: 
 
-Filename: pyRealtor-0.1.4.dist-info/LICENSE.md
+Filename: pyRealtor-0.1.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyRealtor-0.1.4.dist-info/METADATA
+Filename: pyRealtor-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pyRealtor-0.1.4.dist-info/WHEEL
+Filename: pyRealtor-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyRealtor-0.1.4.dist-info/top_level.txt
+Filename: pyRealtor-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyRealtor-0.1.4.dist-info/RECORD
+Filename: pyRealtor-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyRealtor/__init__.py

```diff
@@ -1,14 +1,14 @@
 from pyRealtor.geo import GeoLocationService
 from pyRealtor.realtor import RealtorService
 from pyRealtor.report import ReportingService
 from pyRealtor.facade import HousesFacade
 from pyRealtor.proxy import Proxy
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 __all__ = [
     "GeoLocationService",
     "RealtorService",
     "ReportingService",
     "HousesFacade",
     "Proxy"
```

## pyRealtor/facade.py

```diff
@@ -10,26 +10,27 @@
     def search_save_houses(
         self,
         search_area: str,
         report_file_name: str,
         listing_type: str = 'for_sale',
         use_proxy: bool = False, 
         get_summary: bool = True,
+        price_from: int = 0,
         column_mapping_cfg_fpath:str = 'config/column_mapping_cfg.json', 
         column_lst: list = [
         'MLS', 'Description', 'Bedrooms', 'Bathrooms', 'Size', 'Stories', 
         'House Category', 'Ammenities', 
         'Price', 'Address', 'Latitude', 'Longitude', 'Ownership Category', 'Nearby Ammenities', 'Open House', 'Website'],
         **kwargs
     ):
         current_directory = os.getcwd()
         file_path_to_save = os.path.join(current_directory, report_file_name)
 
-        if 'listing_type' == 'for_rent':
-            column_lst = ['Rent' if x=='Price' else x for x in column_lst]
+
+        
 
         geo_service_obj = GeoLocationService()
         realtor_service_obj = RealtorService(
             ReportingService(
                 column_mapping_cfg_fpath,
                 column_lst
             )
@@ -48,57 +49,83 @@
         )
 
         geo_service_obj.set_display_physical_location(display_address)
         geo_service_obj.set_geo_location_boundry(geo_coord_1, geo_coord_2)
 
         realtor_service_obj.set_geo_coordinate_boundry(geo_service_obj)
         realtor_service_obj.set_transaction_type(listing_type)
+
+        if listing_type == 'for_sale':
+            sorted_col_name = 'Price'
+        else:
+            sorted_col_name = 'Rent'
+            column_lst = ['Rent' if x=='Price' else x for x in column_lst]
+
+        realtor_service_obj.set_min_amount(
+            new_amount = int(price_from),
+            col_name = sorted_col_name
+        )
+
         realtor_service_obj.set_sort_method(by='listing_price', ascending_order=True)
 
         if 'open_house_date' in kwargs:
             open_house_date = kwargs['open_house_date']
             realtor_service_obj.set_open_house_only(open_house_date)
 
         #print(realtor_service_obj.search_api_params)
 
         houses_df = realtor_service_obj.search_houses(
             use_proxy
         ).to_dataframe()
 
+        loop_counter = 0
+
         if houses_df.shape[0] > 0:
-            if listing_type == 'for_sale':
-                sorted_col_name = 'Price'
-            else:
-                sorted_col_name = 'Rent'
 
-            current_min_amount = pd.to_numeric(houses_df[sorted_col_name]).values[-1]
+            current_min_amount = pd.to_numeric(
+                houses_df[sorted_col_name],
+                downcast="integer"
+            ).values[-1]
+
             while True:
+                print(f"Fetching listings with minimum price: {current_min_amount}")
+                
+                if loop_counter > 10:
+                    print(f"The Maximun Limit has reached. Please use the function with parameter price_from={current_min_amount} after some time")
+                    break
+                
                 realtor_service_obj.set_min_amount(
-                    new_amount = current_min_amount,
+                    new_amount = int(current_min_amount),
                     col_name = sorted_col_name
                 )
 
                 try:
                     new_houses_df = realtor_service_obj.search_houses(
                         use_proxy
                     ).to_dataframe()
                 except Exception as e:
+                    print(f"Exception raised while searching from Minimum Price: {current_min_amount}: {e}")
                     break
 
                 if new_houses_df.shape[0] > 0:
-                    new_min_amount = pd.to_numeric(new_houses_df[sorted_col_name]).values[-1]
+                    new_min_amount = pd.to_numeric(
+                        new_houses_df[sorted_col_name],
+                        downcast="integer"
+                    ).values[-1]
 
                     if new_min_amount > current_min_amount:
                         houses_df = pd.concat([houses_df, new_houses_df], axis=0).drop_duplicates(subset=['MLS'])
                         current_min_amount = new_min_amount
                     else:
                         break
                 else:
                     break
 
+                loop_counter += 1
+
 
         if get_summary:
             if listing_type == 'for_sale':
                 summary_df = realtor_service_obj.report_obj.get_average(
                     dataframe = houses_df.copy(),
                     average_col_name = 'Price',
                     grpby_col_lst = ['Bedrooms', 'Bathrooms', 'House Category', 'Ownership Category']
```

## pyRealtor/realtor.py

```diff
@@ -148,14 +148,16 @@
 
                         if realtor_api_response.status_code == 200:
                             break
                         elif realtor_api_response.status_code == 403:
                             print(f"Proxy {proxy.current_proxy} is blocked by REALTOR.CA")
                             continue
 
+                    except requests.exceptions.ChunkedEncodingError as chunkEncodingException:
+                        continue
                     except requests.exceptions.ProxyError as proxyException:
                         continue
                     except requests.exceptions.ConnectionError as connectionException:
                         continue
                 
             else:
                 realtor_api_response = s.post(
@@ -194,15 +196,17 @@
                                     break
                                 elif realtor_api_response.status_code == 403:
                                     print(f"Proxy {proxy.current_proxy} is blocked by REALTOR.CA")
                                     continue
                                 else:
                                     continue
                                 
-                            
+                            except requests.exceptions.ChunkedEncodingError as chunkEncodingException:
+                                continue
+
                             except requests.exceptions.ProxyError as proxyException:
                                 continue
 
                             except requests.exceptions.ConnectionError as connectionException:
                                 continue
 
                     else:
```

## Comparing `pyRealtor-0.1.4.dist-info/LICENSE.md` & `pyRealtor-0.1.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyRealtor-0.1.4.dist-info/METADATA` & `pyRealtor-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealtor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for fetching and analyzing REALTOR.CA MLS Listings
 Home-page: https://github.com/rachitt96/pyRealtor
 Author: Rachit Trivedi
 Author-email: rachitt96@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `pyRealtor-0.1.4.dist-info/RECORD` & `pyRealtor-0.1.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pyRealtor/__init__.py,sha256=OUXklWc7j9K8wuBqhNRZNFpoCiGNR9X_qoI54CiHRfc,367
-pyRealtor/facade.py,sha256=37n9ju5JRNWC4m2m08GLrfnIVT04f9sRUeNyxZjZ5CU,4612
+pyRealtor/__init__.py,sha256=-9QkUtp6EohWjLkTW3Ifl1AyqEZ7PkXR-caAdNzLEwk,367
+pyRealtor/facade.py,sha256=JoaIa2UiZNPdl1iVkClLkpAhKDjNOu0oRaLlevdT3uA,5422
 pyRealtor/geo.py,sha256=bxPot3sw-qfhy8PCIHm9MToTn0ArLpYYFw5C5pJ-pdA,2568
 pyRealtor/proxy.py,sha256=Vk7GFFZSzWRwbHepDEFLrjObtMqZmRmCaMYOjOyt8ys,1953
-pyRealtor/realtor.py,sha256=j8Bnwk4L6teTgRTbmtXEuzBT4x1COjL7tzIZ_fiG0ew,10250
+pyRealtor/realtor.py,sha256=9HjFUVVL3w3EnV01jOmUWuYg68Q2s6dnJJ-7rhbkOhg,10498
 pyRealtor/report.py,sha256=c_hUvLQqyvszponmenR1OT-Wv3ZJ3I3YnD631v_kLUQ,3594
 pyRealtor/config/column_mapping_cfg.json,sha256=X4lJ_33fa-01wybaMppVMWedh0Ek-v1NnzfMzfmLVlI,810
-pyRealtor-0.1.4.dist-info/LICENSE.md,sha256=fXLlor4iPcMb9rBjwd9l2_vOMyezIoLg0TaSbRT2_P0,1137
-pyRealtor-0.1.4.dist-info/METADATA,sha256=jqUUPFoHjAnO-cOthzeu9S2nTfKqyUx1qEfCYuXnFAM,4311
-pyRealtor-0.1.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pyRealtor-0.1.4.dist-info/top_level.txt,sha256=TTBfFsvPGh0MPFp8ahMBdPSXXk9TLuNSw42qZMwlxqg,10
-pyRealtor-0.1.4.dist-info/RECORD,,
+pyRealtor-0.1.5.dist-info/LICENSE.md,sha256=fXLlor4iPcMb9rBjwd9l2_vOMyezIoLg0TaSbRT2_P0,1137
+pyRealtor-0.1.5.dist-info/METADATA,sha256=As2mAecxXw9NMcSuNevaCYjDsjJp-Lo3JpNSnxLlwKE,4311
+pyRealtor-0.1.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pyRealtor-0.1.5.dist-info/top_level.txt,sha256=TTBfFsvPGh0MPFp8ahMBdPSXXk9TLuNSw42qZMwlxqg,10
+pyRealtor-0.1.5.dist-info/RECORD,,
```

