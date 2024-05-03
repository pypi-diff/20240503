# Comparing `tmp/torch_cfd-0.0.3.tar.gz` & `tmp/torch_cfd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_cfd-0.0.3.tar", last modified: Mon Apr 29 03:55:24 2024, max compression
+gzip compressed data, was "torch_cfd-0.0.4.tar", last modified: Fri May  3 03:47:34 2024, max compression
```

## Comparing `torch_cfd-0.0.3.tar` & `torch_cfd-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 03:55:20.000000 torch_cfd-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/torch_cfd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/equations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/fast_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/finite_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/torch_cfd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-03 03:47:28.000000 torch_cfd-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:47:34.820221 torch_cfd-0.0.4/torch_cfd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/fast_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/finite_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/torch_cfd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/top_level.txt
```

### Comparing `torch_cfd-0.0.3/LICENSE` & `torch_cfd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.3/PKG-INFO` & `torch_cfd-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

### Comparing `torch_cfd-0.0.3/setup.py` & `torch_cfd-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'torch-cfd',
   packages=find_packages(include=['torch_cfd', 'torch_cfd.*']),
-  version='0.0.3',
+  version='0.0.4',
   license='Apache-2.0',
   description = 'PyTorch CFD',
   long_description='PyTorch Computational Fluid Dynamics Library',
   long_description_content_type="text/markdown",
   author = 'Shuhao Cao',
   author_email = 'scao.math@gmail.com',
   url = 'https://github.com/scaomath/torch-cfd',
```

### Comparing `torch_cfd-0.0.3/torch_cfd/equations.py` & `torch_cfd-0.0.4/torch_cfd/equations.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,20 +19,52 @@
 
 import torch
 import torch.nn as nn
 import torch.fft as fft
 from . import grids
 from tqdm.auto import tqdm
 
-TQDM_ITERS = 100
+TQDM_ITERS = 500
 
 Array = torch.Tensor
 Grid = grids.Grid
 
 
+def stable_time_step(
+    dx: float = None,
+    dt: float = None,
+    max_velocity: float = 1.0,
+    max_courant_number: float = 0.5,
+    viscosity: float = 1e-3,
+    implicit_diffusion: bool = True,
+    ndim: int = 2,
+) -> float:
+    """
+    Calculate a stable time step satisfying the CFL condition
+    for the explicit advection term
+    if the diffusion is explicit, the time step is the smaller
+    of the advection and diffusion time steps.
+
+    Args:
+    max_velocity: maximum velocity.
+    max_courant_number: the Courant number used to choose the time step. Smaller
+      numbers will lead to more stable simulations. Typically this should be in
+      the range [0.5, 1).
+    dx: spatial mesh size, can be min(grid.step).
+    dt: time step.
+    """
+    dt_diffusion = dx
+
+    if not implicit_diffusion:
+        dt_diffusion = dx ** 2 / (viscosity * 2 ** (ndim))
+    dt_advection = max_courant_number * dx / max_velocity
+    dt = dt_advection if dt is None else dt
+    return min(dt_diffusion, dt_advection, dt)
+
+
 class ImplicitExplicitODE(nn.Module):
     """Describes a set of ODEs with implicit & explicit terms.
 
     The equation is given by:
 
       $\partial x/ \partial t = explicit_terms(x) + implicit_terms(x)$
 
@@ -57,14 +89,98 @@
         x: Array,
         step_size: float,
     ):
         """Solves `y - step_size * implicit_terms(y) = x` for y."""
         raise NotImplementedError
 
 
+def backward_forward_euler(
+    u: torch.Tensor,
+    dt: float,
+    equation: ImplicitExplicitODE,
+) -> Array:
+    """Time stepping via forward and backward Euler methods.
+
+    This method is first order accurate.
+
+    Args:
+        equation: equation to solve.
+        time_step: time step.
+
+    Returns:
+        Function that performs a time step.
+    """
+    F = equation.explicit_terms
+    G_inv = equation.implicit_solve
+
+    g = u + dt * F(u)
+    u = G_inv(g, dt)
+
+    return u
+
+
+def imex_crank_nicolson(
+    u: torch.Tensor,
+    dt: float,
+    equation: ImplicitExplicitODE,
+) -> Array:
+    """Time stepping via forward and backward Euler methods.
+
+    This method is first order accurate.
+
+    Args:
+        equation: equation to solve.
+        time_step: time step.
+
+    Returns:
+        Function that performs a time step.
+    """
+    F = equation.explicit_terms
+    G = equation.implicit_terms
+    G_inv = equation.implicit_solve
+
+    g = u + dt * F(u) + 0.5 * dt * G(u)
+    u = G_inv(g, 0.5 * dt)
+
+    return u
+
+
+def rk2_crank_nicolson(
+    u: torch.Tensor,
+    dt: float,
+    equation: ImplicitExplicitODE,
+) -> Array:
+    """Time stepping via Crank-Nicolson and 2nd order Runge-Kutta (Heun).
+
+    This method is second order accurate.
+
+    Args:
+      equation: equation to solve.
+      time_step: time step.
+
+    Returns:
+      Function that performs a time step.
+
+    Reference:
+      Chandler, G. J. & Kerswell, R. R. Invariant recurrent solutions embedded in
+      a turbulent two-dimensional Kolmogorov flow. J. Fluid Mech. 722, 554–595
+      (2013). https://doi.org/10.1017/jfm.2013.122 (Section 3)
+    """
+    F = equation.explicit_terms
+    G = equation.implicit_terms
+    G_inv = equation.implicit_solve
+
+    g = u + 0.5 * dt * G(u)
+    h = F(u)
+    u = G_inv(g + dt * h, 0.5 * dt)
+    h = 0.5 * (F(u) + h)
+    u = G_inv(g + dt * h, 0.5 * dt)
+    return u
+
+
 def low_storage_runge_kutta_crank_nicolson(
     u: torch.Tensor,
     dt: float,
     params: Dict,
     equation: ImplicitExplicitODE,
 ) -> Array:
     """
