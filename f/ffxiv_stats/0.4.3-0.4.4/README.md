# Comparing `tmp/ffxiv_stats-0.4.3.tar.gz` & `tmp/ffxiv_stats-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffxiv_stats-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ffxiv_stats-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ffxiv_stats-0.4.3.tar` & `ffxiv_stats-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      106 2023-12-24 23:30:17.666831 ffxiv_stats-0.4.3/.gitignore
--rw-r--r--   0        0        0    11558 2023-08-06 18:15:32.993652 ffxiv_stats-0.4.3/LICENSE
--rw-r--r--   0        0        0     4996 2024-02-04 04:04:49.060347 ffxiv_stats-0.4.3/README.md
--rw-r--r--   0        0        0   262348 2024-02-04 03:52:04.000902 ffxiv_stats-0.4.3/examples/deterministic-rotations.ipynb
--rw-r--r--   0        0        0    51264 2023-11-03 01:32:29.636143 ffxiv_stats-0.4.3/examples/smn-rotation-comparison/fryte-results.csv
--rw-r--r--   0        0        0   501435 2023-11-03 01:32:29.639995 ffxiv_stats-0.4.3/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb
--rw-r--r--   0        0        0    20959 2023-11-03 01:32:29.641016 ffxiv_stats-0.4.3/examples/smn-rotation-comparison/smn-rotation.csv
--rw-r--r--   0        0        0  1620366 2024-02-04 03:52:04.014901 ffxiv_stats-0.4.3/examples/stochastic-rotations.ipynb
--rw-r--r--   0        0        0      441 2024-04-06 23:50:19.430834 ffxiv_stats-0.4.3/ffxiv_stats/__init__.py
--rw-r--r--   0        0        0    28657 2024-04-06 23:50:13.641192 ffxiv_stats-0.4.3/ffxiv_stats/jobs.py
--rw-r--r--   0        0        0      299 2023-12-24 23:30:17.668826 ffxiv_stats-0.4.3/ffxiv_stats/modifiers.py
--rw-r--r--   0        0        0    47554 2024-02-07 03:43:11.874269 ffxiv_stats-0.4.3/ffxiv_stats/moments.py
--rw-r--r--   0        0        0     6564 2024-02-04 03:52:04.023903 ffxiv_stats-0.4.3/ffxiv_stats/rate.py
--rw-r--r--   0        0        0      593 2024-01-10 06:09:20.789049 ffxiv_stats-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 ffxiv_stats-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      106 2023-12-24 23:30:17.666831 ffxiv_stats-0.4.4/.gitignore
+-rw-r--r--   0        0        0    11558 2023-08-06 18:15:32.993652 ffxiv_stats-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4996 2024-02-04 04:04:49.060347 ffxiv_stats-0.4.4/README.md
+-rw-r--r--   0        0        0   262348 2024-02-04 03:52:04.000902 ffxiv_stats-0.4.4/examples/deterministic-rotations.ipynb
+-rw-r--r--   0        0        0    51264 2023-11-03 01:32:29.636143 ffxiv_stats-0.4.4/examples/smn-rotation-comparison/fryte-results.csv
+-rw-r--r--   0        0        0   501435 2023-11-03 01:32:29.639995 ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb
+-rw-r--r--   0        0        0    20959 2023-11-03 01:32:29.641016 ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation.csv
+-rw-r--r--   0        0        0  1620366 2024-02-04 03:52:04.014901 ffxiv_stats-0.4.4/examples/stochastic-rotations.ipynb
+-rw-r--r--   0        0        0      441 2024-04-14 19:52:38.808900 ffxiv_stats-0.4.4/ffxiv_stats/__init__.py
+-rw-r--r--   0        0        0    30195 2024-04-14 19:51:14.746010 ffxiv_stats-0.4.4/ffxiv_stats/jobs.py
+-rw-r--r--   0        0        0      299 2023-12-24 23:30:17.668826 ffxiv_stats-0.4.4/ffxiv_stats/modifiers.py
+-rw-r--r--   0        0        0    47554 2024-02-07 03:43:11.874269 ffxiv_stats-0.4.4/ffxiv_stats/moments.py
+-rw-r--r--   0        0        0     6564 2024-02-04 03:52:04.023903 ffxiv_stats-0.4.4/ffxiv_stats/rate.py
+-rw-r--r--   0        0        0      593 2024-01-10 06:09:20.789049 ffxiv_stats-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 ffxiv_stats-0.4.4/PKG-INFO
```

### Comparing `ffxiv_stats-0.4.3/LICENSE` & `ffxiv_stats-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/README.md` & `ffxiv_stats-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/examples/deterministic-rotations.ipynb` & `ffxiv_stats-0.4.4/examples/deterministic-rotations.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/examples/smn-rotation-comparison/fryte-results.csv` & `ffxiv_stats-0.4.4/examples/smn-rotation-comparison/fryte-results.csv`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb` & `ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/examples/smn-rotation-comparison/smn-rotation.csv` & `ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation.csv`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/examples/stochastic-rotations.ipynb` & `ffxiv_stats-0.4.4/examples/stochastic-rotations.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/ffxiv_stats/jobs.py` & `ffxiv_stats-0.4.4/ffxiv_stats/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     ) -> None:
         """
         Base class for converting potency to base damage dealt. Not meant to be used alone.
         Instead use a `ROLE` class, which inherits this class and applies/sets the correct attributes and stats.
         """
         # Level dependent parameters
         # currently for lvl 90
