# Comparing `tmp/hbv-1.5.0.tar.gz` & `tmp/hbv-1.5.2.tar.gz`

## Comparing `hbv-1.5.0.tar` & `hbv-1.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 hbv-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.5.0/Dockerfile
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.5.0/MANIFEST.in
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/Forcing.txt
--rw-r--r--   0        0        0   525026 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/Forward model.ipynb
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/HBV_config.json
--rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/HBV_forcing.nc
--rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/Q_m_out_ref.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/model_layout.png
--rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 hbv-1.5.0/src/HBV/HBV_bmi.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.5.0/src/HBV/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.5.0/src/HBV/utils.py
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hbv-1.5.0/README.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 hbv-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hbv-1.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.5.2/Dockerfile
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.5.2/MANIFEST.in
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.5.2/docs/Forcing.txt
+-rw-r--r--   0        0        0   525026 2020-02-02 00:00:00.000000 hbv-1.5.2/docs/Forward model.ipynb
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.5.2/docs/HBV_config.json
+-rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.5.2/docs/HBV_forcing.nc
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.5.2/docs/Q_m_out_ref.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.5.2/docs/model_layout.png
+-rw-r--r--   0        0        0    20193 2020-02-02 00:00:00.000000 hbv-1.5.2/src/HBV/HBV_bmi.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hbv-1.5.2/src/HBV/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.5.2/src/HBV/utils.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hbv-1.5.2/README.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 hbv-1.5.2/PKG-INFO
```

### Comparing `hbv-1.5.0/CHANGELOG.md` & `hbv-1.5.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -17,8 +17,14 @@
 ### v1.3.2
 - typo in update updating_dict_var_obj: was getting values wrong 
 ## V1.4.0
 - adding snow reservoir
 ### V1.4.1
 - bug fix in naming of values 
 ## v1.5.0
