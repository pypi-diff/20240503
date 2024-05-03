# Comparing `tmp/tabcorr-1.0.1.tar.gz` & `tmp/tabcorr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabcorr-1.0.1.tar", last modified: Sat Feb 25 00:04:08 2023, max compression
+gzip compressed data, was "tabcorr-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tabcorr-1.0.1.tar` & `tabcorr-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1111 2023-02-25 00:00:22.553902 tabcorr-1.0.1/LICENSE
--rw-r--r--   0        0        0     3922 2023-02-25 00:00:22.553902 tabcorr-1.0.1/README.md
--rw-r--r--   0        0        0      502 2023-02-25 00:00:22.553902 tabcorr-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      237 2023-02-25 00:01:17.124363 tabcorr-1.0.1/tabcorr/__init__.py
--rw-r--r--   0        0        0     4408 2023-02-25 00:00:22.555902 tabcorr-1.0.1/tabcorr/aa_cosmos.txt
--rw-r--r--   0        0        0      762 2023-02-25 00:00:22.555902 tabcorr-1.0.1/tabcorr/aa_test_cosmos.txt
--rw-r--r--   0        0        0    22083 2023-02-25 00:00:22.556902 tabcorr-1.0.1/tabcorr/as_cosmos.csv
--rw-r--r--   0        0        0     6933 2023-02-25 00:00:22.556902 tabcorr-1.0.1/tabcorr/corrfunc.py
--rw-r--r--   0        0        0    10008 2023-02-25 00:00:22.556902 tabcorr-1.0.1/tabcorr/database.py
--rw-r--r--   0        0        0    11586 2023-02-25 00:00:22.556902 tabcorr-1.0.1/tabcorr/interpolate.py
--rw-r--r--   0        0        0    37791 2023-02-25 00:00:42.980701 tabcorr-1.0.1/tabcorr/tabcorr.py
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 tabcorr-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-08-09 17:54:24.054695 tabcorr-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3922 2024-05-03 18:13:15.117337 tabcorr-1.1.0/README.md
+-rw-r--r--   0        0        0      510 2024-05-03 19:35:24.461885 tabcorr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      238 2024-05-03 19:33:32.149720 tabcorr-1.1.0/tabcorr/__init__.py
+-rw-r--r--   0        0        0     4408 2023-08-09 17:54:24.055695 tabcorr-1.1.0/tabcorr/aa_cosmos.txt
+-rw-r--r--   0        0        0      762 2023-08-09 17:54:24.055695 tabcorr-1.1.0/tabcorr/aa_test_cosmos.txt
+-rw-r--r--   0        0        0    22083 2023-08-09 17:54:24.055695 tabcorr-1.1.0/tabcorr/as_cosmos.csv
+-rw-r--r--   0        0        0     6933 2023-08-09 17:54:24.055695 tabcorr-1.1.0/tabcorr/corrfunc.py
+-rw-r--r--   0        0        0     9333 2024-05-03 19:23:40.005634 tabcorr-1.1.0/tabcorr/database.py
+-rw-r--r--   0        0        0    14077 2024-05-03 19:12:49.028049 tabcorr-1.1.0/tabcorr/interpolator.py
+-rw-r--r--   0        0        0    38056 2024-05-03 19:12:49.028049 tabcorr-1.1.0/tabcorr/tabcorr.py
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 tabcorr-1.1.0/PKG-INFO
```

### Comparing `tabcorr-1.0.1/LICENSE` & `tabcorr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tabcorr-1.0.1/README.md` & `tabcorr-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tabcorr-1.0.1/tabcorr/aa_cosmos.txt` & `tabcorr-1.1.0/tabcorr/aa_cosmos.txt`

 * *Files identical despite different names*

### Comparing `tabcorr-1.0.1/tabcorr/aa_test_cosmos.txt` & `tabcorr-1.1.0/tabcorr/aa_test_cosmos.txt`

 * *Files identical despite different names*

### Comparing `tabcorr-1.0.1/tabcorr/as_cosmos.csv` & `tabcorr-1.1.0/tabcorr/as_cosmos.csv`

 * *Files identical despite different names*

### Comparing `tabcorr-1.0.1/tabcorr/corrfunc.py` & `tabcorr-1.1.0/tabcorr/corrfunc.py`

 * *Files identical despite different names*

### Comparing `tabcorr-1.0.1/tabcorr/database.py` & `tabcorr-1.1.0/tabcorr/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Module providing database capabilities."""
 
-import os
 import numpy as np
+import os
+
 from astropy import units as u
 from astropy.table import Table
-from . import TabCorr, Interpolator
 from astropy.cosmology import Flatw0waCDM, FlatwCDM, Planck15
+from pathlib import Path
+
+from . import Interpolator
 
 
 def configuration(config_str):
     """Describe the tabulation configuration used.
 
     Parameters
     ----------