+        self.level = level
         self.lvl_main = level_mod[level]["lvl_main"]
         self.lvl_sub = level_mod[level]["lvl_sub"]
         self.lvl_div = level_mod[level]["lvl_div"]
         self.job_attribute = 115
         self.atk_mod = 195
 
         self.main_stat = main_stat
@@ -430,15 +431,19 @@
 
         inputs:
         potency - int, potency of an attack
         ap_adjust - int, amount of main stat to add. Used to account for medication.
         """
         d1 = nf(nf(nf(potency * self.pet_f_atk(ap_adjust) * self.f_det()) / 100) / 1000)
 
-        return nf(nf(nf(nf(nf(d1 * self.f_ten()) / 1000) * self.pet_f_wd()) / 100) * self.trait / 100)
+        return nf(
+            nf(nf(nf(nf(d1 * self.f_ten()) / 1000) * self.pet_f_wd()) / 100)
+            * self.trait
+            / 100
+        )
 
 
 class Healer(BaseStats):
     def __init__(
         self,
         mind: int,
         strength: int,
@@ -501,16 +506,19 @@
             pet_attack_power_offset=pet_attack_power_offset,
             pet_job_attribute=pet_job_attribute,
             pet_atk_mod=pet_atk_mod,
             level=level,
         )
 
         self.auto_trait = 100
-        self.atk_mod = 195
-        self.job_attribute = 115
+
+        if level == 90:
+            self.atk_mod = 195
+        if level == 80:
+            self.atk_mod = 165
 
         self.dot_speed_stat = spell_speed
         self.auto_speed_stat = 400
         self.add_role("Healer")
 
         if (
             (dexterity is not None)
@@ -533,15 +541,15 @@
         tenacity: int,
         crit_stat: int,
         dh_stat: int,
         weapon_damage: int,
         delay: float,
         job: str,
         pet_attack_power: int = None,
-        pet_attack_power_scalar: float = 1.,
+        pet_attack_power_scalar: float = 1.0,
         pet_attack_power_offset: int = -18,
         pet_job_attribute: int = 100,
         pet_atk_mod: int = 195,
         level: int = 90,
     ) -> None:
         """Set tank stats, most notably the attack modifier.
 
@@ -666,14 +674,19 @@
 
         self.add_role("Caster")
 
         self.auto_trait = 100
         self.dot_speed_stat = spell_speed
         self.auto_speed_stat = 400
 
+        if level == 90:
+            self.atk_mod = 195
+        if level == 80:
+            self.atk_mod = 165
+
         pass
 
 
 # class PhysicalRanged(BaseStats):
 #     def __init__(self, mind, intelligence, vitality, strength, dexterity, det,
 #                  skill_speed, spell_speed, tenacity, crit_stat, dh_stat, weapon_damage, delay, level=90) -> None:
 #         """
@@ -700,49 +713,92 @@
 #         self.add_role('Physical Ranged')
 
 #         self.skill_speed = skill_speed
 #         self.spell_speed = spell_speed
 #         pass
 
 