@@ -139,16 +255,16 @@
             0.6994504559488,
             0.1530572479681,
         ],
     )
     return low_storage_runge_kutta_crank_nicolson(
         u,
         dt=dt,
-        params=params,
         equation=equation,
+        params=params,
     )
 
 
 class NavierStokes2DSpectral(nn.Module):
     """Breaks the Navier-Stokes equation into implicit and explicit parts.
 
     Implicit parts are the linear terms and explicit parts are the non-linear
@@ -243,24 +359,31 @@
         two_pi_i = 2 * torch.pi * 1j
         laplace = two_pi_i**2 * (abs(kx) ** 2 + abs(ky) ** 2)
         laplace[0, 0] = 1
         psi_hat = -1 / laplace * w_hat
         vxhat = two_pi_i * ky * psi_hat
         vyhat = -two_pi_i * kx * psi_hat
         return vxhat, vyhat
-    
-    def residual(self,
+
+    def residual(
+        self,
         vort_hat: Array,
         vort_t_hat: Array,
     ):
-        residual = vort_t_hat -  self.explicit_terms(vort_hat) - self.viscosity *  self.implicit_terms(vort_hat)
+        residual = (
+            vort_t_hat
+            - self.explicit_terms(vort_hat)
+            - self.viscosity * self.implicit_terms(vort_hat)
+        )
         return residual
 
     def _explicit_terms(self, vort_hat):
-        vxhat, vyhat = self.vorticity_to_velocity(self.grid, vort_hat, (self.kx, self.ky))
+        vxhat, vyhat = self.vorticity_to_velocity(
+            self.grid, vort_hat, (self.kx, self.ky)
+        )
         vx, vy = fft.irfft2(vxhat), fft.irfft2(vyhat)
 
         grad_x_hat = 2j * torch.pi * self.kx * vort_hat
         grad_y_hat = 2j * torch.pi * self.ky * vort_hat
         grad_x, grad_y = fft.irfft2(grad_x_hat), fft.irfft2(grad_y_hat)
 
         advection = -(grad_x * vx + grad_y * vy)
@@ -268,18 +391,22 @@
 
         if self.smooth:
             advection_hat *= self.filter
 
         terms = advection_hat
 
         if self.forcing_fn is not None:
-            fx, fy = self.forcing_fn(self.grid, (vx, vy))
-            fx_hat, fy_hat = fft.rfft2(fx.data), fft.rfft2(fy.data)
-            terms += self.spectral_curl_2d((fx_hat, fy_hat), (self.kx, self.ky))
-
+            if not self.forcing_fn.vorticity:
+                fx, fy = self.forcing_fn(self.grid, (vx, vy))
+                fx_hat, fy_hat = fft.rfft2(fx.data), fft.rfft2(fy.data)
+                terms += self.spectral_curl_2d((fx_hat, fy_hat), (self.kx, self.ky))
+            else:
+                f = self.forcing_fn(self.grid, vort_hat)
+                f_hat = fft.rfft2(f.data)
+                terms += f_hat
         return terms
 
     def explicit_terms(self, vort_hat):
         return self._explicit_terms(vort_hat)
 
     def implicit_terms(self, vort_hat):
         return self.linear_term * vort_hat
@@ -328,15 +455,16 @@
                     v_all.append(v)
                     dwdt_all.append(dwdt_)
                     res_all.append(res)
 
         result = {
             var_name: torch.stack(var, dim=0)
             for var_name, var in zip(
-                ["vorticity", "velocity", "vort_t", "residual"], [w_all, v_all, dwdt_all, res_all]
+                ["vorticity", "velocity", "vort_t", "residual"],
+                [w_all, v_all, dwdt_all, res_all],
             )
         }
         return result
 
     def step(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torch_cfd-0.0.3/torch_cfd/fast_diagonalization.py` & `torch_cfd-0.0.4/torch_cfd/fast_diagonalization.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.3/torch_cfd/finite_differences.py` & `torch_cfd-0.0.4/torch_cfd/finite_differences.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.3/torch_cfd/forcings.py` & `torch_cfd-0.0.4/torch_cfd/forcings.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,51 +11,84 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Modifications copyright (C) 2024 S.Cao
 # ported Google's Jax-CFD functional template to PyTorch's tensor ops
 
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from . import grids
 
 Array = torch.Tensor
 Grid = grids.Grid
 GridArray = grids.GridArray
 
 
+def forcing_eval(eval_func):
+    def wrapper(
+        cls, grid: Grid, field: Optional[Union[Tuple[Array, Array], Array]]
+    ) -> Array:
+        return eval_func(grid, field)
+
+    return wrapper
+
+
 class ForcingFn(nn.Module):
     """
     A meta class for forcing functions
