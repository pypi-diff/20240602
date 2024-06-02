# Comparing `tmp/pymerc-0.5.0.tar.gz` & `tmp/pymerc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymerc-0.5.0.tar", max compression
+gzip compressed data, was "pymerc-0.6.0.tar", max compression
```

## Comparing `pymerc-0.5.0.tar` & `pymerc-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     4677 2024-05-24 21:36:31.962610 pymerc-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-24 21:36:31.962610 pymerc-0.5.0/pymerc/__init__.py
--rw-r--r--   0        0        0      382 2024-05-24 21:36:31.962610 pymerc-0.5.0/pymerc/api/base.py
--rw-r--r--   0        0        0     1985 2024-05-24 21:36:31.962610 pymerc-0.5.0/pymerc/api/buildings.py
--rw-r--r--   0        0        0      607 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/businesses.py
--rw-r--r--   0        0        0      571 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/map.py
--rw-r--r--   0        0        0     1325 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/buildings.py
--rw-r--r--   0        0        0      912 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/businesses.py
--rw-r--r--   0        0        0    22082 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/common.py
--rw-r--r--   0        0        0      593 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/map.py
--rw-r--r--   0        0        0     1448 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/player.py
--rw-r--r--   0        0        0     2693 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/static.py
--rw-r--r--   0        0        0   128191 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/test.json
--rw-r--r--   0        0        0     3140 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/towns.py
--rw-r--r--   0        0        0     1732 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/transports.py
--rw-r--r--   0        0        0      482 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/player.py
--rw-r--r--   0        0        0     2377 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/static.py
--rw-r--r--   0        0        0     5264 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/towns.py
--rw-r--r--   0        0        0     1541 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/transports.py
--rw-r--r--   0        0        0     5939 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/client.py
--rw-r--r--   0        0        0      334 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/exceptions.py
--rw-r--r--   0        0        0     7540 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/building.py
--rw-r--r--   0        0        0     6779 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/exports.py
--rw-r--r--   0        0        0     6826 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/imports.py
--rw-r--r--   0        0        0     3889 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/player.py
--rw-r--r--   0        0        0     2840 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/recipe.py
--rw-r--r--   0        0        0    10978 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/storehouse.py
--rw-r--r--   0        0        0     4588 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/town.py
--rw-r--r--   0        0        0     9016 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/transport.py
--rw-r--r--   0        0        0      600 2024-05-24 21:36:31.970610 pymerc-0.5.0/pymerc/util/data.py
--rw-r--r--   0        0        0     1602 2024-05-24 21:36:31.970610 pymerc-0.5.0/pymerc/util/towns.py
--rw-r--r--   0        0        0      835 2024-05-24 21:36:31.970610 pymerc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5448 1970-01-01 00:00:00.000000 pymerc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5724 2024-06-02 19:20:24.900179 pymerc-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/__init__.py
+-rw-r--r--   0        0        0      382 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/base.py
+-rw-r--r--   0        0        0     2092 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/buildings.py
+-rw-r--r--   0        0        0      607 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/businesses.py
+-rw-r--r--   0        0        0      571 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/map.py
+-rw-r--r--   0        0        0     1325 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/buildings.py
+-rw-r--r--   0        0        0      912 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/businesses.py
+-rw-r--r--   0        0        0    23118 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/common.py
+-rw-r--r--   0        0        0      593 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/map.py
+-rw-r--r--   0        0        0     1448 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/player.py
+-rw-r--r--   0        0        0     2727 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/static.py
+-rw-r--r--   0        0        0     3330 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/towns.py
+-rw-r--r--   0        0        0     1732 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/models/transports.py
+-rw-r--r--   0        0        0      482 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/player.py
+-rw-r--r--   0        0        0     2377 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/static.py
+-rw-r--r--   0        0        0     5264 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/towns.py
+-rw-r--r--   0        0        0     1541 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/api/transports.py
+-rw-r--r--   0        0        0     7495 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/client.py
+-rw-r--r--   0        0        0      334 2024-06-02 19:20:24.900179 pymerc-0.6.0/pymerc/exceptions.py
+-rw-r--r--   0        0        0     8836 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/building.py
+-rw-r--r--   0        0        0     6779 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/exports.py
+-rw-r--r--   0        0        0     6826 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/imports.py
+-rw-r--r--   0        0        0     7849 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/operation.py
+-rw-r--r--   0        0        0     4423 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/player.py
+-rw-r--r--   0        0        0     3021 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/recipe.py
+-rw-r--r--   0        0        0    11117 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/storehouse.py
+-rw-r--r--   0        0        0     4888 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/town.py
+-rw-r--r--   0        0        0     9016 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/game/transport.py
+-rw-r--r--   0        0        0      600 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/util/data.py
+-rw-r--r--   0        0        0     1602 2024-06-02 19:20:24.904179 pymerc-0.6.0/pymerc/util/towns.py
+-rw-r--r--   0        0        0      835 2024-06-02 19:20:24.904179 pymerc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6495 1970-01-01 00:00:00.000000 pymerc-0.6.0/PKG-INFO
```

### Comparing `pymerc-0.5.0/pymerc/api/buildings.py` & `pymerc-0.6.0/pymerc/api/buildings.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,18 @@
         Args:
             id (int): The ID of the building.
 
         Returns:
             BuildingOperation: The building operation information.
         """
         response = await self.client.get(f"{BASE_URL}{id}/operations")
-        return buildings.BuildingOperation.model_validate(response.json())
+        if response.status_code == 404:
+            return buildings.BuildingOperation()
+        else:
+            return buildings.BuildingOperation.model_validate(response.json())
 
     async def set_manager(
         self, id: int, item: common.Item, manager: common.InventoryManager
     ) -> buildings.Building:
         """Set the manager for an item in a building.
 
         Args:
```

### Comparing `pymerc-0.5.0/pymerc/api/businesses.py` & `pymerc-0.6.0/pymerc/api/businesses.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/map.py` & `pymerc-0.6.0/pymerc/api/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/models/buildings.py` & `pymerc-0.6.0/pymerc/api/models/buildings.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/models/businesses.py` & `pymerc-0.6.0/pymerc/api/models/businesses.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/models/common.py` & `pymerc-0.6.0/pymerc/api/models/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class BuildingType(Enum):
     """Represents the type of a building."""
 
     Apothecary = "apothecary"
     Bakery = "bakery"
     Bloomery = "bloomery"
+    BoardingHouse = "boardinghouse"
     Brewery = "brewery"
     Brickworks = "brickworks"
     Butchery = "butchery"
     Carpentry = "carpentry"
     Cartshed = "cartshed"
     Cathedral = "cathedral"
     Center = "center"
@@ -40,14 +41,15 @@
     Coppersmith = "coppersmith"
     Cottage = "cottage"
     Dairy = "dairy"
     DyeBoiler = "dye boiler"
     Dyeworks = "dyeworks"
     Farmstead = "farmstead"
     Fisher = "fisher"
+    FishingShack = "fishing shack"
     FlaxFarm = "flax farm"
     Foundry = "foundry"
     GlassBlower = "glass blower"
     GlassHouse = "glass house"
     GoldMine = "gold mine"
     GrainFarm = "grain farm"
     Guardhouse = "guardhouse"
@@ -67,14 +69,15 @@
     NetMaker = "net maker"
     Outpost = "outpost"
     Park = "park"
     Pasture = "pasture"
     Quarry = "quarry"
     RettingPit = "retting pit"
     Ropewalk = "ropewalk"
+    SailLoft = "sail loft"
     Saltery = "saltery"
     SaltMine = "salt mine"
     Sawmill = "sawmill"
     SewingShop = "sewing shop"
     Shipyard = "shipyard"
     Smithy = "smithy"
     Smokery = "smokery"
@@ -184,14 +187,15 @@
     Ham = "ham"
     Handcart = "handcart"
     Harnesses = "harnesses"
     Herbs = "herbs"
     Hides = "hides"
     Honey = "honey"
     HopBeer = "hop beer"
+    Hulk = "hulk"
     IronOre = "iron ore"
     Jewellery = "jewellery"
     Labour = "labour"
     LeadBars = "lead bars"
     LeadOre = "lead ore"
     Leather = "leather"
     LightArmor = "light armor"