-# class Melee(BaseStats):
-#     def __init__(self, mind, intelligence, vitality, strength, dexterity,
-#                  det, skill_speed, spell_speed, tenacity, crit_stat, dh_stat, weapon_damage, delay, level=90) -> None:
-#         """
-#         Set melee-specific stats with this class like main stat, traits, etc.
+class Melee(BaseStats):
+    def __init__(
+        self,
+        main_stat: int,
+        det: int,
+        skill_speed: int,
+        crit_stat: int,
+        dh_stat: int,
+        weapon_damage: int,
+        delay: float,
+        job: str,
+        pet_attack_power: int = None,
+        pet_attack_power_scalar: float = 1.,
+        pet_attack_power_offset: int = 0,
+        pet_job_attribute: int = 100,
+        pet_atk_mod: int = 195,
+        level: int = 90,
+    ) -> None:
+        """
+        Set melee-specific stats with this class like main stat, traits, etc.
 
-#         inputs:
-#         mind - int, mind stat
-#         intelligence - int, intelligence stat
-#         vitality - int, vitality stat
-#         strength, - int, strength stat
-#         dexterity - int, strength stat
-#         det - int, determination stat
-#         skill_speed - int, skill speed stat
-#         spell_speed - int, spell speed stat
-#         tenacity - tenacity stat
-#         crit_stat - critical hit stat
-#         dh_stat - direct hit rate stat
-#         weapon_damage - weapon damage stat
-#         delay - weapon delay stat
-#         """
-#         super().__init__(strength, 100, strength, mind, intelligence, vitality, strength, dexterity,
-#                          det, tenacity, crit_stat, dh_stat, skill_speed, skill_speed, weapon_damage, delay, level=90)
+        inputs:
+        mind - int, mind stat
+        intelligence - int, intelligence stat
+        vitality - int, vitality stat
+        strength, - int, strength stat
+        dexterity - int, strength stat
+        det - int, determination stat
+        skill_speed - int, skill speed stat
+        spell_speed - int, spell speed stat
+        tenacity - tenacity stat
+        crit_stat - critical hit stat
+        dh_stat - direct hit rate stat
+        weapon_damage - weapon damage stat
+        delay - weapon delay stat
+        """
+        super().__init__(
+            attack_power=main_stat,
+            trait=100,
+            main_stat=main_stat,
+            strength=main_stat if job != "Ninja" else 300,
+            det=det,
+            crit_stat=crit_stat,
+            dh_stat=dh_stat,
+            dot_speed_stat=skill_speed,
+            auto_speed_stat=400,
+            weapon_damage=weapon_damage,
+            delay=delay,
+            pet_attack_power=pet_attack_power,
+            pet_attack_power_scalar=pet_attack_power_scalar,
+            pet_attack_power_offset=pet_attack_power_offset,
+            pet_job_attribute=pet_job_attribute,
+            pet_atk_mod=pet_atk_mod,
+            level=level,
+        )
 
-#         self.add_role('Melee')
+        self.add_role("Melee")
+
+        self.auto_trait = 100
+        self.dot_speed_stat = skill_speed
+        self.auto_speed_stat = skill_speed
+
+        if level == 90:
+            self.atk_mod = 195
+        if level == 80:
+            self.atk_mod = 165
+
+        self.job = job
+
+        if job not in ("Monk", "Dragoon", "Reaper", "Ninja", "Samurai"):
+            raise ValueError("Invalid job, accepted values are {'Monk', 'Dragoon', 'Reaper', 'Ninja', 'Samurai'}")
+
+        if job in ("Monk", "Ninja"):
+            self.job_attribute = 110
+        # But why
+        elif job == "Samurai":
+            self.job_attribute = 112
+        else:
+            self.job_attribute = 115
 
-#         self.skill_speed = skill_speed
-#         self.spell_speed = spell_speed
 
 if __name__ == "__main__":
-    a = MagicalRanged(
-        3369,
-        190,
-        2136,
-        500,
-        2399,
-        796,
-        132,
-        3.22,
-        3369
-    )
+    # a = MagicalRanged(3369, 190, 2136, 500, 2399, 796, 132, 3.22, 3369)
+    a = Melee(3360, 1697, 400, 2554, 1697, 132, 2.44, "Ninja", 3360, 1)
     pass
```

### Comparing `ffxiv_stats-0.4.3/ffxiv_stats/moments.py` & `ffxiv_stats-0.4.4/ffxiv_stats/moments.py`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/ffxiv_stats/rate.py` & `ffxiv_stats-0.4.4/ffxiv_stats/rate.py`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/pyproject.toml` & `ffxiv_stats-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.3/PKG-INFO` & `ffxiv_stats-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffxiv_stats
-Version: 0.4.3
+Version: 0.4.4
 Summary: Compute damage variability in the critically acclaimed MMORPG Final Fantasy XIV.
 Author-email: Acerola Paracletus <ffxivacerola@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: numpy >= 1.20.2
 Requires-Dist: matplotlib >= 3.4.2
```