@@ -64,59 +67,37 @@
             if config in config_dict[parameter].keys():
                 config_dict[parameter] = config_dict[parameter][config]
                 break
 
     return config_dict
 
 
-def directory():
-    """Return the TabCorr database directory.
-
-    Returns
-    -------
-    dir : str
-        The TabCorr database directory.
-
-    Raises
-    ------
-    RuntimeError
-        If the TABCORR_DATABASE environment variable is not set.
-
-    """
-    try:
-        return os.environ['TABCORR_DATABASE']
-    except KeyError:
-        raise RuntimeError(
-            "You must set the TABCORR_DATABASE environment variable.")
-
-
 def cosmology(suite, i_cosmo=0):
     """Return the cosmology of a given simulation.
 
     Parameters
     ----------
     suite : str
         The simulation suite.
     i_cosmo : int, optional
         Number corresponding to the cosmology. Default is 0.
 
     Returns
     -------
-    cosmo : str
+    cosmo : astropy.cosmology.Cosmology
         The TabCorr database directory.
 
     Raises
     ------
     ValueError
         If the an unkown simulation or cosmology number is requested.
 
     """
     if suite == 'AbacusSummit':
-        table = Table.read(os.path.join(
-            os.path.dirname(os.path.realpath(__file__)), 'as_cosmos.csv'))
+        table = Table.read(Path(__file__).absolute().parent / 'as_cosmos.csv')
         table['i_cosmo'] = np.array([r[-3:] for r in table['root']], dtype=int)
         if i_cosmo not in table['i_cosmo']:
             raise ValueError('Cosmology number {} not in AbacusSummit.'.format(
                 i_cosmo))
         cosmo_dict = dict(table[table['i_cosmo'] == i_cosmo][0])
         h = cosmo_dict['h']
         omega_m = cosmo_dict['omega_b'] + cosmo_dict['omega_cdm']
@@ -128,22 +109,21 @@
             m_nu.append(0 * u.eV)
         return Flatw0waCDM(
             H0=h * 100, Om0=omega_m / h**2, Ob0=cosmo_dict['omega_b'] / h**2,
             w0=cosmo_dict['w0_fld'], wa=cosmo_dict['wa_fld'], Neff=n_eff,
             m_nu=m_nu, Tcmb0=2.7255 * u.K)
 
     elif suite == 'AemulusAlpha':
-        path = os.path.dirname(os.path.realpath(__file__))
+        path = Path(__file__).absolute().parent
         if i_cosmo >= 0 and i_cosmo < 40:
             cosmo_dict = dict(Table.read(
-                os.path.join(path, 'aa_cosmos.txt'), format='ascii')[i_cosmo])
+                path / 'aa_cosmos.txt', format='ascii')[i_cosmo])
         elif i_cosmo >= 0 and i_cosmo < 47:
-            cosmo_dict = dict(Table.read(
-                os.path.join(path, 'aa_test_cosmos.txt'), format='ascii')[
-                    i_cosmo - 40])
+            cosmo_dict = dict(Table.read(path / 'aa_test_cosmos.txt',
+                                         format='ascii')[i_cosmo - 40])
         else:
             raise ValueError('Unknown cosmology number {}. '.format(i_cosmo) +
                              'Must be in the range from 0 to 46.')
         cosmo_dict['Ob0'] = cosmo_dict['ombh2'] / (cosmo_dict['H0'] / 100)**2
         cosmo_dict['Oc0'] = cosmo_dict['omch2'] / (cosmo_dict['H0'] / 100)**2
         cosmo_dict['Om0'] = cosmo_dict['Ob0'] + cosmo_dict['Oc0']
         return FlatwCDM(H0=cosmo_dict['H0'], Om0=cosmo_dict['Om0'],
@@ -162,15 +142,15 @@
     suite : str
         The simulation suite.
     i_cosmo : int, optional
         If applicable, number corresponding to the cosmology. Default is 0.
     i_phase : int, optional
         If applicable, number corresponding to the simulation phase. Default
         is 0.
-    config : str
+    config : str, optional
         Simulation configuration. Only applicable to AbacusSummit. If None,
         will default to 'base' for AbacusSummit. Default is None.
 
     Returns
     -------
     name : str
         The TabCorr database directory.
@@ -202,83 +182,85 @@
             raise ValueError('Unknown cosmology number {}. '.format(i_cosmo) +
                              'Must be in the range from 0 to 46.')
 
     else:
         raise ValueError('Unkown simulation suite {}.'.format(suite))
 
 
-def simulation_snapshot_directory(
-        suite, redshift, i_cosmo=0, i_phase=0, config=None):
+def directory(suite, redshift, i_cosmo=0, i_phase=0, config=None):
     """Return the directory where all data for a simulation snapshot is stored.
 
     Parameters
     ----------
     suite : str
         The simulation suite.
     redshift : float
         The redshift of the simulation output.
     i_cosmo : int, optional
         If applicable, number corresponding to the cosmology. Default is 0.
     i_phase : int, optional
         If applicable, number corresponding to the simulation phase. Default
         is 0.
-    config : str
+    config : str, optional
         Simulation configuration. Only applicable to AbacusSummit. If None,
         will default to 'base' for AbacusSummit. Default is None.
 
     Returns
     -------
-    name : str
+    path : pathlib.Path
         The directory where all data for a simulation snapshot is stored.
 
+    Raises
+    ------
+    RuntimeError
+        If the TABCORR_DATABASE environment variable is not set.
+
     """
+    try:
+        path = Path(os.environ['TABCORR_DATABASE'])
+    except KeyError:
+        raise RuntimeError(
+            "You must set the TABCORR_DATABASE environment variable.")
     name = simulation_name(suite, i_cosmo=i_cosmo, i_phase=i_phase,
                            config=config)
-    return os.path.join(
-        directory(), suite, name,
-        '{:.2f}'.format(redshift).replace('.', 'p'))
+    return (path / suite / name / '{:.2f}'.format(redshift).replace(
+        '.', 'p'))
 
 
-def tabcorr(suite, redshift, tpcf, i_cosmo=0, i_phase=0, sim_config=None,
-            tab_config='default'):
-    """Return the TabCorr tabulation for a given simulation, redshift etc.
+def read(suite, redshift, tpcf, i_cosmo=0, i_phase=0, sim_config=None,
+         tab_config='default'):
+    """Read the TabCorr tabulation for a given simulation, redshift etc.
 
     Parameters
     ----------
     suite : str
         The simulation suite.
     redshift : float
         The redshift of the simulation output.
     tpcf : str
         String describing the two-point correlation function.
     i_cosmo : int, optional
         If applicable, number corresponding to the cosmology. Default is 0.
     i_phase : int, optional
         If applicable, number corresponding to the simulation phase. Default
         is 0.
-    sim_config : str
+    sim_config : str, optional
         Simulation configuration. Only applicable to AbacusSummit. If None,
         will default to 'base' for AbacusSummit. Default is None.
-    tab_config : config_str : str
+    tab_config : config_str : str, optional
         String describing the configuration of the tabulation, i.e. binning,
         cosmology etc.
 
     Returns
     -------
     halotab : tabcorr.TabCorr or tabcorr.Interpolator
         The tabcorr tabulation.
 
     """
-    directory = os.path.join(simulation_snapshot_directory(
-        suite, redshift, i_cosmo=i_cosmo, i_phase=i_phase, config=sim_config),
-        tab_config)
-
-    param_dict_table = Table.read(os.path.join(
-        directory, tpcf[:2] + '_grid.csv'))
-    param_dict_table['log_eta'] = np.log10(param_dict_table['conc_gal_bias'])
-    param_dict_table.remove_column('conc_gal_bias')
-    for key in ['alpha_c', 'alpha_s', 'log_eta']:
-        if len(np.unique(param_dict_table[key])) == 1:
-            param_dict_table.remove_column(key)
-    tabcorr_list = [TabCorr.read(os.path.join(directory, '{}_{}.hdf5'.format(
-        tpcf, i))) for i in range(len(param_dict_table))]
-    return Interpolator(tabcorr_list, param_dict_table)
+    path = directory(
+        suite, redshift, i_cosmo=i_cosmo, i_phase=i_phase, config=sim_config)
+
+    return Interpolator.read(path / '{}_{}.hdf5'.format(tpcf, tab_config))
+
+
+# Define an alias for backwards compatibility.
+tabcorr = read
```

### Comparing `tabcorr-1.0.1/tabcorr/interpolate.py` & `tabcorr-1.1.0/tabcorr/interpolator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-"""Module for interpolation between TabCorr instances."""
+"""Module for interpolation of TabCorr instances."""
 
+import h5py
 import numpy as np
+
+from astropy.table import Table
 from scipy.spatial import Delaunay
 
+from . import TabCorr
+
 
 class Interpolator:
     """Class for interpolation of multiple TabCorr instances."""
 
     def __init__(self, tabcorr_list, param_dict_table, spline=True):
         """Initialize an interpolation of multiple TabCorr instances.
 
@@ -19,36 +24,37 @@
             instance in the TabCorr list. Must have the same length and
             ordering as `tabcorr_list`.
         spline : bool, optional
             For multi-dimensional interpolation, whether the interpolation
             is performed over a regular grid using spline interpolation or
             over an irregular grid using linear barycentric interpolation.
             Spline interpolation is more accurate but slower and the TabCorr
-            instances need to be arranged on a grid. Default is True.
+            instances need to be arranged on a grid. For one-dimensional
+            interpolation, spline interpolation will always be used. Default is
+            True.
 
         Raises
         ------
         ValueError
             If `spline` is True and `param_dict_table` does not describe a
             grid.
 
         """
         if len(tabcorr_list) != len(param_dict_table):
             raise ValueError("The number of TabCorr instances does not match" +
                              " the number of entries in 'param_dict_table'.")
 
         self.tabcorr_list = tabcorr_list
-        self.keys = param_dict_table.colnames
         self.param_dict_table = param_dict_table.copy()
-        self.spline = spline or len(self.keys) == 1
+        self.spline = spline or len(self.param_dict_table.colnames) == 1
 
         if self.spline:
             self.xp = []
             self.a = []
-            for key in self.keys:
+            for key in self.param_dict_table.colnames:
                 self.xp.append(np.sort(np.unique(param_dict_table[key])))
                 self.a.append(spline_interpolation_matrix(self.xp[-1]))
 
             try:
                 # Check that the table has the right length to describe the
                 # grid.
                 assert (np.prod([len(xp) for xp in self.xp]) ==
@@ -60,37 +66,93 @@
                               return_counts=True)[1] == 1)
             except AssertionError:
                 raise ValueError(
                     "The 'param_dict_table' does not describe a grid.")
 
             self.param_dict_table['tabcorr_index'] = np.arange(len(
                 self.param_dict_table))
-            self.param_dict_table.sort(self.keys)
+            self.param_dict_table.sort(self.param_dict_table.colnames)
 
         else:
 
-            if len(self.param_dict_table) <= len(self.keys):
+            if len(self.param_dict_table) <= len(
+                    self.param_dict_table.colnames):
                 raise ValueError(
                     'The number of TabCorr instances provided must be ' +
                     'larger than the number of dimensions.')
 
-            self.xp = np.zeros((len(self.param_dict_table), len(self.keys)))
-            for i, key in enumerate(self.keys):
+            self.xp = np.zeros((len(self.param_dict_table),
+                               len(self.param_dict_table.colnames)))
+            for i, key in enumerate(self.param_dict_table.colnames):
                 self.xp[:, i] = self.param_dict_table[key].data
             self.delaunay = Delaunay(self.xp)
 
         # Determine unique halo tables such that we can save computation time
         # if halo tables are repeated.
         all_gal_type = [np.array(tabcorr.gal_type.as_array().tolist()).ravel()
                         for tabcorr in tabcorr_list]
         unique = np.unique(
             all_gal_type, axis=0, return_index=True, return_inverse=True)
         self.unique_gal_type_index = unique[1]
         self.unique_gal_type_inverse = unique[2]
 
+    @classmethod
+    def read(cls, fname):
+        """Read a TabCorr interpolator from the disk.
+
+        Parameters
+        ----------
+        fname : string
+            Name of the file containing the interpolator object.
+
+        Returns
+        -------
+            `Interpolator` object.
+
+        """
+        tabcorr_list = []
+
+        with h5py.File(fname, 'r') as fstream:
+            param_dict_table = Table.read(fstream['param_dict_table'])
+            param_dict_table.sort('tabcorr_index')
+            param_dict_table.remove_column('tabcorr_index')
+            for i in range(len(param_dict_table)):
+                tabcorr_list.append(
+                    TabCorr.read(fstream['tabcorr_{}'.format(i)]))
+            spline = fstream.attrs['spline']
+
+        return Interpolator(tabcorr_list, param_dict_table, spline=spline)
+
+    def write(self, fname, overwrite=False, max_args_size=1000000,
+              matrix_dtype=np.float32):
+        """Write the TabCorr interpolator to the disk.
+
+        Parameters
+        ----------
+        fname : string or h5py.Group
+            Name of the file the data is written to.
+        overwrite : bool, optional
+            If True, any existing file will be overwritten. Default is False.
+        max_args_size : int, optional
+            By default, TabCorr writes all arguments passed to the correlation
+            function when calling `tabulate` to file. However, arguments that
+            are numpy arrays with more entries than max_args_size will be
+            omitted. Default is 1000000.
+        matrix_dtype : type
+            The dtype used to write the correlation matrix to disk. Can be used
+            to save space at the expense of precision.
+
+        """
+        with h5py.File(fname, 'w' if overwrite else 'w-') as fstream:
+            self.param_dict_table.write(fstream, path='param_dict_table')
+            for i in range(len(self.param_dict_table)):
+                self.tabcorr_list[i].write(
+                    fstream.create_group('tabcorr_{}'.format(i)))
+            fstream.attrs['spline'] = self.spline
+
     def predict(self, model, n_gauss_prim=10, extrapolate=False, **occ_kwargs):
         """Interpolate the predictions from multiple TabCorr instances.
 
         The values of parameters to interpolate should be in the parameter
         dictionary of the model.
 
         Parameters
@@ -119,16 +181,18 @@
         Raises
         ------
         ValueError
             If `extrapolate` is set to True and values are outside the
             interpolation range.
 
         """
-        x_model = np.empty(len(self.keys))
-        for i, key in enumerate(self.keys):
+        x_model = np.empty(len(self.param_dict_table.colnames))
+        for i, key in enumerate(self.param_dict_table.colnames):
+            if key == 'tabcorr_index':
+                continue
             try:
                 x_model[i] = model.param_dict[key]
             except KeyError:
                 raise ValueError(
                     'The key {} is not present in the parameter '.format(key) +
                     'dictionary of the model.')
```

### Comparing `tabcorr-1.0.1/tabcorr/tabcorr.py` & `tabcorr-1.1.0/tabcorr/tabcorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 from halotools.utils import crossmatch
 from halotools.utils.table_utils import compute_conditional_percentiles
 
 
 class TabCorr:
     """Class to tabulate halo and predict galaxy correlation functions."""
 
-    def __init__(self):
-        self.init = False
-
     @classmethod
     def tabulate(cls, halocat, tpcf, *tpcf_args,
                  mode='auto',
                  Num_ptcl_requirement=sim_defaults.Num_ptcl_requirement,
                  prim_haloprop_key=model_defaults.prim_haloprop_key,
                  prim_haloprop_bins=30,
                  sec_haloprop_key=model_defaults.sec_haloprop_key,
@@ -377,25 +374,29 @@
 
     @classmethod
     def read(cls, fname):
         """Read tabulated correlation functions from the disk.
 
         Parameters
         ----------
-        fname : string
-            Name of the file containing the TabCorr object.
+        fname : string or h5py.Group
+            Name of the file or h5py group containing the TabCorr object.
 
         Returns
         -------
             `TabCorr` object.
 
         """
         halotab = cls()
 
-        fstream = h5py.File(fname, 'r')
+        if not isinstance(fname, h5py.Group):
+            fstream = h5py.File(fname, 'r')
+        else:
+            fstream = fname
+
         halotab.attrs = {}
         for key in fstream.attrs.keys():
             halotab.attrs[key] = fstream.attrs[key]
 
         halotab.tpcf_matrix = fstream['tpcf_matrix'][()].astype(np.float64)
 
         halotab.tpcf_args = []
@@ -403,43 +404,46 @@
             halotab.tpcf_args.append(fstream['tpcf_args'][key][()])
         halotab.tpcf_args = tuple(halotab.tpcf_args)
         halotab.tpcf_kwargs = {}
         if 'tpcf_kwargs' in fstream:
             for key in fstream['tpcf_kwargs'].keys():
                 halotab.tpcf_kwargs[key] = fstream['tpcf_kwargs'][key][()]
         halotab.tpcf_shape = tuple(fstream['tpcf_shape'][()])
-        fstream.close()
 
-        halotab.gal_type = Table.read(fname, path='gal_type')
+        if not isinstance(fname, h5py.Group):
+            fstream.close()
 
-        halotab.init = True
+        halotab.gal_type = Table.read(fname, path='gal_type')
 
         return halotab
 
     def write(self, fname, overwrite=False, max_args_size=1000000,
               matrix_dtype=np.float32):
         """Write the tabulated correlation functions to the disk.
 
         Parameters
         ----------
-        fname : string
-            Name of the file that is written.
+        fname : string or h5py.Group
+            Name of the file or h5py group the data is written to.
         overwrite : bool, optional
             If True, any existing file will be overwritten. Default is False.
         max_args_size : int, optional
             By default, TabCorr writes all arguments passed to the correlation
             function when calling `tabulate` to file. However, arguments that
             are numpy arrays with more entries than max_args_size will be
             omitted. Default is 1000000.
         matrix_dtype : type
             The dtype used to write the correlation matrix to disk. Can be used
             to save space at the expense of precision.
 
         """
-        fstream = h5py.File(fname, 'w' if overwrite else 'w-')
+        if not isinstance(fname, h5py.Group):
+            fstream = h5py.File(fname, 'w' if overwrite else 'w-')
+        else:
+            fstream = fname
 
         keys = ['tpcf', 'mode', 'simname', 'redshift', 'Num_ptcl_requirement',
                 'prim_haloprop_key', 'sec_haloprop_key']
         for key in keys:
             fstream.attrs[key] = self.attrs[key]
 
         fstream['tpcf_matrix'] = self.tpcf_matrix.astype(matrix_dtype)
@@ -449,15 +453,17 @@
                     np.prod(arg.shape) < max_args_size):
                 fstream['tpcf_args/arg_%d' % i] = arg
         for key in self.tpcf_kwargs:
             if (type(self.tpcf_kwargs[key]) is not np.ndarray or
                     np.prod(self.tpcf_kwargs[key].shape) < max_args_size):
                 fstream['tpcf_kwargs/' + key] = self.tpcf_kwargs[key]
         fstream['tpcf_shape'] = self.tpcf_shape
-        fstream.close()
+
+        if not isinstance(fname, h5py.Group):
+            fstream.close()
 
         self.gal_type.write(fname, path='gal_type', append=True)
 
     def mean_occupation(self, model, n_gauss_prim=10, **occ_kwargs):
         """Calculate the mean occupation for each halo/galaxy bin.
 
         Parameters
@@ -645,15 +651,15 @@
         if self.attrs['mode'] == 'auto':
             for gal_type_1, gal_type_2 in (
                     itertools.combinations_with_replacement(
                         np.unique(self.gal_type['gal_type']), 2)):
                 mask = symmetric_matrix_to_array(np.outer(
                     gal_type_1 == self.gal_type['gal_type'],
                     gal_type_2 == self.gal_type['gal_type']) |
-                        np.outer(
+                    np.outer(
                     gal_type_2 == self.gal_type['gal_type'],
                     gal_type_1 == self.gal_type['gal_type']))
                 xi_dict['%s-%s' % (gal_type_1, gal_type_2)] = np.sum(
                     xi * mask, axis=1).reshape(self.tpcf_shape)
 
         elif self.attrs['mode'] == 'cross':
             for gal_type in np.unique(self.gal_type['gal_type']):
@@ -681,15 +687,14 @@
         Secondary halo property percentile bins.
     x : numpy.ndarray
         Array to sort into bins.
     gal_type : None or numpy.ndarray, optional
         Galaxy types. If None, results are not sorted by galaxy type. Default
         is None.
 
-
     Returns
     -------
     x_sorted : list
         Values of `x` sorted into bins.
 
     """
     n_p = len(log_prim_haloprop_bins) - 1
```

### Comparing `tabcorr-1.0.1/PKG-INFO` & `tabcorr-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tabcorr
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tabulated Correlation Functions
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: h5py
 Requires-Dist: tqdm
-Project-URL: Home, https://johannesulf.github.io/
+Project-URL: Home, https://tabcorr.readthedocs.io
 
 # TabCorr: Tabulated Correlation Functions
 
 [![PyPI Version](https://img.shields.io/pypi/v/tabcorr?color=blue)](https://pypi.org/project/tabcorr/)
 [![License: MIT](https://img.shields.io/github/license/johannesulf/TabCorr?color=blue)](https://raw.githubusercontent.com/johannesulf/TabCorr/main/LICENSE)
 ![Language: Python](https://img.shields.io/github/languages/top/johannesulf/TabCorr)
```