@@ -211,14 +215,15 @@
     Pasties = "pasties"
     Pickaxes = "pickaxes"
     Pies = "pies"
     Ploughs = "ploughs"
     Protection = "protection"
     Resin = "resin"
     Rope = "rope"
+    Sails = "sails"
     Salt = "salt"
     Scythes = "scythes"
     SilverBars = "silver bars"
     SlakedLime = "slaked lime"
     Snekkja = "snekkja"
     Spirits = "spirits"
     SteelIngots = "steel ingots"
@@ -268,16 +273,18 @@
     BrewBeer1 = "brew beer 1"
     BrewBeer2 = "brew beer 2"
     BrewBeer3 = "brew beer 3"
     BrewBeer4 = "brew beer 4"
     BrewHopBeer1 = "brew hop beer 1"
     BrewHopBeer2 = "brew hop beer 2"
     BuildCog1 = "build cog 1"
+    BuildCog2 = "build cog 2"
     BuildHandcart1 = "build handcart 1"
     BuildHandcart2 = "build handcart 2"
+    BuildHulk1 = "build hulk 1"
     BuildSnekkja1 = "build snekkja 1"
     BuildSnekkja2 = "build snekkja 2"
     BuildTumbrel1 = "build tumbrel 1"
     BurnBricks1 = "burn bricks 1"
     BurnCharcoal1 = "burn charcoal 1"
     BurnCharcoal2 = "burn charcoal 2"
     BurnCharcoal3 = "burn charcoal 3"
@@ -285,35 +292,38 @@
     BurnCookware1 = "burn cookware 1"
     BurnCookware2 = "burn cookware 2"
     BurnGlass1 = "burn glass 1"
     BurnLime1 = "burn lime 1"
     BurnTar1 = "burn tar 1"
     BurnTar2 = "burn tar 2"
     BurnTiles1 = "burn tiles 1"
+    BurnTiles2 = "burn tiles 2"
     ButcherCattle1a = "butcher cattle 1a"
     ButcherCattle1b = "butcher cattle 1b"
     ButcherCattle2 = "butcher cattle 2"
     Carting1 = "carting 1"
     Carting2 = "carting 2"
     ChurnButter1 = "churn butter 1"
     ChurnButter2 = "churn butter 2"
     CogOperations = "cog operations"
     CraftArms1 = "craft arms 1"
     CraftBelts1 = "craft belts 1"
     CraftBelts2 = "craft belts 2"
     CraftBelts3 = "craft belts 3"
+    CraftBelts4 = "craft belts 4"
     CraftCookware1 = "craft cookware 1"
     CraftFurniture1 = "craft furniture 1"
     CraftFurniture2 = "craft furniture 2"
     CraftFurniture3 = "craft furniture 3"
     CraftFurniture4 = "craft furniture 4"
     CraftPloughs1 = "craft ploughs 1"
     CraftPloughs2 = "craft ploughs 2"
     CraftPloughs3 = "craft ploughs 3"
     CraftScythes1 = "craft scythes 1"
+    CraftScythes2 = "craft scythes 2"
     CraftTools1 = "craft tools 1"
     CraftTools2 = "craft tools 2"
     CraftWheels1 = "craft wheels 1"
     CraftWheels2 = "craft wheels 2"
     CraftWheels3 = "craft wheels 3"
     CutBricks1 = "cut bricks 1"
     CutGrindstones1 = "cut grindstones 1"
@@ -331,14 +341,15 @@
     DyeCloth2 = "dye cloth 2"
     ExtractStone1 = "extract stone 1"
     ExtractStone2 = "extract stone 2"
     ExtractStone3 = "extract stone 3"
     Fishing1 = "fishing 1"
     Fishing2a = "fishing 2a"
     Fishing2b = "fishing 2b"
+    Fishing3 = "fishing 3"
     ForgeArms1 = "forge arms 1"
     ForgeArms2 = "forge arms 2"
     ForgeArms2b = "forge arms 2b"
     ForgeAxes1 = "forge axes 1"
     ForgeAxes1b = "forge axes 1b"
     ForgeAxes2 = "forge axes 2"
     ForgeAxes2b = "forge axes 2b"