-  - Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
+- Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
+### v1.5.1
+- Groundwater and overland flow now can no longer be negative   
+### v1.5.2
+- now loads forcing as xarray and then immediately stores the values as numpy arrays in memory. This might be less 
+efficient as xarray takes care of lazy loading in the background. 
+But on long runs using data assimilation the lazy loading seemed to cause issues
```

### Comparing `hbv-1.5.0/Dockerfile` & `hbv-1.5.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/.github/workflows/python-publish.yml` & `hbv-1.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/docs/Forcing.txt` & `hbv-1.5.2/docs/Forcing.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/docs/Forward model.ipynb` & `hbv-1.5.2/docs/Forward model.ipynb`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/docs/HBV_forcing.nc` & `hbv-1.5.2/docs/HBV_forcing.nc`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/docs/Q_m_out_ref.txt` & `hbv-1.5.2/docs/Q_m_out_ref.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/docs/model_layout.png` & `hbv-1.5.2/docs/model_layout.png`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/src/HBV/HBV_bmi.py` & `hbv-1.5.2/src/HBV/HBV_bmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,31 @@
             'initial_storage' list of 4 storage parameters split by a ','
 
         """
         # open json files containing data
         self.config: dict[str, Any] = utils.read_config(config_file)
 
         # store forcing & obs
-        self.P = utils.load_var(self.config["precipitation_file"], "pr")
+        self.ds_P = utils.load_var(self.config["precipitation_file"], "pr")
+        self.P = self.ds_P.to_numpy()
 
-        self.EP = utils.load_var(self.config["potential_evaporation_file"], "evspsblpot")
+        self.ds_EP = utils.load_var(self.config["potential_evaporation_file"], "evspsblpot")
+        self.EP = self.ds_EP.to_numpy()
 
-        self.Tmean = utils.load_var(self.config["mean_temperature_file"], "tas")
+        self.ds_Tmean = utils.load_var(self.config["mean_temperature_file"], "tas")
+        self.Tmean = self.ds_Tmean.to_numpy()
 
         # set up times
-        self.time = self.P['time'].astype("datetime64[s]")
-        self.end_timestep = len(self.time.values)
+        self.time = self.ds_P['time'].astype("datetime64[s]").to_numpy()
+        self.end_timestep = len(self.time)
         self.current_timestep = 0
 
         # time step size in seconds (to be able to do unit conversions) - change here to days
         self.dt = (
-                          self.time.values[1] - self.time.values[0]
+                          self.time[1] - self.time[0]
                   ) / np.timedelta64(1, "s") / 24 / 3600
 
         # define parameters 
         self.set_pars(np.array(self.config['parameters'].split(','), dtype=np.float64))
 
         # add memory vector for tlag & run weights function
         self.memory_vector_lag = self.set_empty_memory_vector_lag()
@@ -107,17 +110,17 @@
             Function to run the update part of one timestep of the HBV model
             par: array/list containing 9 parameters: Imax,  Ce,  Sumax, beta,  Pmax,  T_lag,   Kf,   Ks, Fm (floats)
             s_in: array/list containing 5 storage terms which are input to the timestep: Si,  Su, Sf, Ss,Sp (floats)
             storage_terms: list of arrays which store: Si, Su, Sf, Ss,Sp, Ei_dt, Ea_dt, Qs_dt_lst, Qf_dt_lst, Q_tot_dt
             step_n - nth step which formard model takes: used to determin which Precipitaion & evaporation to use
         """
         if self.current_timestep < self.end_timestep:
-            self.P_dt = self.P.isel(time=self.current_timestep).to_numpy() * self.dt
-            self.Ep_dt = self.EP.isel(time=self.current_timestep).to_numpy() * self.dt
-            self.Tmean_i = self.Tmean.isel(time=self.current_timestep).to_numpy() * self.dt
+            self.P_dt = self.P[self.current_timestep] * self.dt
+            self.Ep_dt = self.EP[self.current_timestep]  * self.dt
+            self.Tmean_i = self.Tmean[self.current_timestep]  * self.dt
 
             # split P into rain and snow:
             if self.Tmean_i < self.Tt:
                 self.Pr = 0  # if snowing, no rainfall
                 self.Ps = self.P_dt  # all precip goes into snow
                 self.M_dt = 0  # too cold to meld
                 self.Sp += self.Ps
@@ -158,20 +161,20 @@
 
             # Percolation
             Qus_dt = self.P_max * (self.Su / self.Su_max) * self.dt  # Flux from Su to Ss
             self.Su = self.Su - Qus_dt
 
             # Fast Reservoir
             self.Sf = self.Sf + Quf_dt
-            self.Qf_dt = self.dt * self.Kf * self.Sf
+            self.Qf_dt = max(self.dt * self.Kf * self.Sf, 0)
             self.Sf = self.Sf - self.Qf_dt
 
             # Slow Reservoir
             self.Ss = self.Ss + Qus_dt
-            self.Qs_dt = self.Ss * self.Ks * self.dt
+            self.Qs_dt = max(self.Ss * self.Ks * self.dt, 0)
             self.Ss = self.Ss - self.Qs_dt
 
             # total = fast + slow
             self.Q_tot_dt = self.Qs_dt + self.Qf_dt
             # add time lag to the process - Qm is set here
             self.add_time_lag()
             # self.Q = self.Q_tot_dt
@@ -342,33 +345,33 @@
     # this doesn't update the obj...
     def get_output_var_names(self) -> Tuple[str]:
         return tuple([str(key) for key in DICT_VAR_UNITS.keys()])
 
     # The BMI has to have some time-related functionality:
     def get_start_time(self) -> float:
         """Return end time in seconds since 1 january 1970."""
-        return get_unixtime(self.time.isel(time=0).values)  # type: ignore
+        return get_unixtime(self.time[0])  # type: ignore
 
     def get_end_time(self) -> float:
         """Return end time in seconds since 1 january 1970."""
-        return get_unixtime(self.time.isel(time=-1).values)  # type: ignore
+        return get_unixtime(self.time[-1])  # type: ignore
 
     def get_current_time(self) -> float:
         """Return current time in seconds since 1 january 1970."""
         # we get the timestep from the data, but the stopping condition requires it to go one beyond. 
-        return get_unixtime(self.time.isel(time=self.current_timestep).values)  # type: ignore
+        return get_unixtime(self.time[self.current_timestep])  # type: ignore
 
     def set_tlag(self, T_lag_in) -> int:
         """Ensures T_lag is an integer of at minimum 1"""
         T_lag = max(1, int(round(T_lag_in, 0)))
         return T_lag
 
     def get_time_step(self) -> float:
         if len(self.time) > 1:
-            return float((self.time.values[1] - self.time.values[0]) / np.timedelta64(1, "s"))
+            return float((self.time[1] - self.time[0]) / np.timedelta64(1, "s"))
         else:
             message = "No time series defined"
             warnings.warn(message=message, category=ImportWarning)
             return 0.0
 
     def get_time_units(self) -> str:
         return "seconds since 1970-01-01 00:00:00.0 +0000"
@@ -411,19 +414,19 @@
 
     def get_grid_origin(self, grid: int, origin: np.ndarray) -> np.ndarray:
         origin[:] = np.array([0., 0.])
         return origin
 
     # Non-uniform rectilinear, curvilinear
     def get_grid_x(self, grid: int, x: np.ndarray) -> np.ndarray:
-        x[:] = self.P["lon"].to_numpy()
+        x[:] = self.ds_P["lon"].to_numpy()
         return x
 
     def get_grid_y(self, grid: int, y: np.ndarray) -> np.ndarray:
-        y[:] = self.P["lat"].to_numpy()
+        y[:] = self.ds_P["lat"].to_numpy()
         return y
 
     def finalize(self) -> None:
         """"Nothing to wrapup"""
         pass
 
     # not implemented & not planning to
```

### Comparing `hbv-1.5.0/src/HBV/utils.py` & `hbv-1.5.2/src/HBV/utils.py`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/LICENSE.txt` & `hbv-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/README.md` & `hbv-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hbv-1.5.0/pyproject.toml` & `hbv-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "HBV"
 description = "Dev version for a HBV hydrological model using BMI for eWaterCycle."
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.5.0"
+version = "1.5.2"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 
 # Include here only the dependencies for the BMI Model
 # This is used to run the BmiModel inside the container
 dependencies = [
```

### Comparing `hbv-1.5.0/PKG-INFO` & `hbv-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: HBV
-Version: 1.5.0
+Version: 1.5.2
 Summary: Dev version for a HBV hydrological model using BMI for eWaterCycle.
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Requires-Dist: bmipy
 Requires-Dist: netcdf4
 Requires-Dist: numpy
```