+
+    Args:
+    vorticity: whether the forcing function is a vorticity forcing
     """
 
     def __init__(
         self,
         grid: Grid,
         scale: float = 1,
         k: int = 1,
         diam: float = 1.0,
         swap_xy: bool = False,
+        vorticity: bool = False,
         offsets: Optional[Tuple[Tuple[float, ...], ...]] = None,
         device: Optional[torch.device] = None,
         **kwargs,
     ):
         super().__init__()
         self.grid = grid
         self.scale = scale
         self.k = k
         self.diam = diam
         self.swap_xy = swap_xy
+        self.vorticity = vorticity
         self.offsets = grid.cell_faces if offsets is None else offsets
         self.device = grid.device if device is None else device
 
+    @forcing_eval
+    def velocity_eval(grid: Grid, velocity: Optional[Tuple[Array, Array]]) -> Array:
+        raise NotImplementedError
+
+    @forcing_eval
+    def vorticity_eval(grid: Grid, vorticity: Optional[Array]) -> Array:
+        raise NotImplementedError
+
+    def forward(
+        self,
+        grid: Optional[Grid],
+        velocity: Optional[Tuple[Array, Array]] = None,
+        vorticity: Optional[Array] = None,
+    ) -> Tuple[Array, Array]:
+        if not self.vorticity:
+            return self.velocity_eval(grid, velocity)
+        else:
+            return self.vorticity_eval(grid, vorticity)
+
 
 class KolmogorovForcing(ForcingFn):
     """
     The Kolmogorov forcing function used in
     Sets up the flow that is used in Kochkov et al. [1].
     which is based on Boffetta et al. [2].
 