@@ -440,80 +451,99 @@
     MakeCheese1 = "make cheese 1"
     MakeCheese2 = "make cheese 2"
     MakeCheese3 = "make cheese 3"
     MakeCheese4 = "make cheese 4"
     MakeCheese5 = "make cheese 5"
     MakeHarnesses1 = "make harnesses 1"
     MakeHarnesses2 = "make harnesses 2"
+    MakeHarnesses2b = "make harnesses 2b"
     MakeJewellery1 = "make jewellery 1"
     MakeJewellery2 = "make jewellery 2"
     MakeLeatherArmor1 = "make leather armor 1"
     MakeMedicine1 = "make medicine 1"
+    MakeMedicine2 = "make medicine 2"
     MakeNets1 = "make nets 1"
     MakeNets2 = "make nets 2"
+    MakeNets3 = "make nets 3"
     MakeRope1 = "make rope 1"
     MakeWindows1 = "make windows 1"
     MakeWine1 = "make wine 1"
     MakeWine2 = "make wine 2"
+    MakeWine3 = "make wine 3"
     Malting1 = "malting 1"
     Malting2 = "malting 2"
     Milling1 = "milling 1"
     Milling2 = "milling 2"
     Milling3 = "milling 3"
     MineCopper1 = "mine copper 1"
     MineCopper2 = "mine copper 2"
     MineCopper3 = "mine copper 3"
     MineCopper4 = "mine copper 4"
     MineGold1 = "mine gold 1"
+    MineGold1b = "mine gold 1b"
     MineGold2 = "mine gold 2"
+    MineGold2b = "mine gold 2b"
     MineIron1 = "mine iron 1"
     MineIron2 = "mine iron 2"
     MineIron3 = "mine iron 3"
     MineIron4 = "mine iron 4"
     MineLead1 = "mine lead 1"
     MineLead2 = "mine lead 2"
+    MineLead2b = "mine lead 2b"
     MineLead3 = "mine lead 3"
+    MineLead3b = "mine lead 3b"
     MineSalt1 = "mine salt 1"
     MineSalt2 = "mine salt 2"
+    MineSalt3 = "mine salt 3"
     MintCopperCoins1 = "mint copper coins 1"
     MintCopperCoins2 = "mint copper coins 2"
     MintGoldCoins1 = "mint gold coins 1"
     MintGoldCoins2 = "mint gold coins 2"
     MintSilverCoins1 = "mint silver coins 1"
     MintSilverCoins2 = "mint silver coins 2"
     Patrol1 = "patrol 1"
     Patrol2a = "patrol 2a"
     Patrol2b = "patrol 2b"
     Patrol3a = "patrol 3a"
     Patrol3b = "patrol 3b"
     RefineSteel1 = "refine steel 1"
+    RefineSteel1b = "refine steel 1b"
     RefineSteel2 = "refine steel 2"
+    RefineSteel2b = "refine steel 2b"
     Retting1 = "retting 1"
     Retting2 = "retting 2"
     SaltingFish1 = "salting fish 1"
     SaltingFish2 = "salting fish 2"
     SaltingMeat1 = "salting meat 1"
     SaltingMeat2 = "salting meat 2"
     Sawing1 = "sawing 1"
     Sawing2 = "sawing 2"
+    Sawing3 = "sawing 3"
+    Sawing4 = "sawing 4"
     Service1 = "service 1"
+    Service2 = "service 2"
+    Service3 = "service 3"
+    Service4 = "service 4"
     SewCoats1a = "sew coats 1a"
     SewCoats1b = "sew coats 1b"
     SewCoats2a = "sew coats 2a"
     SewCoats2b = "sew coats 2b"
     SewGambeson1 = "sew gambeson 1"
     SewGarments1 = "sew garments 1"
     SewGarments2a = "sew garments 2a"
     SewGarments2b = "sew garments 2b"
     SewGarments3a = "sew garments 3a"
     SewGarments3b = "sew garments 3b"
     SewGarments4a = "sew garments 4a"
     SewGarments4b = "sew garments 4b"
+    SewSails1 = "sew sails 1"
+    SewSails2 = "sew sails 2"
     ShearSheep1 = "shear sheep 1"
     ShearSheep2 = "shear sheep 2"
