# Comparing `tmp/hexfft-0.1.0.tar.gz` & `tmp/hexfft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexfft-0.1.0.tar", last modified: Thu Apr 25 02:39:20 2024, max compression
+gzip compressed data, was "hexfft-0.1.1.tar", last modified: Fri May  3 02:59:59 2024, max compression
```

## Comparing `hexfft-0.1.0.tar` & `hexfft-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.862626 hexfft-0.1.0/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.852340 hexfft-0.1.0/.github/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.854107 hexfft-0.1.0/.github/workflows/
--rw-r--r--   0 chris      (501) staff       (20)     1094 2024-04-24 02:26:15.000000 hexfft-0.1.0/.github/workflows/python-package-conda.yml
--rw-r--r--   0 chris      (501) staff       (20)     1078 2024-04-06 16:16:22.000000 hexfft-0.1.0/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)      844 2024-04-25 02:39:20.862399 hexfft-0.1.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      582 2024-04-06 16:16:22.000000 hexfft-0.1.0/README.md
--rw-r--r--   0 chris      (501) staff       (20)       55 2024-04-25 02:06:04.000000 hexfft-0.1.0/environment.yml
--rw-r--r--   0 chris      (501) staff       (20)      359 2024-04-25 02:32:26.000000 hexfft-0.1.0/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)       22 2024-04-25 02:06:20.000000 hexfft-0.1.0/requirements.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2024-04-25 02:39:20.862665 hexfft-0.1.0/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.852598 hexfft-0.1.0/src/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.856824 hexfft-0.1.0/src/hexfft/
--rw-r--r--   0 chris      (501) staff       (20)       84 2024-04-25 00:42:25.000000 hexfft-0.1.0/src/hexfft/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     4435 2024-04-25 02:20:21.000000 hexfft-0.1.0/src/hexfft/array.py
--rw-r--r--   0 chris      (501) staff       (20)     2245 2024-04-23 19:01:41.000000 hexfft-0.1.0/src/hexfft/grids.py
--rw-r--r--   0 chris      (501) staff       (20)    20622 2024-04-25 02:22:50.000000 hexfft-0.1.0/src/hexfft/hexfft.py
--rw-r--r--   0 chris      (501) staff       (20)     3722 2024-04-24 13:10:19.000000 hexfft-0.1.0/src/hexfft/plot.py
--rw-r--r--   0 chris      (501) staff       (20)     2896 2024-04-25 02:03:45.000000 hexfft-0.1.0/src/hexfft/reference.py
--rw-r--r--   0 chris      (501) staff       (20)     3841 2024-04-25 02:21:17.000000 hexfft-0.1.0/src/hexfft/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.862144 hexfft-0.1.0/src/hexfft.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      844 2024-04-25 02:39:20.000000 hexfft-0.1.0/src/hexfft.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      450 2024-04-25 02:39:20.000000 hexfft-0.1.0/src/hexfft.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-04-25 02:39:20.000000 hexfft-0.1.0/src/hexfft.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        7 2024-04-25 02:39:20.000000 hexfft-0.1.0/src/hexfft.egg-info/top_level.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-25 02:39:20.861684 hexfft-0.1.0/tests/
--rw-r--r--   0 chris      (501) staff       (20)     3995 2024-04-25 02:23:31.000000 hexfft-0.1.0/tests/test_api.py
--rw-r--r--   0 chris      (501) staff       (20)     8158 2024-04-25 02:24:33.000000 hexfft-0.1.0/tests/test_hexfft.py
--rw-r--r--   0 chris      (501) staff       (20)     3180 2024-04-25 02:31:28.000000 hexfft-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.797245 hexfft-0.1.1/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.790383 hexfft-0.1.1/.github/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.792371 hexfft-0.1.1/.github/workflows/
+-rw-r--r--   0 chris      (501) staff       (20)     1094 2024-04-24 02:26:15.000000 hexfft-0.1.1/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 chris      (501) staff       (20)     1078 2024-04-06 16:16:22.000000 hexfft-0.1.1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     1102 2024-05-03 02:59:59.796955 hexfft-0.1.1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      840 2024-04-25 02:53:04.000000 hexfft-0.1.1/README.md
+-rw-r--r--   0 chris      (501) staff       (20)       55 2024-04-25 02:06:04.000000 hexfft-0.1.1/environment.yml
+-rw-r--r--   0 chris      (501) staff       (20)      359 2024-05-03 02:58:27.000000 hexfft-0.1.1/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       22 2024-04-25 02:06:20.000000 hexfft-0.1.1/requirements.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2024-05-03 02:59:59.797287 hexfft-0.1.1/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.790620 hexfft-0.1.1/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.794534 hexfft-0.1.1/src/hexfft/
+-rw-r--r--   0 chris      (501) staff       (20)       84 2024-04-25 00:42:25.000000 hexfft-0.1.1/src/hexfft/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4435 2024-05-03 01:21:02.000000 hexfft-0.1.1/src/hexfft/array.py
+-rw-r--r--   0 chris      (501) staff       (20)     2245 2024-04-23 19:01:41.000000 hexfft-0.1.1/src/hexfft/grids.py
+-rw-r--r--   0 chris      (501) staff       (20)    21147 2024-05-03 02:57:35.000000 hexfft-0.1.1/src/hexfft/hexfft.py
+-rw-r--r--   0 chris      (501) staff       (20)     3722 2024-04-26 04:17:34.000000 hexfft-0.1.1/src/hexfft/plot.py
+-rw-r--r--   0 chris      (501) staff       (20)     2896 2024-04-30 13:13:15.000000 hexfft-0.1.1/src/hexfft/reference.py
+-rw-r--r--   0 chris      (501) staff       (20)     3841 2024-04-25 02:21:17.000000 hexfft-0.1.1/src/hexfft/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.796617 hexfft-0.1.1/src/hexfft.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     1102 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      450 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        7 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.796158 hexfft-0.1.1/tests/
+-rw-r--r--   0 chris      (501) staff       (20)     4025 2024-05-03 02:57:35.000000 hexfft-0.1.1/tests/test_api.py
+-rw-r--r--   0 chris      (501) staff       (20)     9604 2024-05-03 02:57:35.000000 hexfft-0.1.1/tests/test_hexfft.py
+-rw-r--r--   0 chris      (501) staff       (20)     3180 2024-04-25 02:31:28.000000 hexfft-0.1.1/tests/test_utils.py
```

### Comparing `hexfft-0.1.0/.github/workflows/python-package-conda.yml` & `hexfft-0.1.1/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/LICENSE` & `hexfft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/PKG-INFO` & `hexfft-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: hexfft
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hexagonal FFTs in Python
 Author-email: Chris Langfield <christopher.langfield@gmail.com>
 Keywords: hexagonal,dsp,fft
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A Python package aiming to provide an easy and efficient interface to various implementations of the [Hexagonal Fast Fourier Transform](https://en.wikipedia.org/wiki/Hexagonal_fast_Fourier_transform). The purpose of the software is primarily educational with a goal of eventually reaching production quality.
 
-For now the `fft()` and `ifft()` methods implement the HFFT algorithm due to Mersereau in
+For now the `fft()` and `ifft()` methods implement HFFT described in the following papers:
 
 > R. M. Mersereau, "The processing of hexagonally sampled two-dimensional signals," in Proceedings of the IEEE, vol. 67, no. 6, pp. 930-949, June 1979, doi: 10.1109/PROC.1979.11356
+
+> Ehrhardt, J. C. (1993). Hexagonal fast Fourier transform with rectangular output. In IEEE Transactions on Signal Processing (Vol. 41, Issue 3, pp. 1469–1472). Institute of Electrical and Electronics Engineers (IEEE). https://doi.org/10.1109/78.205759
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hexfft-0.1.0/src/hexfft/array.py` & `hexfft-0.1.1/src/hexfft/array.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/src/hexfft/grids.py` & `hexfft-0.1.1/src/hexfft/grids.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/src/hexfft/hexfft.py` & `hexfft-0.1.1/src/hexfft/hexfft.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         return HexPeriodicFFT(shape, dtype)
     elif periodicity == "rect":
         return RectPeriodicFFT(shape, dtype)
 
 
 class HexagonalFFT:
     def __init__(self, shape, dtype):
-
         assert len(shape) == 2, "Only 2D transforms are supported."
         assert dtype in [
             np.complex128,
             np.complex64,
         ], "dtype of transform must be complex"
 
         self.shape = shape
@@ -44,17 +43,15 @@
         return self._forward(x)
 
     def inverse(self, X):
         return self._inverse(X)
 
 
 class HexPeriodicFFT(HexagonalFFT):
-
     def __init__(self, shape, dtype):
-
         assert (
             shape[0] == shape[1]
         ), "Input to FFT with hex periodicity must be a square array"
         assert (
             shape[0] % 4 == 0
         ), "Array size for periodicity='hex' must be a multiple of 4."
 
@@ -83,15 +80,14 @@
         self.W2 = np.exp(-1.0j * 2 * np.pi * (k2 + k1) / (3 * M)).astype(self.cdtype)
 
         self.conj_W0 = np.conj(self.W0)
         self.conj_W1 = np.conj(self.W1)
         self.conj_W2 = np.conj(self.W2)
 
     def _forward(self, x):
-
         assert (
             x.shape[-2:] == self.shape
         ), f"Input array with shape {x.shape} does not match FFT object shape {self.shape}"
 
         N = self.shape[0]
 
         squeeze = x.ndim == 2
@@ -239,80 +235,98 @@
         N1, N2 = self.shape
         self.phase_shift = np.exp(
             1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N1
         )
         self.phase_shift_conj = np.conj(self.phase_shift)
 
     def _forward(self, x):
-        assert x.shape[-2:] == self.shape
-
-        if isinstance(x, HexArray) and x.pattern == "oblique":
-            raise ValueError(
-                "Input array to FFT with rectangular periodicity must be in 'offset' coordinates."
-            )
-        else:
-            x = HexArray(x, "offset")
-
-        x = rect_shift(x)
+        assert (
+            x.shape[-2:] == self.shape
+        ), f"Input array with shape {x.shape} does not match FFT object shape {self.shape}"
+        assert isinstance(
+            x, HexArray
+        ), "Input to rectangular periodic FFT must be HexArray."
+
+        shift = x.pattern == "offset"
+        if shift:
+            x = rect_shift(x)
 
         squeeze = x.ndim == 2
         if squeeze:
             x = np.expand_dims(x, 0)
 
         F1 = scipy.fft.fft(x, axis=1)
         F2 = F1 * self.phase_shift
         X = scipy.fft.fft(F2, axis=2)
 
         if squeeze:
             X = np.squeeze(X)
 
-        return rect_unshift(HexArray(X, "oblique"))
+        if shift:
+            X = rect_unshift(HexArray(X, "oblique"))
+        else:
+            X = HexArray(X, "oblique")
+
+        return X
 
     def _inverse(self, X):
-        if isinstance(X, HexArray) and X.pattern == "oblique":
-            _logger.warn(
-                "Passing HexArray with 'oblique' sampling pattern to "
-                "a rectangular periodic FFT."
-            )
+        assert (
+            X.shape[-2:] == self.shape
+        ), f"Input array with shape {X.shape} does not match FFT object shape {self.shape}"
+        assert isinstance(
+            X, HexArray
+        ), "Input to rectangular periodic FFT must be HexArray."
+
+        shift = X.pattern == "offset"
+        if shift:
+            X = rect_shift(X)
 
-        X = rect_shift(X)
         squeeze = X.ndim == 2
         if squeeze:
             X = np.expand_dims(X, 0)
+
         F2 = scipy.fft.ifft(X, axis=2)
         F1 = F2 * self.phase_shift_conj
         x = HexArray(scipy.fft.ifft(F1, axis=1), "oblique")
 
         if squeeze:
             x = np.squeeze(x)
 
-        return rect_unshift(x)
+        if shift:
+            x = rect_unshift(HexArray(x, "oblique"))
+        else:
+            x = HexArray(x, "oblique")
 
+        return x
 
-def fft(x, periodicity="rect"):
 
+def fft(x, periodicity="rect"):
     if periodicity == "hex":
         assert x.shape[0] == x.shape[1], "Input to fft(-, 'hex') must be a square array"
         N = x.shape[0]
         assert N % 4 == 0, "Array size for periodicity='hex' must be a multiple of 4."
 
         px = hex_to_pgram(x)
         PX = mersereau_fft(px)
         return pgram_to_hex(PX, N, pattern=x.pattern)
 
     elif periodicity == "rect":
-        if isinstance(x, HexArray) and x.pattern == "oblique":
-            raise ValueError(
-                "Input array to FFT with rectangular periodicity must be in 'offset' coordinates."
-            )
-        else:
-            x = HexArray(x, "offset")
+        assert isinstance(
+            x, HexArray
+        ), "Input to rectangular periodic FFT must be HexArray."
+
+        shift = x.pattern == "offset"
+        if shift:
+            x = rect_shift(x)
+
+        X = rect_fft(x)
+        if shift:
+            X = rect_unshift(X)
 
-        X = rect_fft(rect_shift(x))
-        return rect_unshift(X)
+        return X
 
     raise ValueError(f"Unrecognized periodicity option: {periodicity}")
 
 
 def ifft(X, periodicity="rect"):
     if periodicity == "hex":
         assert (
@@ -322,16 +336,27 @@
         assert N % 4 == 0, "Array size for periodicity='hex' must be a multiple of 4."
 
         PX = hex_to_pgram(X)
         px = mersereau_ifft(PX)
         return pgram_to_hex(px, N, pattern=X.pattern)
 
     elif periodicity == "rect":
-        x = rect_ifft(rect_shift(X))
-        return rect_unshift(x)
+        assert isinstance(
+            X, HexArray
+        ), "Input to rectangular periodic IFFT must be HexArray."
+        shift = X.pattern == "offset"
+        if shift:
+            X = rect_shift(X)
+
+        x = rect_ifft(X)
+
+        if shift:
+            x = rect_unshift(x)
+
+        return x
 
     raise ValueError(f"Unrecognized periodicity option: {periodicity}")
 
 
 def mersereau_fft(px):
     """"""
     assert 3 * px.shape[0] == px.shape[1], "must have dimensions Nx3N"
```

### Comparing `hexfft-0.1.0/src/hexfft/plot.py` & `hexfft-0.1.1/src/hexfft/plot.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/src/hexfft/reference.py` & `hexfft-0.1.1/src/hexfft/reference.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/src/hexfft/utils.py` & `hexfft-0.1.1/src/hexfft/utils.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.0/src/hexfft.egg-info/PKG-INFO` & `hexfft-0.1.1/src/hexfft.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: hexfft
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hexagonal FFTs in Python
 Author-email: Chris Langfield <christopher.langfield@gmail.com>
 Keywords: hexagonal,dsp,fft
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A Python package aiming to provide an easy and efficient interface to various implementations of the [Hexagonal Fast Fourier Transform](https://en.wikipedia.org/wiki/Hexagonal_fast_Fourier_transform). The purpose of the software is primarily educational with a goal of eventually reaching production quality.
 
-For now the `fft()` and `ifft()` methods implement the HFFT algorithm due to Mersereau in
+For now the `fft()` and `ifft()` methods implement HFFT described in the following papers:
 
 > R. M. Mersereau, "The processing of hexagonally sampled two-dimensional signals," in Proceedings of the IEEE, vol. 67, no. 6, pp. 930-949, June 1979, doi: 10.1109/PROC.1979.11356
+
+> Ehrhardt, J. C. (1993). Hexagonal fast Fourier transform with rectangular output. In IEEE Transactions on Signal Processing (Vol. 41, Issue 3, pp. 1469–1472). Institute of Electrical and Electronics Engineers (IEEE). https://doi.org/10.1109/78.205759
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hexfft-0.1.0/tests/test_api.py` & `hexfft-0.1.1/tests/test_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,53 +32,50 @@
         h = HexArray(array, p)
 
     with pytest.raises(ValueError, match="not implemented or unknown"):
         _ = HexArray(array, "bla")
 
 
 def test_rect_shift_pathological_inputs():
-
     with pytest.raises(AssertionError, match="must be in 'offset'"):
         _ = rect_shift(h_obl)
 
     with pytest.raises(AssertionError, match="must be in 'oblique'"):
         _ = rect_unshift(h_off)
 
     with pytest.raises(ValueError, match="less than 2x2"):
         _ = rect_shift(h_off[:2, :1])
 
     with pytest.raises(ValueError, match="less than 2x2"):
         _ = rect_unshift(h_obl[:2, :1])
 
 
 def test_fft_call():
-
     with pytest.raises(ValueError, match="Unrecognized periodicity"):
         _ = fft(array, "bla")
 
     with pytest.raises(ValueError, match="Unrecognized periodicity"):
         _ = ifft(array, "bla")
 
     # forbidden Arrays for hexagonal periodicity
-    with pytest.raises(AssertionError, match="square"):
+    with pytest.raises(AssertionError, match="square"):  # hex fft input must be square
         _ = fft(array[:4, :], "hex")
 
-    with pytest.raises(AssertionError, match="multiple of 4."):
+    with pytest.raises(
+        AssertionError, match="multiple of 4."
+    ):  # hex fft input must be multiple of 4
         _ = fft(array[:10, :10], "hex")
 
-    with pytest.raises(AssertionError, match="square"):
+    with pytest.raises(AssertionError, match="square"):  # hex ifft input must be square
         _ = ifft(array[:4, :], "hex")
 
-    with pytest.raises(AssertionError, match="multiple of 4."):
-        _ = ifft(array[:10, :10], "hex")
-
     with pytest.raises(
-        ValueError, match="Input array to FFT with rectangular periodicity"
-    ):
-        _ = fft(h_obl, "rect")
+        AssertionError, match="multiple of 4."
+    ):  # hex ifft input must be multiple of 4
+        _ = ifft(array[:10, :10], "hex")
 
 
 @pytest.mark.parametrize("per", periodicities)
 def test_FFT_constr(per):
     with pytest.raises(AssertionError, match="dtype of transform"):
         _ = FFT((8, 8), per, np.float32)
     with pytest.raises(AssertionError, match="Only 2D transforms"):
@@ -96,15 +93,14 @@
         match="Array size for periodicity='hex' must be a multiple of 4.",
     ):
         _ = FFT((10, 10), "hex")
 
 
 @pytest.mark.parametrize("pattern", patterns)
 def test_hex_fft_output(pattern):
-
     X = fft(HexArray(array, pattern), "hex")
     assert X.shape == array.shape
     assert X.dtype == np.complex128
 
     X = fft(HexArray(array.astype(np.float32), pattern), "hex")
     assert X.dtype == np.complex64
```

### Comparing `hexfft-0.1.0/tests/test_hexfft.py` & `hexfft-0.1.1/tests/test_hexfft.py`

 * *Files 11% similar despite different names*

```diff
@@ -125,29 +125,40 @@
         D = _rect_dft_slow(d)
         dd = _rect_idft_slow(D)
 
         assert np.allclose(d, dd, atol=1e-12)
 
 
 def test_rect_fft():
-    for shape in [(4, 5), (8, 8), (11, 16), (19, 19)]:
-        N1, N2 = shape
-        n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
-        center = (N1 // 2 - 1, N2 // 2 - 1)
-        d = rect_shift(hregion(n1, n2, center, 1, "offset"))
+    for pattern in ["oblique", "offset"]:
+        for shape in [(4, 5), (8, 8), (11, 16), (19, 19)]:
+            N1, N2 = shape
+            n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
+            center = (N1 // 2 - 1, N2 // 2 - 1)
+            d = rect_shift(hregion(n1, n2, center, 1, "offset"))
+
+            D = rect_fft(d)
+            D_slow = _rect_dft_slow(d)
+
+            assert np.allclose(D, D_slow)
+
+            dd = rect_ifft(D)
+            dd_slow = _rect_idft_slow(D_slow)
 
-        D = rect_fft(d)
-        D_slow = _rect_dft_slow(d)
+            assert np.allclose(dd, dd_slow)
 
-        assert np.allclose(D, D_slow)
 
-        dd = rect_ifft(rect_unshift(D))
-        dd_slow = _rect_idft_slow(rect_unshift(D_slow))
+# def test_validate_rect_fft():
+#     for shape in [ (8, 8), (11, 16), (19, 19)]:
+#         N1, N2 = shape
+#         n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2), indexing="ij")
+#         mode1 = HexArray(np.exp(-2 * np.pi * 1.0j * n1/N1), "oblique")
 
-        assert np.allclose(dd, dd_slow)
+#         M1 = fft(rect_unshift(mode1))
+#         assert np.real(M1[0, 1]) == 1.
 
 
 def test_rect_fft_stack():
     # create a stack of data
     nstack, N1, N2 = 5, 8, 12
     n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
     center = (N1 / 2 - 1, N2 / 2 - 1)
@@ -180,14 +191,47 @@
     assert np.allclose(DS_STACK, DS_SINGLE)
 
     dds_stack = fftobj.inverse(DS_STACK)
     dds_single = rect_unshift(rect_ifft(rect_shift(DS_SINGLE)))
     assert np.allclose(dds_stack, dds_single)
 
 
+def test_rect_fft_stack_noshift():
+    # create a stack of data
+    nstack, N1, N2 = 5, 8, 12
+    n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
+    center = (N1 / 2 - 1, N2 / 2 - 1)
+    data = np.stack([hregion(n1, n2, center, i).T for i in range(1, nstack + 1)])
+    data = HexArray(data, "oblique")
+
+    fftobj = FFT((N1, N2), periodicity="rect")
+    DATA_STACK = fftobj.forward(data)
+
+    DATA_LOOP = np.stack([rect_fft(data[i]) for i in range(nstack)])
+    DATA_LOOP = HexArray(DATA_LOOP, "offset")
+
+    assert np.allclose(DATA_STACK, DATA_LOOP)
+
+    ddata_stack = fftobj.inverse(DATA_STACK)
+    ddata_loop = np.stack([rect_ifft(DATA_LOOP[i]) for i in range(nstack)])
+    ddata_loop = HexArray(ddata_loop, "offset")
+
+    assert np.allclose(ddata_stack, ddata_loop)
+
+    # test singleton
+    ds = data[0]
+    DS_STACK = fftobj.forward(ds)
+    DS_SINGLE = rect_fft(ds)
+    assert np.allclose(DS_STACK, DS_SINGLE)
+
+    dds_stack = fftobj.inverse(DS_STACK)
+    dds_single = rect_ifft(DS_SINGLE)
+    assert np.allclose(dds_stack, dds_single)
+
+
 def test_hex_fft_stack():
     # create a stack of data
     for pattern in ["oblique", "offset"]:
         for size in [4, 8, 16, 32]:
             nstack, N1, N2 = 5, size, size
             n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
             center = (size // 2, size // 2)
```

### Comparing `hexfft-0.1.0/tests/test_utils.py` & `hexfft-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