@@ -77,25 +110,27 @@
     in turbulent flow". Journal of Fluid Mechanics, 146, 21-43.
     """
 
     def __init__(
         self,
         diam=2 * torch.pi,
         offsets=((0, 0), (0, 0)),
+        vorticity=False,
         *args,
         **kwargs,
     ):
         super().__init__(
             *args,
             diam=diam,
             offsets=offsets,
+            vorticity=vorticity,
             **kwargs,
         )
 
-    def forward(
+    def velocity_eval(
         self,
         grid: Optional[Grid],
         velocity: Optional[Tuple[Array, Array]] = None,
     ) -> Tuple[Array, Array]:
         offsets = self.offsets
         grid = self.grid if grid is None else grid
         domain_factor = 2 * torch.pi / self.diam
@@ -112,55 +147,93 @@
             u = GridArray(
                 self.scale * torch.sin(self.k * domain_factor * y), offsets[0], grid
             )
             v = GridArray(torch.zeros_like(u.data), (1 / 2, 1), grid)
             f = (u, v)
         return f
 
-def potential_template(potential_func):
+    def vorticity_eval(
+        self,
+        grid: Optional[Grid],
+        vorticity: Optional[Array] = None,
+    ) -> Array:
+        offsets = self.offsets
+        grid = self.grid if grid is None else grid
+        domain_factor = 2 * torch.pi / self.diam
+
+        if self.swap_xy:
+            x = grid.mesh(offsets[1])[0]
+            w = GridArray(
+                -self.scale
+                * self.k
+                * domain_factor
+                * torch.cos(self.k * domain_factor * x),
+                offsets[1],
+                grid,
+            )
+        else:
+            y = grid.mesh(offsets[0])[1]
+            w = GridArray(
+                -self.scale
+                * self.k
+                * domain_factor
+                * torch.cos(self.k * domain_factor * y),
+                offsets[0],
+                grid,
+            )
+        return w
+
+
+def scalar_potential(potential_func):
     def wrapper(cls, x: Array, y: Array, s: float, k: float) -> Array:
         return potential_func(x, y, s, k)
+
     return wrapper
-    
+
 
 class SimpleSolenoidalForcing(ForcingFn):
     """
     A simple solenoidal (rotating, divergence free) forcing function template.
-    The template forcing is F = (-psi, psi) such that 
-    
+    The template forcing is F = (-psi, psi) such that
+
     Args:
     grid: grid on which to simulate the flow
     scale: a in the equation above, amplitude of the forcing
     k: k in the equation above, wavenumber of the forcing
     """
 
     def __init__(
         self,
         scale=1,
         diam=1.0,
         k=1.0,
         offsets=((0, 0), (0, 0)),
+        vorticity=True,
         *args,
         **kwargs,
     ):
         super().__init__(
             *args,
             scale=scale,
             diam=diam,
             k=k,
             offsets=offsets,
+            vorticity=vorticity,
             **kwargs,
         )
-    
 
-    @potential_template
+    @scalar_potential
     def potential(*args, **kwargs) -> Array:
         raise NotImplementedError
 
-    def forward(
+    @scalar_potential
+    def vort_potential(*args, **kwargs) -> Array:
+        raise NotImplementedError
+
+    def velocity_eval(
         self,
         grid: Optional[Grid],
         velocity: Optional[Tuple[Array, Array]] = None,
     ) -> Tuple[Array, Array]:
         offsets = self.offsets
         grid = self.grid if grid is None else grid
         domain_factor = 2 * torch.pi / self.diam
@@ -179,14 +252,34 @@
             y = grid.mesh(offsets[1])[1]
             rot = self.potential(x, y, scale, k)
             u = GridArray(rot, offsets[0], grid)
             v = GridArray(-rot, (1 / 2, 1), grid)
             f = (u, v)
         return f
 
+    def vorticity_eval(
+        self,
+        grid: Optional[Grid],
+        vorticity: Optional[Array] = None,
+    ) -> Array:
+        offsets = self.offsets
+        grid = self.grid if grid is None else grid
+        domain_factor = 2 * torch.pi / self.diam
+        k = self.k * domain_factor
+        scale = self.scale
+
+        if self.swap_xy:
+            x = grid.mesh(offsets[1])[0]
+            y = grid.mesh(offsets[0])[1]
+            return self.vort_potential(x, y, scale, k)
+        else:
+            x = grid.mesh(offsets[0])[0]
+            y = grid.mesh(offsets[1])[1]
+            return self.vort_potential(x, y, scale, k)
+
 
 class SinCosForcing(SimpleSolenoidalForcing):
     """
     The solenoidal (divergence free) forcing function used in [4].
 
     Note: in the vorticity-streamfunction formulation, the forcing
     is actually the curl of the velocity field, which