+    ShearSheep3 = "shear sheep 3"
     SmeltCopper1 = "smelt copper 1"
     SmeltCopper2 = "smelt copper 2"
     SmeltGold1 = "smelt gold 1"
     SmeltGold2 = "smelt gold 2"
     SmeltIron1 = "smelt iron 1"
     SmeltIron2 = "smelt iron 2"
     SmeltLead1 = "smelt lead 1"
@@ -530,14 +560,17 @@
     SpinThread2 = "spin thread 2"
     SpinYarn1 = "spin yarn 1"
     SpinYarn2 = "spin yarn 2"
     SplitTimber1 = "split timber 1"
     SplitTimber2 = "split timber 2"
     TanHides1 = "tan hides 1"
     TanHides2 = "tan hides 2"
+    TrapFish1 = "trap fish 1"
+    TrapFish2 = "trap fish 2"
+    TrapFish3 = "trap fish 3"
     TumbrelOperations = "tumbrel operations"
     WeaveCloth1 = "weave cloth 1"
     WeaveCloth2a = "weave cloth 2a"
     WeaveCloth2b = "weave cloth 2b"
     WeaveCloth3a = "weave cloth 3a"
     WeaveCloth3b = "weave cloth 3b"
     WeaveCloth4a = "weave cloth 4a"
@@ -570,14 +603,15 @@
 
 
 class Transport(Enum):
     """Represents a transport."""
 
     Cog = "cog"
     Handcart = "handcart"
+    Hulk = "hulk"
     Snekkja = "snekkja"
     Tumbrel = "tumbrel"
 
 
 class Location(BaseModel):
     """Represents the location of something on the map.
```

### Comparing `pymerc-0.5.0/pymerc/api/models/map.py` & `pymerc-0.6.0/pymerc/api/models/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/models/player.py` & `pymerc-0.6.0/pymerc/api/models/player.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/models/static.py` & `pymerc-0.6.0/pymerc/api/models/static.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,10 +104,10 @@
     classes: Optional[list[common.Skill]] = []
     price: ItemPrice
 
 
 class ItemPrice(BaseModel):
     """Represents the price of an item in the game."""
 
-    low: float
+    low: Optional[float] = None
     typical: float
-    high: float
+    high: Optional[float] = None
```

### Comparing `pymerc-0.5.0/pymerc/api/models/towns.py` & `pymerc-0.6.0/pymerc/api/models/towns.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,19 @@
     """Represents the commoners in a town."""
 
     account_id: str
     count: int
     migration: float
     sustenance: list[TownDemandCategory]
 
+    @property
+    def demands(self) -> list[TownDemand]:
+        """The demands of the commoners."""
+        return [demand for category in self.sustenance for demand in category.products]
+
 
 class TownDemandCategory(BaseModel):
     """Represents a category of demands in a town."""
 
     name: str
     products: list[TownDemand]
```

### Comparing `pymerc-0.5.0/pymerc/api/models/transports.py` & `pymerc-0.6.0/pymerc/api/models/transports.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/static.py` & `pymerc-0.6.0/pymerc/api/static.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/towns.py` & `pymerc-0.6.0/pymerc/api/towns.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/api/transports.py` & `pymerc-0.6.0/pymerc/api/transports.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/game/building.py` & `pymerc-0.6.0/pymerc/game/building.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,50 @@
 
 from collections import UserList
 from typing import TYPE_CHECKING, Optional
 
 from pymerc.api.models import common
 from pymerc.api.models.buildings import Building as BuildingModel
 from pymerc.game.recipe import Recipe
+from pymerc.game.operation import BuildingOperation, Operation, OperationsList
 
 if TYPE_CHECKING:
     from pymerc.client import Client
+    from pymerc.game.player import Player
 
 
 class Building:
     """A higher level representation of a building in the game."""
 
     data: BuildingModel
+    player: Player
 
-    def __init__(self, client: Client, id: int):
+    def __init__(self, client: Client, player: Player, id: int):
         self._client = client
+        self.player = player
         self.id = id
 
     async def load(self):
         """Loads the data for the building."""
         self.data = await self._client.buildings_api.get(self.id)
-        self.operations_data = await self._client.buildings_api.get_operations(self.id)
+
+    @property
+    def building_operation(self) -> Optional[BuildingOperation]:
+        """Returns the building operation."""
+        return self.player.operations.get(self.id, None)
 
     @property
     def flows(self) -> Optional[dict[common.Item, common.InventoryFlow]]:
-        """The flows of the building."""
-        return self.operations_data.total_flow
+        """Returns the flows of the building."""
+        if self.building_operation.total_flow:
+            return self.building_operation.data.total_flow
+        elif self.operation:
+            return self.operation.data.flows
+        else:
+            return None
 
     @property
     def inventory(self) -> Optional[common.Inventory]:
         """Returns the inventory of the building."""
         if self.data and self.data.storage:
             return self.data.storage.inventory
         return None
@@ -42,24 +55,37 @@
         """Returns the items in the building's storage."""
         if self.data and self.data.storage:
             return self.data.storage.inventory.account.assets
         else:
             return None
 
     @property
+    def operation(self) -> Optional[Operation]:
+        """Returns the operation of the building."""
+        if len(self.operations) == 1:
+            return self.operations[0]
+        else:
+            return None
+
+    @property
+    def operations(self) -> Optional[OperationsList]:
+        """Returns the operations of the building."""
+        if self.id in self.player.operations:
+            if not self.player.operations[self.id].operations:
+                return self.player.storehouse.operations.by_building_id(self.id)
+
+            return self.player.operations[self.id].operations
+        return None
+
+    @property
     def managers(self) -> dict[common.Item, common.InventoryManager]:
         """The managers of the building."""
         return self.data.storage.inventory.managers
 
     @property
-    def operations(self) -> Optional[list[common.Operation]]:
-        """The operations of the building."""
-        return self.operations_data.operations
-
-    @property
     def previous_flows(self) -> Optional[dict[common.Item, common.InventoryFlow]]:
         """The flows of the building."""
         if self.data.storage:
             return self.data.storage.inventory.previous_flows
         else:
             return None
 
@@ -206,14 +232,29 @@
 
         return 0.0
 
 
 class BuildingsList(UserList):
     """A list of buildings."""
 
+    def by_id(self, id: int) -> Optional[Building]:
+        """Get a building by its ID.
+
+        Args:
+            id (int): The ID of the building.
+
+        Returns:
+            Building: The building with the given ID if it exists, otherwise None.
+        """
+        for building in self:
+            if building.id == id:
+                return building
+
+        return None
+
     def by_type(self, type: common.BuildingType) -> BuildingsList:
         """Get all buildings of a certain type.
 
         Args:
             type (BuildingType): The type of the buildings.
 
         Returns:
```

### Comparing `pymerc-0.5.0/pymerc/game/exports.py` & `pymerc-0.6.0/pymerc/game/exports.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/game/imports.py` & `pymerc-0.6.0/pymerc/game/imports.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/game/player.py` & `pymerc-0.6.0/pymerc/game/player.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 from pymerc.api.models import common, businesses
 from pymerc.api.models.player import Household, Sustenance
 from pymerc.api.models.player import Player as PlayerModel
 from pymerc.game.building import BuildingsList
 from pymerc.game.exports import ExportsList, ExportsSummed
 from pymerc.game.imports import ImportsList, ImportsSummed
+from pymerc.game.operation import (
+    BuildingOperation,
+    BuildingOperationsDict,
+    BuildingOperationList,
+)
 from pymerc.game.town import Town
 from pymerc.game.transport import Transport, TransportList
 
 if TYPE_CHECKING:
     from pymerc.client import Client
 
 
@@ -20,35 +25,46 @@
     """A higher level representation of a player in the game."""
 
     buildings: BuildingsList
     business: businesses.Business
     data: PlayerModel
     exports: ExportsSummed
     imports: ImportsSummed
+    operations: BuildingOperationsDict
     town: Town
     transports: list[Transport]
 
     def __init__(self, client: Client):
         self._client = client
         self.exports = ExportsSummed()
         self.imports = ImportsSummed()
 
     async def load(self):
         """Loads the data for the player."""
-        tasks = []
-
         self.data = await self._client.player_api.get()
         self.business = await self._client.businesses_api.get(
             self.data.household.business_ids[0]
         )
         self.town = await self._client.town(self.data.household.town_id)
 
         tasks = []
+        for operation in self.data.household.operations:
+            id = int(operation.split("/")[1])
+            tasks.append(self._client.building_operation(self, id))
+
+        self.operations = BuildingOperationsDict(
+            {
+                op.building_id: op
+                for op in BuildingOperationList(await asyncio.gather(*tasks))
+            }
+        )
+
+        tasks = []
         for id in self.business.building_ids:
-            tasks.append(self._client.building(id))
+            tasks.append(self._client.building(self, id))
         self.buildings = BuildingsList(await asyncio.gather(*tasks))
 
         tasks = []
         if self.business.transport_ids:
             for id in self.business.transport_ids:
                 tasks.append(self._client.transport(self, id))
         self.transports = TransportList(await asyncio.gather(*tasks))
```

### Comparing `pymerc-0.5.0/pymerc/game/recipe.py` & `pymerc-0.6.0/pymerc/game/recipe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
-from pymerc.api.models.common import InventoryAccountAsset, InventoryManager, Item
+from pymerc.api.models import common
+from pymerc.api.models.static import Ingredient
 from pymerc.api.models.static import Recipe as RecipeModel
 
 if TYPE_CHECKING:
     from pymerc.client import Client
 
 
 class Recipe:
-    def __init__(self, client: Client, recipe_name: str):
+    """A higher level representation of a recipe in the game."""
+
+    data: RecipeModel
+
+    def __init__(self, client: Client, recipe: RecipeModel):
         self._client = client
-        self.recipe_name = recipe_name
-        self.data: Optional[RecipeModel] = None
+        self.data = recipe
 
     async def load(self):
-        """Loads the data for the recipe and calculates labor required."""
-        recipes = await self._client.static_api.get_recipes()
-        for recipe in recipes:
-            if recipe.name.value == self.recipe_name:
-                self.data = recipe
-        if self.data is None:
-            raise ValueError(f"Recipe {self.recipe_name} not found")
+        """Loads the data for the recipe"""
+        pass
+
+    @property
+    def inputs(self) -> dict[common.Item, Ingredient]:
+        """The inputs of the recipe."""
+        return {ingredient.product: ingredient for ingredient in self.data.inputs}
+
+    @property
+    def outputs(self) -> dict[common.Item, Ingredient]:
+        """The outputs of the recipe."""
+        return {ingredient.product: ingredient for ingredient in self.data.outputs}
 
     @property
     def labour(self) -> float:
         """Calculates the labor required for the recipe."""
         for input_ingredient in self.data.inputs:
-            if input_ingredient.product == Item.Labour:
+            if input_ingredient.product == common.Item.Labour:
                 return input_ingredient.amount
         return 0.0
 
     def calculate_target_labor(
         self,
         target: float,
-        inventory_assets: Optional[dict[Item, InventoryAccountAsset]] = {},
-        inventory_managers: Optional[dict[Item, InventoryManager]] = {},
+        inventory_assets: Optional[
+            dict[common.Item, common.InventoryAccountAsset]
+        ] = {},
+        inventory_managers: Optional[dict[common.Item, common.InventoryManager]] = {},
     ) -> float:
         """Calculates the labor required for the given target multiplier.
 
         Args:
             target (float): The target percentage multiplier for the recipe.
             inventory_assets (Optional[List[InventoryAccountAsset]]): The list of inventory assets.
             inventory_managers (Optional[List[InventoryManager]]): The list of inventory managers.