@@ -218,10 +311,14 @@
             scale=scale,
             diam=diam,
             k=k,
             offsets=offsets,
             **kwargs,
         )
 
-    @potential_template
+    @scalar_potential
     def potential(x: Array, y: Array, s: float, k: float) -> Array:
-        return s * (torch.sin(k * (x + y)) - torch.cos(k * (x + y)))
+        return s * (torch.sin(k * (x + y)) - torch.cos(k * (x + y)))
+
+    @scalar_potential
+    def vort_potential(x: Array, y: Array, s: float, k: float) -> Array:
+        return s * (torch.cos(k * (x + y)) + torch.sin(k * (x + y)))
```

### Comparing `torch_cfd-0.0.3/torch_cfd/grids.py` & `torch_cfd-0.0.4/torch_cfd/grids.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.3/torch_cfd/initial_conditions.py` & `torch_cfd-0.0.4/torch_cfd/initial_conditions.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,22 +41,43 @@
     """Wrap velocity arrays for input into simulations."""
     device = grid.device if device is None else device
     return tuple(
         GridVariable(GridArray(u, offset, grid).to(device), bc)
         for u, offset, bc in zip(v, grid.cell_faces, bcs)
     )
 
+def wrap_vorticity(
+    w: Array,
+    grid: grids.Grid,
+    bc: BoundaryConditions,
+    device: Optional[torch.device] = None,
+) -> GridVariable:
+    """Wrap vorticity arrays for input into simulations."""
+    device = grid.device if device is None else device
+    return GridVariable(GridArray(w, grid.cell_faces, grid).to(device), bc)
+
 
-def _log_normal_pdf(x, mode: float, variance=0.25):
+def _log_normal_density(k, mode: float, variance=0.25):
     """Unscaled PDF for a log normal given `mode` and log variance 1."""
     mean = math.log(mode) + variance
-    logx = torch.log(x)
-    return torch.exp(-((mean - logx) ** 2) / 2 / variance - logx)
+    logk = torch.log(k)
+    return torch.exp(-((mean - logk) ** 2) / 2 / variance - logk)
 
 
+def McWilliams_density(k, mode: float, tau: float = 1.0):
+    """Implements the McWilliams spectral density function.
+    |\psi|^2 \sim k^{-1}(tau^2 + (k/k_0)^4)^{-1}
+    k_0 is a prescribed wavenumber that the energy peaks.
+    tau flattens the spectrum density at low wavenumbers to be bigger.
+
+    Refs:
+      McWilliams, J. C. (1984). The emergence of isolated coherent vortices in turbulent flow.
+    """
+    return (k * (tau**2 + (k / mode) ** 4)) ** (-1)
+
 def _angular_frequency_magnitude(grid: grids.Grid) -> Array:
     frequencies = [
         2 * torch.pi * fft.fftfreq(size, step)
         for size, step in zip(grid.shape, grid.step)
     ]
     freq_vector = torch.stack(torch.meshgrid(*frequencies, indexing="ij"), axis=0)
     return torch.linalg.norm(freq_vector, axis=0)
@@ -70,14 +91,21 @@
     """Filter an Array with white noise to match a prescribed spectral density."""
     k = _angular_frequency_magnitude(grid)
     filters = torch.where(k > 0, spectral_density(k), 0.0)
     # The output signal can safely be assumed to be real if our input signal was
     # real, because our spectral density only depends on norm(k).
     return fft.ifftn(fft.fftn(v) * filters).real
 