```

### Comparing `pymerc-0.5.0/pymerc/game/storehouse.py` & `pymerc-0.6.0/pymerc/game/storehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TYPE_CHECKING, Optional
 
 from pymerc.api.models import common
 from pymerc.api.models.towns import TownMarketItem, TownMarketItemDetails
 from pymerc.game.building import Building
 from pymerc.game.exports import ExportsList
 from pymerc.game.imports import ImportsList
+from pymerc.game.operation import OperationsList
 
 if TYPE_CHECKING:
     from pymerc.client import Client
     from pymerc.game.player import Player
 
 
 class Storehouse:
@@ -38,15 +39,20 @@
 
     @property
     def flows(self) -> dict[common.Item, common.InventoryFlow]:
         """The flows of the storehouse."""
         return self.data.flows
 
     @property
-    def operations(self) -> Optional[list[common.Operation]]:
+    def id(self) -> int:
+        """The id of the storehouse."""
+        return self.data.id
+
+    @property
+    def operations(self) -> OperationsList:
         """The operations of the storehouse."""
         return self.data.operations
 
     @property
     def previous_flows(self) -> dict[common.Item, common.InventoryFlow]:
         """The previous flows of the storehouse."""
         return self.data.previous_flows
```

### Comparing `pymerc-0.5.0/pymerc/game/town.py` & `pymerc-0.6.0/pymerc/game/town.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,24 @@
 
     async def load(self):
         """Loads the data for the town."""
         self.data = await self._client.towns_api.get_data(self.id)
         self._market = await self._client.towns_api.get_market_data(self.id)
 
     @property