+def streamfunc_normalize(k, psi):
+    # only half the spectrum for real ffts, needs spectral normalisation
+    nx, ny = psi.shape
+    psih = fft.fft2(psi)
+    uh = k * psih
+    kinetic_energy = (2 * uh.abs() ** 2 / (nx * ny) ** 2).sum()
+    return psi / kinetic_energy.sqrt()
 
 def _rhs_transform(
     u: GridArray,
     bc: BoundaryConditions,
 ) -> Array:
     """Transform the RHS of pressure projection equation for stability.
 
@@ -139,15 +167,17 @@
     v: GridVariableVector,
     solve: Callable = solve_fast_diag,
 ) -> GridVariableVector:
     """
     Apply pressure projection (a discrete Helmholtz decomposition)
     to make a velocity field divergence free.
     
-    Note: this will have a non-negligible error in fp32.
+    Note by S.Cao: this was originally implemented by the jax-cfd team
+    but using FDM results having a non-negligible error in fp32. 
+    One resolution is to use fp64 then cast back to fp32.
     """
     grid = grids.consistent_grid(*v)
     pressure_bc = grids.get_pressure_bc_from_velocity(v)
 
     q0 = GridArray(torch.zeros(grid.shape), grid.cell_center, grid)
     q0 = pressure_bc.impose_bc(q0)
 
@@ -189,15 +219,15 @@
       periodic boundary conditions with the velocity field components.
     """
 
     # Log normal distribution peaked at `peak_wavenumber`. Note that we have to
     # divide by `k ** (ndim - 1)` to account for the volume of the
     # `ndim - 1`-sphere of values with wavenumber `k`.
     def spectral_density(k):
-        return _log_normal_pdf(k, peak_wavenumber) / k ** (grid.ndim - 1)
+        return _log_normal_density(k, peak_wavenumber) / k ** (grid.ndim - 1)
 
     random_states = [random_state + i for i in range(grid.ndim)]
     rng = torch.Generator()
     velocity_components = []
     boundary_conditions = []
     for k in random_states:
         rng.manual_seed(k)
@@ -209,7 +239,42 @@
     # Due to numerical precision issues, we repeatedly normalize and project the
     # velocity field. This ensures that it is divergence-free and achieves the
     # specified maximum velocity.
     # velocity is ((n, n), (n, n)) GridVariableVector
     for _ in range(iterations):
         velocity = project_and_normalize(velocity, maximum_velocity)
     return velocity
+
+
+def vorticity_field(
+    grid: grids.Grid,
+    peak_wavenumber: float = 3,
+    random_state: int = 0,
+) -> GridArray:
+    """Create vorticity field with a spectral filtering
+    using the McWilliams power spectrum density function.
+
+    Args:
+      rng_key: key for seeding the random initial vorticity field.
+      grid: the grid on which the vorticity field is defined.
+      maximum_velocity: the maximum speed in the velocity field.
+      peak_wavenumber: the velocity field will be filtered so that the largest
+        magnitudes are associated with this wavenumber.
+
+    Returns:
+      A vorticity field with periodic boundary condition.
+    """
+
+    def spectral_density(k):
+        return McWilliams_density(k, peak_wavenumber)
+
+    rng = torch.Generator()
+    rng.manual_seed(random_state)
+    noise = torch.randn(grid.shape, generator=rng)
+    k = _angular_frequency_magnitude(grid)
+    psi = spectral_filter(spectral_density, noise, grid)
+    psi = streamfunc_normalize(k, psi)
+    vorticity = fft.ifftn(fft.fftn(psi) * k**2).real
+    boundary_condition = grids.periodic_boundary_conditions(grid.ndim)
+    vorticity = wrap_vorticity(vorticity, grid, boundary_condition)
+
+    return vorticity
```

### Comparing `torch_cfd-0.0.3/torch_cfd/tensor_utils.py` & `torch_cfd-0.0.4/torch_cfd/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.3/torch_cfd.egg-info/PKG-INFO` & `torch_cfd-0.0.4/torch_cfd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