+    def commoners(self) -> models.TownCommoners:
+        """The commoners in the town."""
+        return self.data.commoners
+
+    @property
+    def demands(self) -> list[models.TownDemand]:
+        """The demands of commoners in the town."""
+        return self.data.commoners.demands
+
+    @property
     def market(self) -> dict[str, models.TownMarketItem]:
         """The market data for the town."""
         return self._market.markets
 
     @property
     def name(self) -> str:
         """The name of the town."""
```

### Comparing `pymerc-0.5.0/pymerc/game/transport.py` & `pymerc-0.6.0/pymerc/game/transport.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/util/data.py` & `pymerc-0.6.0/pymerc/util/data.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pymerc/util/towns.py` & `pymerc-0.6.0/pymerc/util/towns.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.5.0/pyproject.toml` & `pymerc-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymerc"
-version = "0.5.0"
+version = "0.6.0"
 description = "A Python library for interacting with the Mercatorio browser based game"
 authors = ["Joshua Gilman <joshuagilman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jmgilman/pymerc"
 keywords = ["mercatorio", "python", "library", "game"]
 packages = [{ include = "pymerc" }]
```

### Comparing `pymerc-0.5.0/PKG-INFO` & `pymerc-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymerc
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for interacting with the Mercatorio browser based game
 Home-page: https://github.com/jmgilman/pymerc
 License: MIT
 Keywords: mercatorio,python,library,game
 Author: Joshua Gilman
 Author-email: joshuagilman@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -131,14 +131,49 @@
 >>> player.storehouse.items[Item.Cloth].balance
 1477.096
 >>> await tr.exports[Item.Cloth].sell(1, 8.99)
 >>> player.storehouse.items[Item.Cloth].balance
 1476.096
 ```
 
+#### Operations
+
+Get the operations for all of our weaveries:
+
+```python
+>>> from pymerc.api.models.common import BuildingType
+>>> player.operations.by_building_type(BuildingType.Weavery)
+OperationsList([<pymerc.game.operation.Operation at 0x7ffbb00de6f0>])
+```
+
+We have a single operation going on associated with a weavery.
+Check how much it is currently outputting:
+
+```python
+>>> player.operations.by_building_type(BuildingType.Weavery).outputs
+{<Item.Cloth: 'cloth'>: 400.0}
+```
+
+Check all of our operations that are taking cloth as an input:
+
+```python
+>>> player.operations.by_item_input(Item.Cloth)
+OperationsList([<pymerc.game.operation.Operation at 0x7ffbb00debd0>,
+                <pymerc.game.operation.Operation at 0x7ffbb00dede0>,
+                <pymerc.game.operation.Operation at 0x7ffbb00dee70>,
+                <pymerc.game.operation.Operation at 0x7ffbb00dcf80>])
+```
+
+Check how much cloth all of these operations are consuming in total:
+
+```python
+>>> player.operations.by_item_input(Item.Cloth).inputs[Item.Cloth]
+197.0
+```
+
 #### Data Analysis
 
 Compare our total and actual imports:
 
 ```python
 >>> player.imports.volume
 426
```

