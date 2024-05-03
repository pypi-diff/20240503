# Comparing `tmp/bosing-2.0.0b9.tar.gz` & `tmp/bosing-2.0.1.tar.gz`

## Comparing `bosing-2.0.0b9.tar` & `bosing-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 bosing-2.0.0b9/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.github/dependabot.yml
--rw-r--r--   0     1001      127     6323 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.gitignore
--rw-r--r--   0     1001      127      972 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-04-29 16:20:07.000000 bosing-2.0.0b9/LICENSE.txt
--rw-r--r--   0     1001      127     1360 2024-04-29 16:20:07.000000 bosing-2.0.0b9/README.md
--rw-r--r--   0     1001      127    10696 2024-04-29 16:20:07.000000 bosing-2.0.0b9/bosing.pyi
--rw-r--r--   0     1001      127       78 2024-04-29 16:20:07.000000 bosing-2.0.0b9/clippy.toml
--rw-r--r--   0     1001      127      634 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/quickstart.rst
--rw-r--r--   0     1001      127       22 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/schedule.rst
--rw-r--r--   0     1001      127     1171 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/flexible.py
--rw-r--r--   0     1001      127      533 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/hann.py
--rw-r--r--   0     1001      127      788 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/interp.py
--rw-r--r--   0     1001      127      696 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/overlap.py
--rw-r--r--   0     1001      127     2074 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/schedule.py
--rw-r--r--   0     1001      127     2329 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-04-29 16:20:07.000000 bosing-2.0.0b9/ruff_defaults.toml
--rw-r--r--   0     1001      127     7368 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/executor.rs
--rw-r--r--   0     1001      127    66930 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/lib.rs
--rw-r--r--   0     1001      127    12363 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/pulse.rs
--rw-r--r--   0     1001      127     1667 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/quant.rs
--rw-r--r--   0     1001      127     2481 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7389 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3326 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/play.rs
--rw-r--r--   0     1001      127     2350 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3966 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5760 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/stack.rs
--rw-r--r--   0     1001      127    11084 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule.rs
--rw-r--r--   0     1001      127     6642 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-04-29 16:20:07.000000 bosing-2.0.0b9/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-04-29 16:20:07.000000 bosing-2.0.0b9/tests/__init__.py
--rw-r--r--   0     1001      127     1291 2024-04-29 16:20:07.000000 bosing-2.0.0b9/tests/test_basic.py
--rw-r--r--   0     1001      127    18617 2024-04-29 16:20:12.000000 bosing-2.0.0b9/Cargo.lock
--rw-r--r--   0     1001      127     1863 2024-04-29 16:20:07.000000 bosing-2.0.0b9/pyproject.toml
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 bosing-2.0.0b9/PKG-INFO
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 bosing-2.0.1/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-05-03 09:42:22.000000 bosing-2.0.1/.github/dependabot.yml
+-rw-r--r--   0     1001      127      690 2024-05-03 09:42:22.000000 bosing-2.0.1/.github/workflows/auto-dep.yml
+-rw-r--r--   0     1001      127     6323 2024-05-03 09:42:22.000000 bosing-2.0.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-05-03 09:42:22.000000 bosing-2.0.1/.gitignore
+-rw-r--r--   0     1001      127      972 2024-05-03 09:42:22.000000 bosing-2.0.1/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-05-03 09:42:22.000000 bosing-2.0.1/LICENSE.txt
+-rw-r--r--   0     1001      127     1360 2024-05-03 09:42:22.000000 bosing-2.0.1/README.md
+-rw-r--r--   0     1001      127    10767 2024-05-03 09:42:22.000000 bosing-2.0.1/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-05-03 09:42:22.000000 bosing-2.0.1/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/quickstart.rst
+-rw-r--r--   0     1001      127       22 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/schedule.rst
+-rw-r--r--   0     1001      127     1171 2024-05-03 09:42:22.000000 bosing-2.0.1/example/flexible.py
+-rw-r--r--   0     1001      127      533 2024-05-03 09:42:22.000000 bosing-2.0.1/example/hann.py
+-rw-r--r--   0     1001      127      788 2024-05-03 09:42:22.000000 bosing-2.0.1/example/interp.py
+-rw-r--r--   0     1001      127      696 2024-05-03 09:42:22.000000 bosing-2.0.1/example/overlap.py
+-rw-r--r--   0     1001      127     2074 2024-05-03 09:42:22.000000 bosing-2.0.1/example/schedule.py
+-rw-r--r--   0     1001      127     2343 2024-05-03 09:42:22.000000 bosing-2.0.1/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-05-03 09:42:22.000000 bosing-2.0.1/ruff_defaults.toml
+-rw-r--r--   0     1001      127     7345 2024-05-03 09:42:22.000000 bosing-2.0.1/src/executor.rs
+-rw-r--r--   0     1001      127    63044 2024-05-03 09:42:22.000000 bosing-2.0.1/src/lib.rs
+-rw-r--r--   0     1001      127    12435 2024-05-03 09:42:22.000000 bosing-2.0.1/src/pulse.rs
+-rw-r--r--   0     1001      127     6647 2024-05-03 09:42:22.000000 bosing-2.0.1/src/quant.rs
+-rw-r--r--   0     1001      127     2662 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7589 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3561 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2490 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     4225 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5752 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    10472 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule.rs
+-rw-r--r--   0     1001      127     7649 2024-05-03 09:42:22.000000 bosing-2.0.1/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-05-03 09:42:22.000000 bosing-2.0.1/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-05-03 09:42:22.000000 bosing-2.0.1/tests/__init__.py
+-rw-r--r--   0     1001      127     1291 2024-05-03 09:42:22.000000 bosing-2.0.1/tests/test_basic.py
+-rw-r--r--   0     1001      127    18328 2024-05-03 09:42:30.000000 bosing-2.0.1/Cargo.lock
+-rw-r--r--   0     1001      127     1863 2024-05-03 09:42:22.000000 bosing-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 bosing-2.0.1/PKG-INFO
```

### Comparing `bosing-2.0.0b9/Cargo.toml` & `bosing-2.0.1/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [package]
 name = "bosing"
-version = "2.0.0-beta.9"
+version = "2.0.1"
 edition = "2021"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bosing"
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0.82"
 bspline = "1.1.0"
-cached = "0.49.3"
-enum_dispatch = "0.3.13"
+cached = "0.50.0"
 float-cmp = "0.9.0"
-hashbrown = { version = "0.14.3", features = ["rayon"] }
+hashbrown = { version = "0.14.5", features = ["rayon"] }
 indoc = "2.0.5"
 itertools = "0.12.1"
 ndarray = { version = "0.15.6", features = ["rayon"] }
-num = "0.4.1"
+num = "0.4.2"
 numpy = "0.21.0"
 ordered-float = "4.2.0"
-pyo3 = { version = "0.21.0", features = ["hashbrown"] }
+pyo3 = { version = "0.21.2", features = ["hashbrown", "anyhow"] }
 rayon = "1.10.0"
```

### Comparing `bosing-2.0.0b9/.github/workflows/ci.yml` & `bosing-2.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/.gitignore` & `bosing-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/.readthedocs.yaml` & `bosing-2.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/LICENSE.txt` & `bosing-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/README.md` & `bosing-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/bosing.pyi` & `bosing-2.0.1/bosing.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,39 +11,42 @@
         base_freq: float,
         sample_rate: float,
         length: int,
         *,
         delay: float = ...,
         align_level: int = ...,
         iq_matrix: npt.ArrayLike | None = ...,
-        iq_offset: tuple[float, float] = ...,
+        offset: npt.ArrayLike | None = ...,
         iir: npt.ArrayLike | None = ...,
         fir: npt.ArrayLike | None = ...,
         filter_offset: bool = ...,
+        is_real: bool = ...,
     ) -> Self: ...
     @property
     def base_freq(self) -> float: ...
     @property
     def sample_rate(self) -> float: ...
     @property
     def length(self) -> int: ...
     @property
     def delay(self) -> float: ...
     @property
     def align_level(self) -> int: ...
     @property
     def iq_matrix(self) -> np.ndarray | None: ...
     @property
-    def iq_offset(self) -> tuple[float, float]: ...
+    def offset(self) -> np.ndarray | None: ...
     @property
     def iir(self) -> np.ndarray | None: ...
     @property
     def fir(self) -> np.ndarray | None: ...
     @property
     def filter_offset(self) -> bool: ...
+    @property
+    def is_real(self) -> bool: ...
 
 @final
 class Alignment:
     End: ClassVar[Alignment]
     Start: ClassVar[Alignment]
     Center: ClassVar[Alignment]
     Stretch: ClassVar[Alignment]
```

### Comparing `bosing-2.0.0b9/docs/Makefile` & `bosing-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/docs/_templates/autosummary/module.rst` & `bosing-2.0.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/docs/conf.py` & `bosing-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/docs/index.rst` & `bosing-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/docs/instruction.rst` & `bosing-2.0.1/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/docs/make.bat` & `bosing-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/docs/schedule.rst` & `bosing-2.0.1/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/example/flexible.py` & `bosing-2.0.1/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/example/hann.py` & `bosing-2.0.1/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/example/interp.py` & `bosing-2.0.1/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/example/overlap.py` & `bosing-2.0.1/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/example/schedule.py` & `bosing-2.0.1/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/example/schedule_stress.py` & `bosing-2.0.1/example/schedule_stress.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     nxy = 64
     nu = 2 * nxy
     nm = nxy // 8
     iir = get_biquad([0.1, -0.1], [100e-9, 1e-6], 2e9)
     fir = [1, 0.1, 0.01, 0.001]
     channels = (
         {f"xy{i}": Channel(3e6 * i, 2e9, 100000, iq_matrix=[[1, 0.1], [0.1, 1]]) for i in range(nxy)}
-        | {f"u{i}": Channel(0, 2e9, 100000, iir=iir, fir=fir) for i in range(nu)}
+        | {f"u{i}": Channel(0, 2e9, 100000, iir=iir, fir=fir, is_real=True) for i in range(nu)}
         | {f"m{i}": Channel(0, 2e9, 100000) for i in range(nm)}
     )
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     spline = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
     shapes = {
         "hann": Hann(),
         "halfcos": Interp(spline.t, spline.c, spline.k),
```

### Comparing `bosing-2.0.0b9/ruff_defaults.toml` & `bosing-2.0.1/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/src/executor.rs` & `bosing-2.0.1/src/executor.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 use hashbrown::HashMap;
 
 use crate::{
     pulse::{Envelope, PulseList, PulseListBuilder},
-    quant::{Frequency, Time},
+    quant::{Amplitude, ChannelId, Frequency, Phase, ShapeId, Time},
     schedule::{self, ArrangedElement, ElementVariant},
     shape::Shape,
 };
 
 #[derive(Debug, Clone)]
 pub struct Executor {
-    channels: HashMap<String, Channel>,
-    shapes: HashMap<String, Shape>,
-    amp_tolerance: f64,
-    time_tolerance: f64,
+    channels: HashMap<ChannelId, Channel>,
+    shapes: HashMap<ShapeId, Shape>,
+    amp_tolerance: Amplitude,
+    time_tolerance: Time,
 }
 
 impl Executor {
-    pub fn new(amp_tolerance: f64, time_tolerance: f64) -> Self {
+    pub fn new(amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
         Self {
             channels: HashMap::new(),
             shapes: HashMap::new(),
             amp_tolerance,
             time_tolerance,
         }
     }
 
-    pub fn add_channel(&mut self, name: String, base_freq: f64) {
+    pub fn add_channel(&mut self, name: ChannelId, base_freq: Frequency) {
         self.channels.insert(
             name,
             Channel::new(base_freq, self.amp_tolerance, self.time_tolerance),
         );
     }
 
-    pub fn add_shape(&mut self, name: String, shape: Shape) {
+    pub fn add_shape(&mut self, name: ShapeId, shape: Shape) {
         self.shapes.insert(name, shape);
     }
 
     pub fn execute(&mut self, element: &ArrangedElement) {
-        self.execute_dispatch(element, 0.0);
+        self.execute_dispatch(element, Time::ZERO);
     }
 
-    pub fn into_result(self) -> HashMap<String, PulseList> {
+    pub fn into_result(self) -> HashMap<ChannelId, PulseList> {
         self.channels
             .into_iter()
             .map(|(n, b)| (n, b.pulses.build()))
             .collect()
     }
 
-    fn execute_dispatch(&mut self, element: &ArrangedElement, time: f64) {
-        if element.element().common().phantom() {
+    fn execute_dispatch(&mut self, element: &ArrangedElement, time: Time) {
+        if element.element().common.phantom() {
             return;
         }
         let time = time + element.inner_time();
         let duration = element.inner_duration();
-        match element.element().variant() {
+        match &element.element().variant {
             ElementVariant::Play(e) => self.execute_play(e, time, duration),
             ElementVariant::ShiftPhase(e) => self.execute_shift_phase(e),
             ElementVariant::SetPhase(e) => self.execute_set_phase(e, time),
             ElementVariant::ShiftFreq(e) => self.execute_shift_freq(e, time),
             ElementVariant::SetFreq(e) => self.execute_set_freq(e, time),
             ElementVariant::SwapPhase(e) => self.execute_swap_phase(e, time),
             ElementVariant::Barrier(_) => (),
@@ -68,160 +68,157 @@
             ElementVariant::Stack(_) | ElementVariant::Absolute(_) | ElementVariant::Grid(_) => {
                 let children = element.try_get_children().expect("Invalid arrange data");
                 self.execute_container(children, time);
             }
         }
     }
 
-    fn execute_play(&mut self, element: &schedule::Play, time: f64, duration: f64) {
+    fn execute_play(&mut self, element: &schedule::Play, time: Time, duration: Time) {
         let shape = element.shape_id().map(|id| self.shapes[id].clone());
         let width = element.width();
         let plateau = if element.flexible() {
             duration - width
         } else {
             element.plateau()
         };
         let amplitude = element.amplitude();
         let drag_coef = element.drag_coef();
         let freq = element.frequency();
         let phase = element.phase();
-        let time = Time::new(time).unwrap();
-        let width = Time::new(width).unwrap();
-        let plateau = Time::new(plateau).unwrap();
         let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.add_pulse(
             shape, time, width, plateau, amplitude, drag_coef, freq, phase,
         );
     }
 
     fn execute_shift_phase(&mut self, element: &schedule::ShiftPhase) {
         let delta_phase = element.phase();
         let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.shift_phase(delta_phase);
     }
 
-    fn execute_set_phase(&mut self, element: &schedule::SetPhase, time: f64) {
+    fn execute_set_phase(&mut self, element: &schedule::SetPhase, time: Time) {
         let phase = element.phase();
         let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.set_phase(phase, time);
     }
 
-    fn execute_shift_freq(&mut self, element: &schedule::ShiftFreq, time: f64) {
+    fn execute_shift_freq(&mut self, element: &schedule::ShiftFreq, time: Time) {
         let delta_freq = element.frequency();
         let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.shift_freq(delta_freq, time);
     }
 
-    fn execute_set_freq(&mut self, element: &schedule::SetFreq, time: f64) {
+    fn execute_set_freq(&mut self, element: &schedule::SetFreq, time: Time) {
         let freq = element.frequency();
         let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.set_freq(freq, time);
     }
 
-    fn execute_swap_phase(&mut self, element: &schedule::SwapPhase, time: f64) {
+    fn execute_swap_phase(&mut self, element: &schedule::SwapPhase, time: Time) {
         let ch1 = element.channel_id1();
         let ch2 = element.channel_id2();
         if ch1 == ch2 {
             return;
         }
         let [channel, other] = self.channels.get_many_mut([ch1, ch2]).unwrap();
         channel.swap_phase(other, time);
     }
 
     fn execute_repeat(
         &mut self,
         element: &schedule::Repeat,
         child: &ArrangedElement,
-        time: f64,
-        duration: f64,
+        time: Time,
+        duration: Time,
     ) {
         let count = element.count();
         if count == 0 {
             return;
         }
         let spacing = element.spacing();
         let time_step = (duration + spacing) / count as f64;
         for i in 0..count {
             let child_time = time + i as f64 * time_step;
             self.execute_dispatch(child, child_time);
         }
     }
 
-    fn execute_container(&mut self, children: &[ArrangedElement], time: f64) {
+    fn execute_container(&mut self, children: &[ArrangedElement], time: Time) {
         for child in children {
             self.execute_dispatch(child, time);
         }
     }
 }
 
 #[derive(Debug, Clone)]
 struct Channel {
-    base_freq: f64,
-    delta_freq: f64,
-    phase: f64,
+    base_freq: Frequency,
+    delta_freq: Frequency,
+    phase: Phase,
     pulses: PulseListBuilder,
 }
 
 impl Channel {
-    fn new(base_freq: f64, amp_tolerance: f64, time_tolerance: f64) -> Self {
+    fn new(base_freq: Frequency, amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
         Self {
             base_freq,
-            delta_freq: 0.0,
-            phase: 0.0,
+            delta_freq: Frequency::ZERO,
+            phase: Phase::ZERO,
             pulses: PulseListBuilder::new(amp_tolerance, time_tolerance),
         }
     }
 
-    fn shift_freq(&mut self, delta_freq: f64, time: f64) {
+    fn shift_freq(&mut self, delta_freq: Frequency, time: Time) {
         let delta_phase = -delta_freq * time;
         self.delta_freq += delta_freq;
         self.phase += delta_phase;
     }
 
-    fn set_freq(&mut self, freq: f64, time: f64) {
+    fn set_freq(&mut self, freq: Frequency, time: Time) {
         let delta_freq = freq - self.delta_freq;
         let delta_phase = -delta_freq * time;
         self.delta_freq = freq;
         self.phase += delta_phase;
     }
 
-    fn shift_phase(&mut self, delta_phase: f64) {
+    fn shift_phase(&mut self, delta_phase: Phase) {
         self.phase += delta_phase;
     }
 
-    fn set_phase(&mut self, phase: f64, time: f64) {
+    fn set_phase(&mut self, phase: Phase, time: Time) {
         self.phase = phase - self.delta_freq * time;
     }
 
-    fn total_freq(&self) -> f64 {
+    fn total_freq(&self) -> Frequency {
         self.base_freq + self.delta_freq
     }
 
-    fn swap_phase(&mut self, other: &mut Self, time: f64) {
+    fn swap_phase(&mut self, other: &mut Self, time: Time) {
         let delta_freq = self.total_freq() - other.total_freq();
         let phase1 = self.phase;
         let phase2 = other.phase;
         self.phase = phase2 - delta_freq * time;
         other.phase = phase1 + delta_freq * time;
     }
 
     fn add_pulse(
         &mut self,
         shape: Option<Shape>,
         time: Time,
         width: Time,
         plateau: Time,
-        amplitude: f64,
+        amplitude: Amplitude,
         drag_coef: f64,
-        freq: f64,
-        phase: f64,
+        freq: Frequency,
+        phase: Phase,
     ) {
         let envelope = Envelope::new(shape, width, plateau);
-        let global_freq = Frequency::new(self.total_freq()).unwrap();
-        let local_freq = Frequency::new(freq).unwrap();
+        let global_freq = self.total_freq();
+        let local_freq = freq;
         self.pulses.push(
             envelope,
             global_freq,
             local_freq,
             time,
             amplitude,
             drag_coef,
```

### Comparing `bosing-2.0.0b9/src/lib.rs` & `bosing-2.0.1/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,142 @@
 //! Although Element struct may contains [`Py<Element>`] as children, it is not
 //! possible to create cyclic references because we don't allow mutate the
 //! children after creation.
-use std::sync::Arc;
+use std::{borrow::Borrow, fmt::Debug, sync::Arc};
 
 use hashbrown::HashMap;
 use indoc::indoc;
 use numpy::{
-    dot_bound, prelude::*, pyarray_bound, AllowTypeChange, PyArray1, PyArray2, PyArrayLike1,
-    PyArrayLike2,
+    dot_bound, prelude::*, AllowTypeChange, PyArray1, PyArray2, PyArrayLike1, PyArrayLike2,
 };
 use pyo3::{
-    exceptions::{PyRuntimeError, PyTypeError, PyValueError},
+    exceptions::{PyTypeError, PyValueError},
     prelude::*,
-    types::PyDict,
+    types::{DerefToPyAny, PyDict},
 };
+use rayon::prelude::*;
 
-use crate::{
-    executor::Executor,
-    pulse::Sampler,
-    quant::{Frequency, Time},
-    schedule::ElementCommonBuilder,
-};
+use executor::Executor;
+use pulse::{PulseList, Sampler};
+use quant::{Amplitude, ChannelId, Frequency, Phase, ShapeId, Time};
+use schedule::{ElementCommonBuilder, ElementRef};
 
 mod executor;
 mod pulse;
 mod quant;
 mod schedule;
 mod shape;
 
 /// Channel configuration.
 ///
 /// `align_level` is the time axis alignment granularity. With sampling interval
 /// :math:`\Delta t` and `align_level` :math:`n`, start of pulse is aligned to
 /// the nearest multiple of :math:`2^n \Delta t`.
 ///
+/// Each channel can be either real or complex. If the channel is complex, the
+/// filter will be applied to both I and Q components. If the channel is real,
+/// `iq_matrix` will be ignored.
+///
+/// .. caution::
+///
+///     Crosstalk matrix will not be applied to offset.
+///
 /// Args:
 ///     base_freq (float): Base frequency of the channel.
 ///     sample_rate (float): Sample rate of the channel.
 ///     length (int): Length of the waveform.
 ///     delay (float): Delay of the channel. Defaults to 0.0.
 ///     align_level (int): Time axis alignment granularity. Defaults to -10.
 ///     iq_matrix (array_like[2, 2] | None): IQ matrix of the channel. Defaults
-///         to None.
-///     iq_offset (tuple[float, float]): IQ offset of the channel. Defaults to
-///         (0.0, 0.0).
+///         to ``None``.
+///     offset (Sequence[float] | None): Offsets of the channel. The length of the
+///         sequence should be 2 if the channel is complex, or 1 if the channel is
+///         real. Defaults to ``None``.
 ///     iir (array_like[N, 6] | None): IIR filter of the channel. The format of
 ///         the array is ``[[b0, b1, b2, a0, a1, a2], ...]``, which is the same
-///         as `sos` parameter of :func:`scipy.signal.sosfilt`. Defaults to None.
+///         as `sos` parameter of :func:`scipy.signal.sosfilt`. Defaults to ``None``.
 ///     fir (array_like[M] | None): FIR filter of the channel. Defaults to None.
 ///     filter_offset (bool): Whether to apply filter to the offset. Defaults to
-///         False.
+///         ``False``.
+///     is_real (bool): Whether the channel is real. Defaults to ``False``.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Channel {
-    base_freq: f64,
-    sample_rate: f64,
+    base_freq: Frequency,
+    sample_rate: Frequency,
     length: usize,
-    delay: f64,
+    delay: Time,
     align_level: i32,
     iq_matrix: Option<Py<PyArray2<f64>>>,
-    iq_offset: (f64, f64),
+    offset: Option<Py<PyArray1<f64>>>,
     iir: Option<Py<PyArray2<f64>>>,
     fir: Option<Py<PyArray1<f64>>>,
     filter_offset: bool,
+    is_real: bool,
 }
 
 #[pymethods]
 impl Channel {
     #[new]
     #[pyo3(signature = (
         base_freq,
         sample_rate,
         length,
         *,
-        delay=0.0,
+        delay=Time::ZERO,
         align_level=-10,
         iq_matrix=None,
-        iq_offset=(0.0, 0.0),
+        offset=None,
         iir=None,
         fir=None,
         filter_offset=false,
+        is_real=false,
     ))]
+    #[allow(clippy::too_many_arguments)]
     fn new(
-        py: Python<'_>,
-        base_freq: f64,
-        sample_rate: f64,
+        py: Python,
+        base_freq: Frequency,
+        sample_rate: Frequency,
         length: usize,
-        delay: f64,
+        delay: Time,
         align_level: i32,
-        iq_matrix: Option<PyArrayLike2<f64, AllowTypeChange>>,
-        iq_offset: (f64, f64),
+        mut iq_matrix: Option<PyArrayLike2<f64, AllowTypeChange>>,
+        offset: Option<PyArrayLike1<f64, AllowTypeChange>>,
         iir: Option<PyArrayLike2<f64, AllowTypeChange>>,
         fir: Option<PyArrayLike1<f64, AllowTypeChange>>,
         filter_offset: bool,
+        is_real: bool,
     ) -> PyResult<Self> {
+        if is_real {
+            iq_matrix = None;
+        }
         let iq_matrix = if let Some(iq_matrix) = iq_matrix {
             if iq_matrix.shape() != [2, 2] {
                 return Err(PyValueError::new_err("iq_matrix should be a 2x2 matrix"));
             }
             let kwargs = PyDict::new_bound(py);
             kwargs.set_item("write", false)?;
             iq_matrix.getattr("setflags")?.call((), Some(&kwargs))?;
             Some(Bound::clone(&iq_matrix).unbind())
         } else {
             None
         };
+        let offset = if let Some(offset) = offset {
+            if !matches!((offset.len(), is_real), (1, true) | (2, false)) {
+                return Err(PyValueError::new_err(
+                    "offset length does not match is_real",
+                ));
+            }
+            let kwargs = PyDict::new_bound(py);
+            kwargs.set_item("write", false)?;
+            offset.getattr("setflags")?.call((), Some(&kwargs))?;
+            Some(Bound::clone(&offset).unbind())
+        } else {
+            None
+        };
         let iir = if let Some(iir) = iir {
             if !matches!(iir.shape(), [_, 6]) {
                 return Err(PyValueError::new_err("iir should be a Nx6 matrix"));
             }
             let kwargs = PyDict::new_bound(py);
             kwargs.set_item("write", false)?;
             iir.getattr("setflags")?.call((), Some(&kwargs))?;
@@ -127,18 +155,19 @@
         Ok(Channel {
             base_freq,
             sample_rate,
             length,
             delay,
             align_level,
             iq_matrix,
-            iq_offset,
+            offset,
             iir,
             fir,
             filter_offset,
+            is_real,
         })
     }
 }
 
 /// Alignment of a schedule element.
 ///
 /// The alignment of a schedule element is used to align the element within its
@@ -146,15 +175,15 @@
 ///
 /// - :attr:`Alignment.End`
 /// - :attr:`Alignment.Start`
 /// - :attr:`Alignment.Center`
 /// - :attr:`Alignment.Stretch`: Stretch the element to fill the parent.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
-enum Alignment {
+pub enum Alignment {
     End,
     Start,
     Center,
     Stretch,
 }
 
 #[pymethods]
@@ -172,15 +201,15 @@
     /// Args:
     ///     obj (str | Alignment): The value to convert.
     /// Returns:
     ///     Alignment: The converted value.
     /// Raises:
     ///     ValueError: If the value cannot be converted to Alignment.
     #[staticmethod]
-    fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
+    fn convert(obj: &Bound<PyAny>) -> PyResult<Py<Self>> {
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(s) = obj.extract() {
             let alignment = match s {
                 "end" => Some(Alignment::End),
                 "start" => Some(Alignment::Start),
@@ -196,15 +225,15 @@
             "Failed to convert the value to Alignment. ",
             "Must be Alignment or one of 'end', 'start', 'center', 'stretch'"
         );
         Err(PyValueError::new_err(msg))
     }
 }
 
-fn extract_alignment(obj: &Bound<'_, PyAny>) -> PyResult<Alignment> {
+fn extract_alignment(obj: &Bound<PyAny>) -> PyResult<Alignment> {
     Alignment::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// Base class for shapes.
 ///
 /// Shapes are used to define the envelope of a pulse. Internally, the shape is
 /// represented as a function :math:`f(t)` defined on the interval :math:`t \in
@@ -216,26 +245,25 @@
 /// - :class:`Hann`: Hann window.
 /// - :class:`Interp`: Interpolated shape.
 #[pyclass(subclass, frozen)]
 #[derive(Debug, Clone)]
 struct Shape;
 
 impl Shape {
-    fn get_rust_shape(slf: &Bound<'_, Shape>) -> PyResult<shape::Shape> {
+    fn get_rust_shape(slf: &Bound<Shape>) -> PyResult<shape::Shape> {
         if slf.downcast::<Hann>().is_ok() {
             return Ok(shape::Shape::new_hann());
         }
         if let Ok(interp) = slf.downcast::<Interp>() {
             let interp = interp.get();
-            return shape::Shape::new_interp(
+            return Ok(shape::Shape::new_interp(
                 interp.knots.clone(),
                 interp.controls.clone(),
                 interp.degree,
-            )
-            .map_err(|e| PyValueError::new_err(e.to_string()));
+            )?);
         }
         Err(PyTypeError::new_err("Invalid shape type."))
     }
 }
 
 /// A Hann shape.
 #[pyclass(extends=Shape, frozen)]
@@ -294,20 +322,23 @@
                 degree,
             },
             Shape,
         ))
     }
 }
 
-fn extract_margin(obj: &Bound<'_, PyAny>) -> PyResult<(f64, f64)> {
+fn extract_margin(obj: &Bound<PyAny>) -> PyResult<(Time, Time)> {
     if let Ok(v) = obj.extract() {
-        return Ok((v, v));
+        let t = Time::new(v)?;
+        return Ok((t, t));
     }
     if let Ok((v1, v2)) = obj.extract() {
-        return Ok((v1, v2));
+        let t1 = Time::new(v1)?;
+        let t2 = Time::new(v2)?;
+        return Ok((t1, t2));
     }
     let msg = "Failed to convert the value to (float, float).";
     Err(PyValueError::new_err(msg))
 }
 
 /// Base class for schedule elements.
 ///
@@ -381,74 +412,91 @@
 ///         add to waveforms. Defaults to ``False``.
 ///     duration (float): Duration of the element. Defaults to ``None``.
 ///     max_duration (float): Maximum duration of the element. Defaults to
 ///         ``inf``.
 ///     min_duration (float): Minimum duration of the element. Defaults to 0.
 #[pyclass(subclass, frozen)]
 #[derive(Debug, Clone)]
-struct Element(Arc<schedule::Element>);
+struct Element(ElementRef);
 
 #[pymethods]
 impl Element {
     #[getter]
-    fn margin(&self) -> (f64, f64) {
-        self.0.common().margin()
+    fn margin(&self) -> (Time, Time) {
+        self.0.common.margin()
     }
 
     #[getter]
     fn alignment(&self) -> Alignment {
-        self.0.common().alignment()
+        self.0.common.alignment()
     }
 
     #[getter]
     fn phantom(&self) -> bool {
-        self.0.common().phantom()
+        self.0.common.phantom()
     }
 
     #[getter]
-    fn duration(&self) -> Option<f64> {
-        self.0.common().duration()
+    fn duration(&self) -> Option<Time> {
+        self.0.common.duration()
     }
 
     #[getter]
-    fn max_duration(&self) -> f64 {
-        self.0.common().max_duration()
+    fn max_duration(&self) -> Time {
+        self.0.common.max_duration()
     }
 
     #[getter]
-    fn min_duration(&self) -> f64 {
-        self.0.common().min_duration()
+    fn min_duration(&self) -> Time {
+        self.0.common.min_duration()
     }
 }
 
-fn build_element(
-    variant: impl Into<schedule::ElementVariant>,
-    margin: Option<&Bound<'_, PyAny>>,
-    alignment: Option<&Bound<'_, PyAny>>,
-    phantom: bool,
-    duration: Option<f64>,
-    max_duration: f64,
-    min_duration: f64,
-) -> PyResult<Element> {
-    let mut builder = ElementCommonBuilder::new();
-    if let Some(obj) = margin {
-        builder.margin(extract_margin(obj)?);
+trait ElementSubclass: Sized + DerefToPyAny
+where
+    for<'a> &'a Self::Variant: TryFrom<&'a schedule::ElementVariant>,
+    for<'a> <&'a Self::Variant as TryFrom<&'a schedule::ElementVariant>>::Error: Debug,
+{
+    type Variant: Into<schedule::ElementVariant>;
+
+    fn variant<'a>(slf: &'a Bound<Self>) -> &'a Self::Variant {
+        slf.downcast::<Element>()
+            .expect("Self should be a subclass of Element")
+            .get()
+            .0
+            .variant
+            .borrow()
+            .try_into()
+            .expect("Element should have a valid variant")
     }
-    if let Some(obj) = alignment {
-        builder.alignment(extract_alignment(obj)?);
+
+    fn build_element(
+        variant: Self::Variant,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
+        phantom: bool,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
+    ) -> PyResult<Element> {
+        let mut builder = ElementCommonBuilder::new();
+        if let Some(obj) = margin {
+            builder.margin(extract_margin(obj)?);
+        }
+        if let Some(obj) = alignment {
+            builder.alignment(extract_alignment(obj)?);
+        }
+        builder
+            .phantom(phantom)
+            .duration(duration)
+            .max_duration(max_duration)
+            .min_duration(min_duration);
+        let common = builder.build()?;
+        Ok(Element(Arc::new(schedule::Element::new(common, variant))))
     }
-    builder
-        .phantom(phantom)
-        .duration(duration)
-        .max_duration(max_duration)
-        .min_duration(min_duration);
-    let common = builder
-        .build()
-        .map_err(|e| PyValueError::new_err(e.to_string()))?;
-    Ok(Element(Arc::new(schedule::Element::new(common, variant))))
 }
 
 /// A pulse play element.
 ///
 /// Given the pulse envelope :math:`E(t)`, channel total frequency :math:`f_c`,
 /// and channel phase :math:`\phi_c`, the the final pulse :math:`P(t)` starts at
 /// :math:`t_0` with sideband will be
@@ -488,206 +536,120 @@
 ///         0.
 ///     flexible (bool): Whether the pulse has flexible plateau length. Defaults
 ///         to ``False``.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct Play;
 
+impl ElementSubclass for Play {
+    type Variant = schedule::Play;
+}
+
 #[pymethods]
 impl Play {
     #[new]
     #[pyo3(signature = (
         channel_id,
         shape_id,
         amplitude,
         width,
         *,
-        plateau=0.0,
+        plateau=Time::ZERO,
         drag_coef=0.0,
-        frequency=0.0,
-        phase=0.0,
+        frequency=Frequency::ZERO,
+        phase=Phase::ZERO,
         flexible=false,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: String,
-        shape_id: Option<String>,
-        amplitude: f64,
-        width: f64,
-        plateau: f64,
+        channel_id: ChannelId,
+        shape_id: Option<ShapeId>,
+        amplitude: Amplitude,
+        width: Time,
+        plateau: Time,
         drag_coef: f64,
-        frequency: f64,
-        phase: f64,
+        frequency: Frequency,
+        phase: Phase,
         flexible: bool,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
-        let variant = schedule::Play::new(channel_id, shape_id, amplitude, width)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
-        let variant = variant
-            .with_plateau(plateau)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
-        let variant = variant
-            .with_drag_coef(drag_coef)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
-        let variant = variant
-            .with_frequency(frequency)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
-        let variant = variant
-            .with_phase(phase)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
-        let variant = variant.with_flexible(flexible);
+        let variant = schedule::Play::new(channel_id, shape_id, amplitude, width)?
+            .with_plateau(plateau)?
+            .with_drag_coef(drag_coef)?
+            .with_frequency(frequency)?
+            .with_phase(phase)?
+            .with_flexible(flexible);
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .channel_id();
-        Ok(ret.to_string())
+    fn channel_id<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id()
     }
 
     #[getter]
-    fn shape_id(slf: &Bound<'_, Self>) -> PyResult<Option<String>> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .shape_id();
-        Ok(ret.map(|x| x.to_string()))
+    fn shape_id<'a>(slf: &'a Bound<Self>) -> Option<&'a ShapeId> {
+        Self::variant(slf).shape_id()
     }
 
     #[getter]
-    fn amplitude(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .amplitude();
-        Ok(ret)
+    fn amplitude(slf: &Bound<Self>) -> Amplitude {
+        Self::variant(slf).amplitude()
     }
 
     #[getter]
-    fn width(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .width();
-        Ok(ret)
+    fn width(slf: &Bound<Self>) -> Time {
+        Self::variant(slf).width()
     }
 
     #[getter]
-    fn plateau(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .plateau();
-        Ok(ret)
+    fn plateau(slf: &Bound<Self>) -> Time {
+        Self::variant(slf).plateau()
     }
 
     #[getter]
-    fn drag_coef(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .drag_coef();
-        Ok(ret)
+    fn drag_coef(slf: &Bound<Self>) -> f64 {
+        Self::variant(slf).drag_coef()
     }
 
     #[getter]
-    fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .frequency();
-        Ok(ret)
+    fn frequency(slf: &Bound<Self>) -> Frequency {
+        Self::variant(slf).frequency()
     }
 
     #[getter]
-    fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .phase();
-        Ok(ret)
+    fn phase(slf: &Bound<Self>) -> Phase {
+        Self::variant(slf).phase()
     }
 
     #[getter]
-    fn flexible(slf: &Bound<'_, Self>) -> PyResult<bool> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_play()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the play variant from the element.",
-            ))?
-            .flexible();
-        Ok(ret)
+    fn flexible(slf: &Bound<Self>) -> bool {
+        Self::variant(slf).flexible()
     }
 }
 
 /// A phase shift element.
 ///
 /// Phase shift will be added to the channel phase offset :math:`\phi_c` and is
 /// time-independent.
@@ -700,81 +662,66 @@
 /// Args:
 ///     channel_id (str): Target channel ID.
 ///     phase (float): Phase shift in **cycles**.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct ShiftPhase;
 
+impl ElementSubclass for ShiftPhase {
+    type Variant = schedule::ShiftPhase;
+}
+
 #[pymethods]
 impl ShiftPhase {
     #[new]
     #[pyo3(signature = (
         channel_id,
         phase,
         *,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: String,
-        phase: f64,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        channel_id: ChannelId,
+        phase: Phase,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
-        let variant = schedule::ShiftPhase::new(channel_id, phase)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
+        let variant = schedule::ShiftPhase::new(channel_id, phase)?;
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_shift_phase()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the shift_phase variant from the element.",
-            ))?
-            .channel_id();
-        Ok(ret.to_string())
+    fn channel_id<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id()
     }
 
     #[getter]
-    fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_shift_phase()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the shift_phase variant from the element.",
-            ))?
-            .phase();
-        Ok(ret)
+    fn phase(slf: &Bound<Self>) -> Phase {
+        Self::variant(slf).phase()
     }
 }
 
 /// A phase set element.
 ///
 /// Waveform generator treats the base frequency :math:`f_0` and the channel
 /// frequency shift :math:`\Delta f` differently. :math:`f_0` is never changed
@@ -795,81 +742,66 @@
 /// Args:
 ///     channel_id (str): Target channel ID.
 ///     phase (float): Target phase value in **cycles**.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SetPhase;
 
+impl ElementSubclass for SetPhase {
+    type Variant = schedule::SetPhase;
+}
+
 #[pymethods]
 impl SetPhase {
     #[new]
     #[pyo3(signature = (
         channel_id,
         phase,
         *,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: String,
-        phase: f64,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        channel_id: ChannelId,
+        phase: Phase,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
-        let variant = schedule::SetPhase::new(channel_id, phase)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
+        let variant = schedule::SetPhase::new(channel_id, phase)?;
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_set_phase()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the set_phase variant from the element.",
-            ))?
-            .channel_id();
-        Ok(ret.to_string())
+    fn channel_id<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id()
     }
 
     #[getter]
-    fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_set_phase()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the set_phase variant from the element.",
-            ))?
-            .phase();
-        Ok(ret)
+    fn phase(slf: &Bound<Self>) -> Phase {
+        Self::variant(slf).phase()
     }
 }
 
 /// A frequency shift element.
 ///
 /// Frequency shift will be added to the channel frequency shift :math:`\Delta
 /// f` and the channel phase offset :math:`\phi_c` will be adjusted such that
@@ -878,81 +810,66 @@
 /// Args:
 ///     channel_id (str): Target channel ID.
 ///     frequency (float): Delta frequency.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct ShiftFreq;
 
+impl ElementSubclass for ShiftFreq {
+    type Variant = schedule::ShiftFreq;
+}
+
 #[pymethods]
 impl ShiftFreq {
     #[new]
     #[pyo3(signature = (
         channel_id,
         frequency,
         *,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: String,
-        frequency: f64,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        channel_id: ChannelId,
+        frequency: Frequency,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
-        let variant = schedule::ShiftFreq::new(channel_id, frequency)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
+        let variant = schedule::ShiftFreq::new(channel_id, frequency)?;
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_shift_freq()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the shift_freq variant from the element.",
-            ))?
-            .channel_id();
-        Ok(ret.to_string())
+    fn channel_id<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id()
     }
 
     #[getter]
-    fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_shift_freq()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the shift_freq variant from the element.",
-            ))?
-            .frequency();
-        Ok(ret)
+    fn frequency(slf: &Bound<Self>) -> Frequency {
+        Self::variant(slf).frequency()
     }
 }
 
 /// A frequency set element.
 ///
 /// The channel frequency shift :math:`\Delta f` will be set to the provided
 /// `frequency` parameter and the channel phase offset :math:`\phi_c` will be
@@ -962,81 +879,66 @@
 /// Args:
 ///     channel_id (str): Target channel ID.
 ///     frequency (float): Target frequency.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SetFreq;
 
+impl ElementSubclass for SetFreq {
+    type Variant = schedule::SetFreq;
+}
+
 #[pymethods]
 impl SetFreq {
     #[new]
     #[pyo3(signature = (
         channel_id,
         frequency,
         *,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: String,
-        frequency: f64,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        channel_id: ChannelId,
+        frequency: Frequency,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
-        let variant = schedule::SetFreq::new(channel_id, frequency)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
+        let variant = schedule::SetFreq::new(channel_id, frequency)?;
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_set_freq()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the set_freq variant from the element.",
-            ))?
-            .channel_id();
-        Ok(ret.to_string())
+    fn channel_id<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id()
     }
 
     #[getter]
-    fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_set_freq()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the set_freq variant from the element.",
-            ))?
-            .frequency();
-        Ok(ret)
+    fn frequency(slf: &Bound<Self>) -> Frequency {
+        Self::variant(slf).frequency()
     }
 }
 
 /// A phase swap element.
 ///
 /// Different from :class:`SetPhase` and :class:`SetFreq`, both the channel
 /// base frequency :math:`f_0` and the channel frequency shift :math:`\Delta f`
@@ -1048,80 +950,66 @@
 /// Args:
 ///     channel_id1 (str): Target channel ID 1.
 ///     channel_id2 (str): Target channel ID 2.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SwapPhase;
 
+impl ElementSubclass for SwapPhase {
+    type Variant = schedule::SwapPhase;
+}
+
 #[pymethods]
 impl SwapPhase {
     #[new]
     #[pyo3(signature = (
         channel_id1,
         channel_id2,
         *,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id1: String,
-        channel_id2: String,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        channel_id1: ChannelId,
+        channel_id2: ChannelId,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
         let variant = schedule::SwapPhase::new(channel_id1, channel_id2);
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id1(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_swap_phase()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the swap_phase variant from the element.",
-            ))?
-            .channel_id1();
-        Ok(ret.to_string())
+    fn channel_id1<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id1()
     }
 
     #[getter]
-    fn channel_id2(slf: &Bound<'_, Self>) -> PyResult<String> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_swap_phase()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the swap_phase variant from the element.",
-            ))?
-            .channel_id2();
-        Ok(ret.to_string())
+    fn channel_id2<'a>(slf: &'a Bound<Self>) -> &'a ChannelId {
+        Self::variant(slf).channel_id2()
     }
 }
 
 /// A barrier element.
 ///
 /// A barrier element is a no-op element. Useful for aligning elements on
 /// different channels and adding space between elements in a :class:`Stack`
@@ -1132,63 +1020,57 @@
 ///
 /// Args:
 ///     *channel_ids (str): Channel IDs. Defaults to empty.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct Barrier;
 
+impl ElementSubclass for Barrier {
+    type Variant = schedule::Barrier;
+}
+
 #[pymethods]
 impl Barrier {
     #[new]
     #[pyo3(signature = (
         *channel_ids,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     fn new(
-        channel_ids: Vec<String>,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        channel_ids: Vec<ChannelId>,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
         let variant = schedule::Barrier::new(channel_ids);
         Ok((
             Self,
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_ids(slf: &Bound<'_, Self>) -> PyResult<Vec<String>> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_barrier()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the barrier variant from the element.",
-            ))?
-            .channel_ids()
-            .to_vec();
-        Ok(ret)
+    fn channel_ids(slf: &Bound<Self>) -> Vec<ChannelId> {
+        Self::variant(slf).channel_ids().to_vec()
     }
 }
 
 /// A repeat element.
 ///
 /// Repeat the child element multiple times with a spacing between repetitions.
 ///
@@ -1198,85 +1080,69 @@
 ///     spacing (float): Spacing between repetitions. Defaults to 0.
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Repeat {
     child: Py<Element>,
 }
 
+impl ElementSubclass for Repeat {
+    type Variant = schedule::Repeat;
+}
+
 #[pymethods]
 impl Repeat {
     #[new]
     #[pyo3(signature = (
         child,
         count,
-        spacing=0.0,
+        spacing=Time::ZERO,
         *,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         child: Py<Element>,
         count: usize,
-        spacing: f64,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        spacing: Time,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
         let rust_child = child.get().0.clone();
-        let variant = schedule::Repeat::new(rust_child, count)
-            .with_spacing(spacing)
-            .map_err(|e| PyValueError::new_err(e.to_string()))?;
+        let variant = schedule::Repeat::new(rust_child, count).with_spacing(spacing)?;
         Ok((
             Self { child },
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn count(slf: &Bound<'_, Self>) -> PyResult<usize> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_repeat()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the repeat variant from the element.",
-            ))?
-            .count();
-        Ok(ret)
+    fn count(slf: &Bound<Self>) -> usize {
+        Self::variant(slf).count()
     }
 
     #[getter]
-    fn spacing(slf: &Bound<'_, Self>) -> PyResult<f64> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_repeat()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the repeat variant from the element.",
-            ))?
-            .spacing();
-        Ok(ret)
+    fn spacing(slf: &Bound<Self>) -> Time {
+        Self::variant(slf).spacing()
     }
 }
 
 /// Layout order in a stack layout.
 ///
 /// A stack layout has two possible children processing orders:
 ///
@@ -1285,15 +1151,15 @@
 ///     This is the default order.
 ///
 /// - :attr:`Direction.Forward`:
 ///     Process children in original order and schedule them as early as
 ///     possible.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
-enum Direction {
+pub enum Direction {
     Backward,
     Forward,
 }
 
 #[pymethods]
 impl Direction {
     /// Convert the value to Direction.
@@ -1306,15 +1172,15 @@
     /// Args:
     ///     obj (str | Direction): Value to convert.
     /// Returns:
     ///     Direction: Converted value.
     /// Raises:
     ///     ValueError: If the value cannot be converted.
     #[staticmethod]
-    fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
+    fn convert(obj: &Bound<PyAny>) -> PyResult<Py<Self>> {
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(s) = obj.extract() {
             let direction = match s {
                 "backward" => Some(Direction::Backward),
                 "forward" => Some(Direction::Forward),
@@ -1328,15 +1194,15 @@
             "Failed to convert the value to Direction. ",
             "Must be Direction or one of 'backward', 'forward'"
         );
         Err(PyValueError::new_err(msg))
     }
 }
 
-fn extract_direction(obj: &Bound<'_, PyAny>) -> PyResult<Direction> {
+fn extract_direction(obj: &Bound<PyAny>) -> PyResult<Direction> {
     Direction::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// A stack layout element.
 ///
 /// Each child element occupies some channels and has a duration. Stack layout
 /// will put children as close as possible without changing the order of
@@ -1349,48 +1215,52 @@
 ///     direction (str | Direction): Layout order. Defaults to 'backward'.
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Stack {
     children: Vec<Py<Element>>,
 }
 
+impl ElementSubclass for Stack {
+    type Variant = schedule::Stack;
+}
+
 #[pymethods]
 impl Stack {
     #[new]
     #[pyo3(signature = (
         *children,
         direction=None,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         children: Vec<Py<Element>>,
-        direction: Option<&Bound<'_, PyAny>>,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        direction: Option<&Bound<PyAny>>,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
         let rust_children = children.iter().map(|x| x.get().0.clone()).collect();
         let variant = schedule::Stack::new().with_children(rust_children);
         let variant = if let Some(obj) = direction {
             variant.with_direction(extract_direction(obj)?)
         } else {
             variant
         };
         Ok((
             Self { children },
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
@@ -1411,70 +1281,55 @@
     ///     )
     ///
     /// Args:
     ///     *children (Element): New child elements.
     /// Returns:
     ///     Stack: New stack layout.
     #[pyo3(signature=(*children))]
-    fn with_children(slf: &Bound<'_, Self>, children: Vec<Py<Element>>) -> PyResult<Py<Self>> {
+    fn with_children(slf: &Bound<Self>, children: Vec<Py<Element>>) -> PyResult<Py<Self>> {
         let py = slf.py();
         let rust_children = children.iter().map(|x| x.get().0.clone()).collect();
         let rust_base = &slf.downcast::<Element>()?.get().0;
-        let common = rust_base.common().clone();
-        let variant = rust_base
-            .try_get_stack()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the stack variant from the element.",
-            ))?
-            .clone()
-            .with_children(rust_children);
+        let common = rust_base.common.clone();
+        let variant = Self::variant(slf).clone().with_children(rust_children);
         Py::new(
             py,
             (
                 Self { children },
                 Element(Arc::new(schedule::Element::new(common, variant))),
             ),
         )
     }
 
     #[getter]
-    fn direction(slf: &Bound<'_, Self>) -> PyResult<Direction> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_stack()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the stack variant from the element.",
-            ))?
-            .direction();
-        Ok(ret)
+    fn direction(slf: &Bound<Self>) -> Direction {
+        Self::variant(slf).direction()
     }
 }
 
 /// A child element with an absolute time in a absolute layout.
 ///
 /// The time of each child element is relative to the start of the absolute
 /// layout.
 ///
 /// Args:
 ///     time (float): Time relative to the start of the parent element.
 ///     element (Element): Child element.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct AbsoluteEntry {
-    time: f64,
+    time: Time,
     element: Py<Element>,
 }
 
 #[pymethods]
 impl AbsoluteEntry {
     #[new]
-    fn new(time: f64, element: Py<Element>) -> PyResult<Self> {
-        if !time.is_finite() {
+    fn new(time: Time, element: Py<Element>) -> PyResult<Self> {
+        if !time.value().is_finite() {
             return Err(PyValueError::new_err("Time must be finite"));
         }
         Ok(AbsoluteEntry { time, element })
     }
 
     /// Convert the value to AbsoluteEntry.
     ///
@@ -1487,32 +1342,32 @@
     /// Args:
     ///     obj (AbsoluteEntry | Element | tuple[float, Element]): Value to convert.
     /// Returns:
     ///     AbsoluteEntry: Converted value.
     /// Raises:
     ///     ValueError: If the value cannot be converted.
     #[staticmethod]
-    fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
+    fn convert(obj: &Bound<PyAny>) -> PyResult<Py<Self>> {
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(element) = obj.extract() {
-            return Py::new(py, AbsoluteEntry::new(0.0, element)?);
+            return Py::new(py, AbsoluteEntry::new(Time::ZERO, element)?);
         }
         if let Ok((time, element)) = obj.extract() {
             return Py::new(py, AbsoluteEntry::new(time, element)?);
         }
         Err(PyValueError::new_err(
             "Failed to convert the value to AbsoluteEntry",
         ))
     }
 }
 
-fn extract_absolute_entry(obj: &Bound<'_, PyAny>) -> PyResult<AbsoluteEntry> {
+fn extract_absolute_entry(obj: &Bound<PyAny>) -> PyResult<AbsoluteEntry> {
     AbsoluteEntry::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// An absolute layout element.
 ///
 /// The child elements are arranged in absolute time. The time of each child
 /// element is relative to the start of the absolute schedule. The duration of
@@ -1536,54 +1391,56 @@
 ///         )
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Absolute {
     children: Vec<AbsoluteEntry>,
 }
 
+impl ElementSubclass for Absolute {
+    type Variant = schedule::Absolute;
+}
+
 #[pymethods]
 impl Absolute {
     #[new]
     #[pyo3(signature = (
         *children,
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        py: Python<'_>,
+        py: Python,
         children: Vec<Py<PyAny>>,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
         let children: Vec<AbsoluteEntry> = children
             .into_iter()
             .map(|x| extract_absolute_entry(&x.into_bound(py)))
             .collect::<PyResult<_>>()?;
         let rust_children = children
             .iter()
             .map(|x| {
                 let element = x.element.get().0.clone();
-                schedule::AbsoluteEntry::new(element)
-                    .with_time(x.time)
-                    .map_err(|e| PyValueError::new_err(e.to_string()))
+                Ok(schedule::AbsoluteEntry::new(element).with_time(x.time)?)
             })
             .collect::<PyResult<_>>()?;
         let variant = schedule::Absolute::new().with_children(rust_children);
         Ok((
             Self { children },
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
@@ -1605,38 +1462,30 @@
     ///
     /// Args:
     ///     *children (AbsoluteEntry | Element | tuple[float, Element]): New
     ///         child elements.
     /// Returns:
     ///     Absolute: New absolute schedule.
     #[pyo3(signature=(*children))]
-    fn with_children(slf: &Bound<'_, Self>, children: Vec<Py<PyAny>>) -> PyResult<Py<Self>> {
+    fn with_children(slf: &Bound<Self>, children: Vec<Py<PyAny>>) -> PyResult<Py<Self>> {
         let py = slf.py();
         let children: Vec<_> = children
             .into_iter()
             .map(|x| extract_absolute_entry(&x.into_bound(py)))
             .collect::<PyResult<_>>()?;
         let rust_children = children
             .iter()
             .map(|x| {
                 let element = x.element.get().0.clone();
-                schedule::AbsoluteEntry::new(element)
-                    .with_time(x.time)
-                    .map_err(|e| PyValueError::new_err(e.to_string()))
+                Ok(schedule::AbsoluteEntry::new(element).with_time(x.time)?)
             })
             .collect::<PyResult<_>>()?;
         let rust_base = &slf.downcast::<Element>()?.get().0;
-        let common = rust_base.common().clone();
-        let variant = rust_base
-            .try_get_absolute()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the absolute variant from the element.",
-            ))?
-            .clone()
-            .with_children(rust_children);
+        let common = rust_base.common.clone();
+        let variant = Self::variant(slf).clone().with_children(rust_children);
         Py::new(
             py,
             (
                 Self { children },
                 Element(Arc::new(schedule::Element::new(common, variant))),
             ),
         )
@@ -1661,15 +1510,15 @@
 /// Length of a grid column.
 ///
 /// :class:`GridLength` is used to specify the length of a grid column. The
 /// length can be specified in seconds, as a fraction of the remaining duration,
 /// or automatically.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
-struct GridLength {
+pub struct GridLength {
     value: f64,
     unit: GridLengthUnit,
 }
 
 #[pymethods]
 impl GridLength {
     /// Create an automatic grid length.
@@ -1734,15 +1583,15 @@
     /// Args:
     ///     obj (GridLength | float | str): Value to convert.
     /// Returns:
     ///     GridLength: Converted value.
     /// Raises:
     ///     ValueError: If the value cannot be converted.
     #[staticmethod]
-    fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
+    fn convert(obj: &Bound<PyAny>) -> PyResult<Py<Self>> {
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(v) = obj.extract() {
             return Py::new(py, GridLength::fixed(v)?);
         }
@@ -1762,15 +1611,15 @@
         }
         Err(PyValueError::new_err(
             "Failed to convert the value to GridLength.",
         ))
     }
 }
 
-fn extract_grid_length(obj: &Bound<'_, PyAny>) -> PyResult<GridLength> {
+fn extract_grid_length(obj: &Bound<PyAny>) -> PyResult<GridLength> {
     GridLength::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// A child element in a grid layout.
 ///
 /// Args:
 ///     element (Element): Child element.
@@ -1811,15 +1660,15 @@
     /// Args:
     ///     obj (GridEntry | Element | tuple[Element, int] | tuple[Element, int, int]): Value to convert.
     /// Returns:
     ///     GridEntry: Converted value.
     /// Raises:
     ///     ValueError: If the value cannot be converted.
     #[staticmethod]
-    fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
+    fn convert(obj: &Bound<PyAny>) -> PyResult<Py<Self>> {
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(element) = obj.extract() {
             return Py::new(py, GridEntry::new(element, 0, 1)?);
         }
@@ -1831,15 +1680,15 @@
         }
         Err(PyValueError::new_err(
             "Failed to convert the value to GridEntry.",
         ))
     }
 }
 
-fn extract_grid_entry(obj: &Bound<'_, PyAny>) -> PyResult<GridEntry> {
+fn extract_grid_entry(obj: &Bound<PyAny>) -> PyResult<GridEntry> {
     GridEntry::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// A grid layout element.
 ///
 /// A grid layout has multiple columns and each child element occupies some
 /// columns. The width of each column can be specified by :class:`GridLength`,
@@ -1885,38 +1734,42 @@
 ///         )
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Grid {
     children: Vec<GridEntry>,
 }
 
+impl ElementSubclass for Grid {
+    type Variant = schedule::Grid;
+}
+
 #[pymethods]
 impl Grid {
     #[new]
     #[pyo3(signature = (
         *children,
         columns=vec![],
         margin=None,
         alignment=None,
         phantom=false,
         duration=None,
-        max_duration=f64::INFINITY,
-        min_duration=0.0,
+        max_duration=Time::INFINITY,
+        min_duration=Time::ZERO,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        py: Python<'_>,
+        py: Python,
         children: Vec<Py<PyAny>>,
         columns: Vec<Py<PyAny>>,
-        margin: Option<&Bound<'_, PyAny>>,
-        alignment: Option<&Bound<'_, PyAny>>,
+        margin: Option<&Bound<PyAny>>,
+        alignment: Option<&Bound<PyAny>>,
         phantom: bool,
-        duration: Option<f64>,
-        max_duration: f64,
-        min_duration: f64,
+        duration: Option<Time>,
+        max_duration: Time,
+        min_duration: Time,
     ) -> PyResult<(Self, Element)> {
         let children: Vec<_> = children
             .into_iter()
             .map(|x| extract_grid_entry(&x.into_bound(py)))
             .collect::<PyResult<_>>()?;
         let columns: Vec<_> = columns
             .into_iter()
@@ -1932,15 +1785,15 @@
             })
             .collect();
         let variant = schedule::Grid::new()
             .with_children(rust_children)
             .with_columns(columns);
         Ok((
             Self { children },
-            build_element(
+            Self::build_element(
                 variant,
                 margin,
                 alignment,
                 phantom,
                 duration,
                 max_duration,
                 min_duration,
@@ -1962,15 +1815,15 @@
     ///     )
     ///
     /// Args:
     ///     *children (GridEntry | Element | tuple[Element, int] | tuple[Element, int, int]): New child elements.
     /// Returns:
     ///     Grid: New grid schedule.
     #[pyo3(signature=(*children))]
-    fn with_children(slf: &Bound<'_, Self>, children: Vec<Py<PyAny>>) -> PyResult<Py<Self>> {
+    fn with_children(slf: &Bound<Self>, children: Vec<Py<PyAny>>) -> PyResult<Py<Self>> {
         let py = slf.py();
         let children: Vec<_> = children
             .into_iter()
             .map(|x| extract_grid_entry(&x.into_bound(py)))
             .collect::<PyResult<_>>()?;
         let rust_children = children
             .iter()
@@ -1978,63 +1831,52 @@
                 let element = x.element.get().0.clone();
                 schedule::GridEntry::new(element)
                     .with_column(x.column)
                     .with_span(x.span)
             })
             .collect();
         let rust_base = &slf.downcast::<Element>()?.get().0;
-        let common = rust_base.common().clone();
-        let variant = rust_base
-            .try_get_grid()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the grid variant from the element.",
-            ))?
-            .clone()
-            .with_children(rust_children);
+        let common = rust_base.common.clone();
+        let variant = Self::variant(slf).clone().with_children(rust_children);
         Py::new(
             py,
             (
                 Self { children },
                 Element(Arc::new(schedule::Element::new(common, variant))),
             ),
         )
     }
 
     #[getter]
-    fn columns(slf: &Bound<'_, Self>) -> PyResult<Vec<GridLength>> {
-        let ret = slf
-            .downcast::<Element>()?
-            .get()
-            .0
-            .try_get_grid()
-            .ok_or(PyValueError::new_err(
-                "Failed to get the grid variant from the element.",
-            ))?
-            .columns()
-            .to_vec();
-        Ok(ret)
+    fn columns(slf: &Bound<Self>) -> Vec<GridLength> {
+        Self::variant(slf).columns().to_vec()
     }
 }
 
 /// Generate waveforms from a schedule.
 ///
+/// .. caution::
+///
+///     Crosstalk matrix will not be applied to offset of the channels.
+///
 /// Args:
 ///     channels (Mapping[str, Channel]): Information of the channels.
 ///     shapes (Mapping[str, Shape]): Shapes used in the schedule.
 ///     schedule (Element): Root element of the schedule.
 ///     time_tolerance (float): Tolerance for time comparison. Default is 1e-12.
 ///     amp_tolerance (float): Tolerance for amplitude comparison. Default is
 ///         0.1 / 2^16.
 ///     allow_oversize (bool): Allow oversize elements. Default is ``False``.
 ///     crosstalk (tuple[array_like, Sequence[str]] | None): Crosstalk matrix
 ///         with corresponding channel ids. Default is ``None``.
 /// Returns:
 ///     Dict[str, numpy.ndarray]: Waveforms of the channels. The key is the
 ///         channel name and the value is the waveform. The shape of the
-///         waveform is ``(2, length)``.
+///         waveform is ``(n, length)``, where ``n`` is 2 for complex waveform
+///         and 1 for real waveform.
 /// Raises:
 ///     ValueError: If some input is invalid.
 ///     TypeError: If some input has an invalid type.
 ///     RuntimeError: If waveform generation fails.
 /// Example:
 ///     .. code-block:: python
 ///
@@ -2054,115 +1896,161 @@
 ///         result = generate_waveforms(channels, shapes, schedule)
 #[pyfunction]
 #[pyo3(signature = (
     channels,
     shapes,
     schedule,
     *,
-    time_tolerance=1e-12,
-    amp_tolerance=0.1 / 2f64.powi(16),
+    time_tolerance=Time::new(1e-12).unwrap(),
+    amp_tolerance=Amplitude::new(0.1 / 2f64.powi(16)).unwrap(),
     allow_oversize=false,
     crosstalk=None,
 ))]
 #[allow(clippy::too_many_arguments)]
 fn generate_waveforms(
-    py: Python<'_>,
-    channels: HashMap<String, Channel>,
-    shapes: HashMap<String, Py<Shape>>,
-    schedule: &Bound<'_, Element>,
-    time_tolerance: f64,
-    amp_tolerance: f64,
+    py: Python,
+    channels: HashMap<ChannelId, Channel>,
+    shapes: HashMap<ShapeId, Py<Shape>>,
+    schedule: Bound<Element>,
+    time_tolerance: Time,
+    amp_tolerance: Amplitude,
     allow_oversize: bool,
-    crosstalk: Option<(PyArrayLike2<'_, f64, AllowTypeChange>, Vec<String>)>,
-) -> PyResult<HashMap<String, Py<PyArray2<f64>>>> {
+    crosstalk: Option<(PyArrayLike2<f64, AllowTypeChange>, Vec<ChannelId>)>,
+) -> PyResult<HashMap<ChannelId, Py<PyArray2<f64>>>> {
     if let Some((crosstalk, names)) = &crosstalk {
         let nl = names.len();
         if crosstalk.shape() != [nl, nl] {
             return Err(PyValueError::new_err(
                 "The size of the crosstalk matrix must be the same as the number of names.",
             ));
         }
     }
-    let root = schedule.downcast::<Element>()?.get().0.clone();
-    let measured = schedule::measure(root, f64::INFINITY);
+    let pulse_lists = build_pulse_lists(
+        py,
+        schedule,
+        &channels,
+        &shapes,
+        time_tolerance,
+        amp_tolerance,
+        allow_oversize,
+    )?;
+    let waveforms = sample_waveform(py, &channels, pulse_lists, crosstalk, time_tolerance);
+    py.allow_threads(|| {
+        waveforms
+            .into_par_iter()
+            .map(|(n, w)| {
+                Python::with_gil(|py| {
+                    let mut w = w.into_bound(py);
+                    let c = &channels[&n];
+                    post_process(py, &mut w, c)?;
+                    Ok((n, w.unbind()))
+                })
+            })
+            .collect::<PyResult<_>>()
+    })
+}
+
+fn build_pulse_lists(
+    py: Python,
+    schedule: Bound<Element>,
+    channels: &HashMap<ChannelId, Channel>,
+    shapes: &HashMap<ShapeId, Py<Shape>>,
+    time_tolerance: Time,
+    amp_tolerance: Amplitude,
+    allow_oversize: bool,
+) -> PyResult<HashMap<ChannelId, PulseList>> {
+    let root = schedule.get().0.clone();
+    let measured = schedule::measure(root, Time::INFINITY);
     let arrange_options = schedule::ScheduleOptions {
         time_tolerance,
         allow_oversize,
     };
-    let arranged = schedule::arrange(&measured, 0.0, measured.duration(), &arrange_options)
-        .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
+    let arranged = schedule::arrange(&measured, Time::ZERO, measured.duration(), &arrange_options)?;
     let mut executor = Executor::new(amp_tolerance, time_tolerance);
-    for (n, c) in &channels {
+    for (n, c) in channels {
         executor.add_channel(n.clone(), c.base_freq);
     }
-    for (n, s) in &shapes {
+    for (n, s) in shapes {
         let s = s.bind(py);
         executor.add_shape(n.clone(), Shape::get_rust_shape(s)?);
     }
     executor.execute(&arranged);
-    let results = executor.into_result();
-    let waveforms: HashMap<String, Bound<PyArray2<f64>>> = channels
+    Ok(executor.into_result())
+}
+
+fn sample_waveform(
+    py: Python,
+    channels: &HashMap<ChannelId, Channel>,
+    pulse_lists: HashMap<ChannelId, PulseList>,
+    crosstalk: Option<(PyArrayLike2<f64, AllowTypeChange>, Vec<ChannelId>)>,
+    time_tolerance: Time,
+) -> HashMap<ChannelId, Py<PyArray2<f64>>> {
+    let waveforms: HashMap<_, _> = channels
         .iter()
-        .map(|(n, c)| (n.clone(), PyArray2::zeros_bound(py, (2, c.length), false)))
-        .collect();
-    {
-        let mut sampler = Sampler::new(results);
-        for (n, c) in &channels {
-            // SAFETY: These arrays are just created.
-            let array = unsafe { waveforms[n].as_array_mut() };
-            sampler.add_channel(
+        .map(|(n, c)| {
+            let n_w = if c.is_real { 1 } else { 2 };
+            (
                 n.clone(),
-                array,
-                Frequency::new(c.sample_rate).unwrap(),
-                Time::new(c.delay).unwrap(),
-                c.align_level,
-            );
-        }
-        if let Some((crosstalk, names)) = &crosstalk {
-            sampler.set_crosstalk(crosstalk.as_array(), names.clone());
-        }
-        sampler.sample(time_tolerance);
-    }
-    let waveforms = waveforms
-        .into_iter()
-        .map(|(n, mut w)| {
-            let c = &channels[&n];
-            if let Some(iq_matrix) = &c.iq_matrix {
-                w = dot_bound(iq_matrix.bind(py), &w)?;
-            }
-            if c.filter_offset {
-                apply_offset(py, &w, c.iq_offset)?;
-                if let Some(iir) = &c.iir {
-                    apply_iir(py, &w, iir.bind(py))?;
-                }
-                if let Some(fir) = &c.fir {
-                    apply_fir(py, &w, fir.bind(py))?;
-                }
-            } else {
-                if let Some(iir) = &c.iir {
-                    apply_iir(py, &w, iir.bind(py))?;
-                }
-                if let Some(fir) = &c.fir {
-                    apply_fir(py, &w, fir.bind(py))?;
-                }
-                apply_offset(py, &w, c.iq_offset)?;
-            }
-            Ok((n, w.unbind()))
+                PyArray2::zeros_bound(py, (n_w, c.length), false).unbind(),
+            )
         })
-        .collect::<PyResult<_>>()?;
-    Ok(waveforms)
+        .collect();
+    let mut sampler = Sampler::new(pulse_lists);
+    for (n, c) in channels {
+        // SAFETY: These arrays are just created.
+        let array = unsafe { waveforms[n].bind(py).as_array_mut() };
+        sampler.add_channel(n.clone(), array, c.sample_rate, c.delay, c.align_level);
+    }
+    if let Some((crosstalk, names)) = &crosstalk {
+        sampler.set_crosstalk(crosstalk.as_array(), names.clone());
+    }
+    sampler.sample(time_tolerance);
+    waveforms
 }
 
-fn apply_offset(py: Python<'_>, w: &Bound<'_, PyArray2<f64>>, offset: (f64, f64)) -> PyResult<()> {
-    if offset.0 == 0.0 && offset.1 == 0.0 {
-        return Ok(());
+fn post_process<'py>(
+    py: Python<'py>,
+    w: &mut Bound<'py, PyArray2<f64>>,
+    c: &Channel,
+) -> PyResult<()> {
+    if let Some(iq_matrix) = &c.iq_matrix {
+        *w = dot_bound(iq_matrix.bind(py), w)?;
     }
+    if c.filter_offset {
+        if let Some(offset) = &c.offset {
+            apply_offset(py, w, offset.bind(py))?;
+        }
+        if let Some(iir) = &c.iir {
+            apply_iir(py, w, iir.bind(py))?;
+        }
+        if let Some(fir) = &c.fir {
+            apply_fir(py, w, fir.bind(py))?;
+        }
+    } else {
+        if let Some(iir) = &c.iir {
+            apply_iir(py, w, iir.bind(py))?;
+        }
+        if let Some(fir) = &c.fir {
+            apply_fir(py, w, fir.bind(py))?;
+        }
+        if let Some(offset) = &c.offset {
+            apply_offset(py, w, offset.bind(py))?;
+        }
+    }
+    Ok(())
+}
+
+fn apply_offset(
+    py: Python,
+    w: &Bound<PyArray2<f64>>,
+    offset: &Bound<PyArray1<f64>>,
+) -> PyResult<()> {
     let locals = PyDict::new_bound(py);
     locals.set_item("w", w)?;
-    locals.set_item("offset", pyarray_bound![py, offset.0, offset.1])?;
+    locals.set_item("offset", offset)?;
     py.run_bound(
         indoc! {"
             import numpy as np
             w += offset[:, np.newaxis]
         "},
         None,
         Some(&locals),
@@ -2213,15 +2101,15 @@
 /// experiments.
 ///
 /// .. caution::
 ///
 ///     The unit of phase is number of cycles, not radians. For example, a phase
 ///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
 #[pymodule]
-fn bosing(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
+fn bosing(_py: Python, m: &Bound<PyModule>) -> PyResult<()> {
     m.add_class::<Absolute>()?;
     m.add_class::<AbsoluteEntry>()?;
     m.add_class::<Alignment>()?;
     m.add_class::<Barrier>()?;
     m.add_class::<Channel>()?;
     m.add_class::<Direction>()?;
     m.add_class::<Element>()?;
```

### Comparing `bosing-2.0.0b9/src/pulse.rs` & `bosing-2.0.1/src/pulse.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 use std::{
-    f64::consts::TAU,
     ops::{Add, Mul},
     sync::Arc,
 };
 
 use cached::proc_macro::cached;
 use float_cmp::approx_eq;
 use hashbrown::HashMap;
 use itertools::{izip, Itertools};
 use ndarray::{s, ArrayView2, ArrayViewMut2};
 use numpy::Complex64;
 use rayon::prelude::*;
 
 use crate::{
-    quant::{AlignedIndex, Frequency, Time},
+    quant::{AlignedIndex, Amplitude, ChannelId, Frequency, Phase, Time},
     shape::Shape,
 };
 
 /// A pulse envelope
 ///
 /// If `shape` is `None`, constructor will set `plateau` to `width + plateau`
 /// and `width` to `0`.
@@ -28,17 +27,17 @@
     plateau: Time,
 }
 
 impl Envelope {
     pub fn new(mut shape: Option<Shape>, mut width: Time, mut plateau: Time) -> Self {
         if shape.is_none() {
             plateau += width;
-            width = Time::new(0.0).unwrap();
+            width = Time::ZERO;
         }
-        if width.value() == 0.0 {
+        if width == Time::ZERO {
             shape = None
         }
         Self {
             shape,
             width,
             plateau,
         }
@@ -86,42 +85,42 @@
 pub struct PulseList {
     items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
 }
 
 #[derive(Debug, Clone)]
 pub struct Crosstalk<'a> {
     matrix: ArrayView2<'a, f64>,
-    names: Vec<String>,
+    names: Vec<ChannelId>,
 }
 
 impl<'a> Crosstalk<'a> {
-    pub fn new(matrix: ArrayView2<'a, f64>, names: Vec<String>) -> Self {
+    pub fn new(matrix: ArrayView2<'a, f64>, names: Vec<ChannelId>) -> Self {
         Self { matrix, names }
     }
 }
 
 #[derive(Debug)]
 pub struct Sampler<'a> {
-    channels: HashMap<String, Channel<'a>>,
-    pulse_lists: HashMap<String, PulseList>,
+    channels: HashMap<ChannelId, Channel<'a>>,
+    pulse_lists: HashMap<ChannelId, PulseList>,
     crosstalk: Option<Crosstalk<'a>>,
 }
 
 impl<'a> Sampler<'a> {
-    pub fn new(pulse_lists: HashMap<String, PulseList>) -> Self {
+    pub fn new(pulse_lists: HashMap<ChannelId, PulseList>) -> Self {
         Self {
             channels: HashMap::new(),
             pulse_lists,
             crosstalk: None,
         }
     }
 
     pub fn add_channel(
         &mut self,
-        name: String,
+        name: ChannelId,
         waveform: ArrayViewMut2<'a, f64>,
         sample_rate: Frequency,
         delay: Time,
         align_level: i32,
     ) {
         self.channels.insert(
             name.clone(),
@@ -130,28 +129,28 @@
                 sample_rate,
                 align_level,
                 delay,
             },
         );
     }
 
-    pub fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>, names: Vec<String>) {
+    pub fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>, names: Vec<ChannelId>) {
         self.crosstalk = Some(Crosstalk::new(crosstalk, names));
     }
 
-    pub fn sample(self, time_tolerance: f64) {
+    pub fn sample(self, time_tolerance: Time) {
         if let Some(crosstalk) = self.crosstalk {
             let ct_lookup = crosstalk
                 .names
                 .iter()
                 .enumerate()
-                .map(|(i, name)| (name.as_str(), i))
+                .map(|(i, name)| (name, i))
                 .collect::<HashMap<_, _>>();
             self.channels.into_par_iter().for_each(|(n, c)| {
-                let row_index = ct_lookup.get(n.as_str()).copied();
+                let row_index = ct_lookup.get(&n).copied();
                 if let Some(row_index) = row_index {
                     let row = crosstalk.matrix.slice(s![row_index, ..]);
                     let lists = row
                         .iter()
                         .copied()
                         .zip(&crosstalk.names)
                         .map(|(multiplier, in_name)| (multiplier, &self.pulse_lists[in_name]));
@@ -190,61 +189,66 @@
     align_level: i32,
     delay: Time,
 }
 
 #[derive(Debug, Clone)]
 pub struct PulseListBuilder {
     items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
-    amp_tolerance: f64,
-    time_tolerance: f64,
+    amp_tolerance: Amplitude,
+    time_tolerance: Time,
 }
 
 impl PulseListBuilder {
-    pub fn new(amp_tolerance: f64, time_tolerance: f64) -> Self {
+    pub fn new(amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
         Self {
             items: HashMap::new(),
             amp_tolerance,
             time_tolerance,
         }
     }
 
     pub fn push(
         &mut self,
         envelope: Envelope,
         global_freq: Frequency,
         local_freq: Frequency,
         time: Time,
-        amplitude: f64,
+        amplitude: Amplitude,
         drag_coef: f64,
-        phase: f64,
+        phase: Phase,
     ) {
-        if approx_eq!(f64, amplitude, 0.0, epsilon = self.amp_tolerance) {
+        if approx_eq!(
+            f64,
+            amplitude.value(),
+            0.0,
+            epsilon = self.amp_tolerance.value()
+        ) {
             return;
         }
         let bin = ListBin {
             envelope,
             global_freq,
             local_freq,
         };
-        let amp = Complex64::from_polar(amplitude, TAU * phase);
+        let amp = amplitude.value() * phase.phaser();
         let drag = amp * Complex64::i() * drag_coef;
         let amplitude = PulseAmplitude { amp, drag };
         self.items.entry(bin).or_default().push((time, amplitude));
     }
 
     pub fn build(mut self) -> PulseList {
         for pulses in self.items.values_mut() {
             pulses.sort_unstable_by_key(|(time, _)| *time);
             let mut i = 0;
             for j in 1..pulses.len() {
                 if approx_eq!(
                     f64,
                     pulses[i].0.value(),
                     pulses[j].0.value(),
-                    epsilon = self.time_tolerance
+                    epsilon = self.time_tolerance.value()
                 ) {
                     pulses[i].1 = pulses[i].1 + pulses[j].1;
                 } else {
                     i += 1;
                     pulses[i] = pulses[j];
                 }
             }
@@ -255,47 +259,51 @@
 }
 
 fn mix_add_envelope(
     mut waveform: ArrayViewMut2<f64>,
     envelope: &[f64],
     amplitude: Complex64,
     drag_amp: Complex64,
-    phase0: f64,
-    dphase: f64,
+    phase0: Phase,
+    dphase: Phase,
 ) {
-    let mut carrier = Complex64::from_polar(1.0, phase0);
-    let dcarrier = Complex64::from_polar(1.0, dphase);
+    let mut carrier = phase0.phaser();
+    let dcarrier = dphase.phaser();
     let slope_iter = (0..envelope.len()).map(|i| {
         let left = if i > 0 { envelope[i - 1] } else { 0.0 };
         let right = if i < envelope.len() - 1 {
             envelope[i + 1]
         } else {
             0.0
         };
         (right - left) / 2.0
     });
     for (mut y, env, slope) in izip!(waveform.columns_mut(), envelope.iter().copied(), slope_iter) {
         let w = carrier * (amplitude * env + drag_amp * slope);
         y[0] += w.re;
-        y[1] += w.im;
+        if let Some(y1) = y.get_mut(1) {
+            *y1 += w.im;
+        }
         carrier *= dcarrier;
     }
 }
 
 fn mix_add_plateau(
     mut waveform: ArrayViewMut2<f64>,
     amplitude: Complex64,
-    phase: f64,
-    dphase: f64,
+    phase: Phase,
+    dphase: Phase,
 ) {
-    let mut carrier = Complex64::from_polar(1.0, phase) * amplitude;
-    let dcarrier = Complex64::from_polar(1.0, dphase);
+    let mut carrier = phase.phaser() * amplitude;
+    let dcarrier = dphase.phaser();
     for mut y in waveform.columns_mut() {
         y[0] += carrier.re;
-        y[1] += carrier.im;
+        if let Some(y1) = y.get_mut(1) {
+            *y1 += carrier.im;
+        }
         carrier *= dcarrier;
     }
 }
 
 #[cached(size = 1024)]
 fn get_envelope(
     shape: Shape,
@@ -332,15 +340,15 @@
 
 fn merge_and_sample<'a>(
     lists: impl IntoIterator<Item = (f64, &'a PulseList)>,
     waveform: ArrayViewMut2<f64>,
     sample_rate: Frequency,
     delay: Time,
     align_level: i32,
-    time_tolerance: f64,
+    time_tolerance: Time,
 ) {
     let mut merged: HashMap<ListBin, Vec<_>> = HashMap::new();
     for (multiplier, list) in lists {
         if multiplier == 0.0 {
             continue;
         }
         for (bin, items) in &list.items {
@@ -354,15 +362,20 @@
     let merged = merged.into_iter().map(|(bin, items)| {
         (
             bin,
             items
                 .into_iter()
                 .kmerge_by(|a, b| a.0 < b.0)
                 .coalesce(|a, b| {
-                    if approx_eq!(f64, a.0.value(), b.0.value(), epsilon = time_tolerance) {
+                    if approx_eq!(
+                        f64,
+                        a.0.value(),
+                        b.0.value(),
+                        epsilon = time_tolerance.value()
+                    ) {
                         Ok((a.0, a.1 + b.1))
                     } else {
                         Err((a, b))
                     }
                 }),
         )
     });
@@ -384,26 +397,22 @@
             envelope,
             global_freq,
             local_freq,
         } = bin;
         for (time, PulseAmplitude { amp, drag }) in items {
             let t_start = time + delay;
             let i_frac_start = AlignedIndex::new(t_start, sample_rate, align_level).unwrap();
-            let i_start = i_frac_start.ceil();
-            let index_offset = i_frac_start.index_offset();
-            let global_freq = global_freq.value();
-            let local_freq = local_freq.value();
+            let i_start = i_frac_start.ceil_as_usize().unwrap();
+            let index_offset = i_frac_start.index_offset().unwrap();
             let total_freq = global_freq + local_freq;
-            let dt = 1.0 / sample_rate.value();
-            let phase0 = global_freq * (i_start.value() * dt - delay.value())
+            let dt = sample_rate.dt();
+            let phase0 = global_freq * (i_start as f64 * dt - delay)
                 + local_freq * index_offset.value() * dt;
             let dphase = total_freq * dt;
-            let phase0 = phase0 * TAU;
-            let dphase = dphase * TAU;
-            let mut waveform = waveform.slice_mut(s![.., i_start.value() as usize..]);
+            let mut waveform = waveform.slice_mut(s![.., i_start..]);
             if let Some(shape) = &envelope.shape {
                 let envelope = get_envelope(
                     shape.clone(),
                     envelope.width,
                     envelope.plateau,
                     index_offset,
                     sample_rate,
```

### Comparing `bosing-2.0.0b9/src/schedule/absolute.rs` & `bosing-2.0.1/src/schedule/absolute.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 use anyhow::{bail, Result};
 use itertools::Itertools as _;
 
 use super::{
     arrange, measure, ArrangeContext, ArrangeResult, ArrangeResultVariant, ElementRef,
     MeasureContext, MeasureResult, MeasureResultVariant, Schedule,
 };
+use crate::quant::{ChannelId, Time};
 
 #[derive(Debug, Clone)]
 pub struct AbsoluteEntry {
-    time: f64,
+    time: Time,
     element: ElementRef,
 }
 
 impl AbsoluteEntry {
     pub fn new(element: ElementRef) -> Self {
-        Self { time: 0.0, element }
+        Self {
+            time: Time::ZERO,
+            element,
+        }
     }
 
-    pub fn with_time(mut self, time: f64) -> Result<Self> {
-        if !time.is_finite() {
-            bail!("Invalid time {}", time);
+    pub fn with_time(mut self, time: Time) -> Result<Self> {
+        if !time.value().is_finite() {
+            bail!("Invalid time {:?}", time);
         }
         self.time = time;
         Ok(self)
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Absolute {
     children: Vec<AbsoluteEntry>,
-    channel_ids: Vec<String>,
+    channel_ids: Vec<ChannelId>,
+}
+
+impl Default for Absolute {
+    fn default() -> Self {
+        Self::new()
+    }
 }
 
 impl Absolute {
     pub fn new() -> Self {
         Self {
             children: vec![],
             channel_ids: vec![],
@@ -51,15 +61,15 @@
         self.channel_ids = channel_ids;
         self
     }
 }
 
 impl Schedule for Absolute {
     fn measure(&self, context: &MeasureContext) -> MeasureResult {
-        let mut max_time: f64 = 0.0;
+        let mut max_time = Time::ZERO;
         let mut measured_children = vec![];
         for e in &self.children {
             let measured_child = measure(e.element.clone(), context.max_duration);
             max_time = max_time.max(e.time + measured_child.duration);
             measured_children.push(measured_child);
         }
         MeasureResult(max_time, MeasureResultVariant::Multiple(measured_children))
@@ -79,11 +89,11 @@
             .collect::<Result<_>>()?;
         Ok(ArrangeResult(
             context.final_duration,
             ArrangeResultVariant::Multiple(arranged_children),
         ))
     }
 
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
```

### Comparing `bosing-2.0.0b9/src/schedule/grid.rs` & `bosing-2.0.1/src/schedule/grid.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 use anyhow::{bail, Result};
 use itertools::Itertools as _;
-use ordered_float::OrderedFloat;
 
 use super::{
     arrange, measure, Alignment, ArrangeContext, ArrangeResult, ArrangeResultVariant, ElementRef,
     MeasureContext, MeasureResult, MeasureResultVariant, Schedule,
 };
-use crate::{GridLength, GridLengthUnit};
+use crate::{
+    quant::{ChannelId, Time},
+    GridLength, GridLengthUnit,
+};
 
 #[derive(Debug, Clone)]
 pub struct GridEntry {
     element: ElementRef,
     column: usize,
     span: usize,
 }
@@ -35,15 +37,21 @@
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Grid {
     children: Vec<GridEntry>,
     columns: Vec<GridLength>,
-    channel_ids: Vec<String>,
+    channel_ids: Vec<ChannelId>,
+}
+
+impl Default for Grid {
+    fn default() -> Self {
+        Self::new()
+    }
 }
 
 impl Grid {
     pub fn new() -> Self {
         Self {
             children: vec![],
             columns: vec![GridLength::star(1.0).unwrap()],
@@ -85,16 +93,18 @@
             .children
             .iter()
             .map(|e| measure(e.element.clone(), context.max_duration))
             .collect();
         let mut col_sizes: Vec<_> = columns
             .iter()
             .map(|c| match c.unit {
-                GridLengthUnit::Seconds => c.value,
-                _ => 0.0,
+                GridLengthUnit::Seconds => {
+                    Time::new(c.value).expect("Should be checked in GridLenth")
+                }
+                _ => Time::ZERO,
             })
             .collect();
         let it = measured_children
             .iter()
             .zip_eq(self.children.iter())
             .map(|(m, e)| (m.duration, e.column, e.span));
         for (dur, col, span) in it.clone() {
@@ -106,15 +116,15 @@
         }
         for (dur, col, span) in it {
             let col = col.min(n_col - 1);
             let span = span.min(n_col - col);
             if span == 1 {
                 continue;
             }
-            let col_size: f64 = col_sizes.iter().skip(col).take(span).sum();
+            let col_size: Time = col_sizes.iter().skip(col).take(span).sum();
             if col_size >= dur {
                 continue;
             }
             let n_star = columns
                 .iter()
                 .skip(col)
                 .take(span)
@@ -152,25 +162,25 @@
     fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult> {
         let (measured_children, mut col_sizes) = match &context.measured_self.data {
             MeasureResultVariant::Grid(children, col_sizes) => (children, col_sizes.clone()),
             _ => bail!("Invalid measure data"),
         };
         let columns = &self.columns;
         let n_col = columns.len();
-        let min_duration: f64 = col_sizes.iter().sum();
+        let min_duration: Time = col_sizes.iter().sum();
         expand_col_by_ratio(
             &mut col_sizes,
             0,
             n_col,
             context.final_duration - min_duration,
             columns,
         );
-        let col_starts: Vec<_> = std::iter::once(0.0)
+        let col_starts: Vec<_> = std::iter::once(Time::ZERO)
             .chain(col_sizes.iter().copied())
-            .scan(0.0, |state, x| {
+            .scan(Time::ZERO, |state, x| {
                 *state += x;
                 Some(*state)
             })
             .collect();
         let arranged_children = measured_children
             .iter()
             .zip(self.children.iter())
@@ -183,52 +193,52 @@
                     Alignment::Stretch => span_duration,
                     _ => measured.duration,
                 }
                 .min(span_duration);
                 let child_time = match measured.element.common.alignment {
                     Alignment::End => span_duration - child_duration,
                     Alignment::Center => (span_duration - child_duration) / 2.0,
-                    _ => 0.0,
+                    _ => Time::ZERO,
                 } + col_starts[col];
                 arrange(measured, child_time, child_duration, context.options)
             })
             .collect::<Result<_>>()?;
         Ok(ArrangeResult(
             context.final_duration,
             ArrangeResultVariant::Multiple(arranged_children),
         ))
     }
 
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
 
 fn expand_col_by_ratio(
-    col_sizes: &mut [f64],
+    col_sizes: &mut [Time],
     start: usize,
     span: usize,
-    mut left_dur: f64,
+    mut left_dur: Time,
     columns: &[GridLength],
 ) {
     let mut sorted: Vec<_> = col_sizes
         .iter_mut()
         .zip(columns)
         .skip(start)
         .take(span)
         .filter(|(_, c)| c.unit == GridLengthUnit::Star)
         .map(|(s, c)| (*s / c.value, s, c.value))
-        .sorted_by_key(|(k, _, _)| OrderedFloat(*k))
+        .sorted_by_key(|(k, _, _)| *k)
         .collect();
     let mut star_count = 0.0;
     for i in 0..sorted.len() {
         let next_ratio = if i + 1 < sorted.len() {
             sorted[i + 1].0
         } else {
-            f64::INFINITY
+            Time::INFINITY
         };
         star_count += sorted[i].2;
         left_dur += *sorted[i].1;
         let new_ratio = left_dur / star_count;
         if new_ratio < next_ratio {
             for (_, s, v) in sorted.iter_mut().take(i + 1) {
                 **s = new_ratio * *v;
```

### Comparing `bosing-2.0.0b9/src/schedule/play.rs` & `bosing-2.0.1/src/schedule/play.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,119 +1,120 @@
 use anyhow::{bail, Result};
 
 use super::{
     ArrangeContext, ArrangeResult, ArrangeResultVariant, MeasureContext, MeasureResult,
     MeasureResultVariant, Schedule,
 };
+use crate::quant::{Amplitude, ChannelId, Frequency, Phase, ShapeId, Time};
 
 #[derive(Debug, Clone)]
 pub struct Play {
-    channel_id: [String; 1],
-    shape_id: Option<String>,
-    amplitude: f64,
-    width: f64,
-    plateau: f64,
+    channel_id: [ChannelId; 1],
+    shape_id: Option<ShapeId>,
+    amplitude: Amplitude,
+    width: Time,
+    plateau: Time,
     drag_coef: f64,
-    frequency: f64,
-    phase: f64,
+    frequency: Frequency,
+    phase: Phase,
     flexible: bool,
 }
 
 impl Play {
     pub fn new(
-        channel_id: String,
-        shape_id: Option<String>,
-        amplitude: f64,
-        width: f64,
+        channel_id: ChannelId,
+        shape_id: Option<ShapeId>,
+        amplitude: Amplitude,
+        width: Time,
     ) -> Result<Self> {
-        if !amplitude.is_finite() {
-            bail!("Invalid amplitude {}", amplitude);
+        if !amplitude.value().is_finite() {
+            bail!("Invalid amplitude {:?}", amplitude);
         }
-        if !width.is_finite() || width < 0.0 {
-            bail!("Invalid width {}", width);
+        if !width.value().is_finite() || width.value() < 0.0 {
+            bail!("Invalid width {:?}", width);
         }
         Ok(Self {
             channel_id: [channel_id],
             shape_id,
             amplitude,
             width,
-            plateau: 0.0,
+            plateau: Time::ZERO,
             drag_coef: 0.0,
-            frequency: 0.0,
-            phase: 0.0,
+            frequency: Frequency::ZERO,
+            phase: Phase::ZERO,
             flexible: false,
         })
     }
 
-    pub fn with_plateau(mut self, plateau: f64) -> Result<Self> {
-        if !plateau.is_finite() || plateau < 0.0 {
-            bail!("Invalid plateau {}", plateau);
+    pub fn with_plateau(mut self, plateau: Time) -> Result<Self> {
+        if !plateau.value().is_finite() || plateau.value() < 0.0 {
+            bail!("Invalid plateau {:?}", plateau);
         }
         self.plateau = plateau;
         Ok(self)
     }
 
     pub fn with_drag_coef(mut self, drag_coef: f64) -> Result<Self> {
         if !drag_coef.is_finite() {
             bail!("Invalid drag_coef {}", drag_coef);
         }
         self.drag_coef = drag_coef;
         Ok(self)
     }
 
-    pub fn with_frequency(mut self, frequency: f64) -> Result<Self> {
-        if !frequency.is_finite() {
-            bail!("Invalid frequency {}", frequency);
+    pub fn with_frequency(mut self, frequency: Frequency) -> Result<Self> {
+        if !frequency.value().is_finite() {
+            bail!("Invalid frequency {:?}", frequency);
         }
         self.frequency = frequency;
         Ok(self)
     }
 
-    pub fn with_phase(mut self, phase: f64) -> Result<Self> {
-        if !phase.is_finite() {
-            bail!("Invalid phase {}", phase);
+    pub fn with_phase(mut self, phase: Phase) -> Result<Self> {
+        if !phase.value().is_finite() {
+            bail!("Invalid phase {:?}", phase);
         }
         self.phase = phase;
         Ok(self)
     }
 
     pub fn with_flexible(mut self, flexible: bool) -> Self {
         self.flexible = flexible;
         self
     }
 
-    pub fn channel_id(&self) -> &str {
+    pub fn channel_id(&self) -> &ChannelId {
         &self.channel_id[0]
     }
 
-    pub fn shape_id(&self) -> Option<&str> {
-        self.shape_id.as_deref()
+    pub fn shape_id(&self) -> Option<&ShapeId> {
+        self.shape_id.as_ref()
     }
 
-    pub fn amplitude(&self) -> f64 {
+    pub fn amplitude(&self) -> Amplitude {
         self.amplitude
     }
 
-    pub fn width(&self) -> f64 {
+    pub fn width(&self) -> Time {
         self.width
     }
 
-    pub fn plateau(&self) -> f64 {
+    pub fn plateau(&self) -> Time {
         self.plateau
     }
 
     pub fn drag_coef(&self) -> f64 {
         self.drag_coef
     }
 
-    pub fn frequency(&self) -> f64 {
+    pub fn frequency(&self) -> Frequency {
         self.frequency
     }
 
-    pub fn phase(&self) -> f64 {
+    pub fn phase(&self) -> Phase {
         self.phase
     }
 
     pub fn flexible(&self) -> bool {
         self.flexible
     }
 }
@@ -133,11 +134,11 @@
             context.final_duration
         } else {
             self.width + self.plateau
         };
         Ok(ArrangeResult(arranged, ArrangeResultVariant::Simple))
     }
 
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_id
     }
 }
```

### Comparing `bosing-2.0.0b9/src/schedule/repeat.rs` & `bosing-2.0.1/src/schedule/repeat.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 use anyhow::{bail, Result};
 
 use super::{
     arrange, measure, ArrangeContext, ArrangeResult, ArrangeResultVariant, ElementRef,
     MeasureContext, MeasureResult, MeasureResultVariant, Schedule,
 };
+use crate::quant::{ChannelId, Time};
 
 #[derive(Debug, Clone)]
 pub struct Repeat {
     child: ElementRef,
     count: usize,
-    spacing: f64,
+    spacing: Time,
 }
 
 impl Repeat {
     pub fn new(child: ElementRef, count: usize) -> Self {
         Self {
             child,
             count,
-            spacing: 0.0,
+            spacing: Time::ZERO,
         }
     }
 
-    pub fn with_spacing(mut self, spacing: f64) -> Result<Self> {
-        if !spacing.is_finite() {
-            bail!("Invalid spacing {}", spacing);
+    pub fn with_spacing(mut self, spacing: Time) -> Result<Self> {
+        if !spacing.value().is_finite() {
+            bail!("Invalid spacing {:?}", spacing);
         }
         self.spacing = spacing;
         Ok(self)
     }
 
     pub fn count(&self) -> usize {
         self.count
     }
 
-    pub fn spacing(&self) -> f64 {
+    pub fn spacing(&self) -> Time {
         self.spacing
     }
 }
 
 impl Schedule for Repeat {
     fn measure(&self, context: &MeasureContext) -> MeasureResult {
         if self.count == 0 {
-            return MeasureResult(0.0, MeasureResultVariant::Simple);
+            return MeasureResult(Time::ZERO, MeasureResultVariant::Simple);
         }
         let n = self.count as f64;
         let duration_per_repeat = (context.max_duration - self.spacing * (n - 1.0)) / n;
         let measured_child = measure(self.child.clone(), duration_per_repeat);
         let wanted_duration = measured_child.duration * n + self.spacing * (n - 1.0);
         MeasureResult(
             wanted_duration,
             MeasureResultVariant::Multiple(vec![measured_child]),
         )
     }
 
     fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult> {
         if self.count == 0 {
-            return Ok(ArrangeResult(0.0, ArrangeResultVariant::Simple));
+            return Ok(ArrangeResult(Time::ZERO, ArrangeResultVariant::Simple));
         }
         let n = self.count as f64;
         let duration_per_repeat = (context.final_duration - self.spacing * (n - 1.0)) / n;
         let measured_child = match &context.measured_self.data {
             MeasureResultVariant::Multiple(c) if c.len() == 1 => &c[0],
             _ => bail!("Invalid measure data"),
         };
-        let arranged_child = arrange(measured_child, 0.0, duration_per_repeat, context.options)?;
+        let arranged_child = arrange(
+            measured_child,
+            Time::ZERO,
+            duration_per_repeat,
+            context.options,
+        )?;
         let arranged = arranged_child.inner_duration * n + self.spacing * (n - 1.0);
         Ok(ArrangeResult(
             arranged,
             ArrangeResultVariant::Multiple(vec![arranged_child]),
         ))
     }
 
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         self.child.variant.channels()
     }
 }
```

### Comparing `bosing-2.0.0b9/src/schedule/simple.rs` & `bosing-2.0.1/src/schedule/simple.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,203 +1,204 @@
 use anyhow::{bail, Result};
 
 use super::{
     ArrangeContext, ArrangeResult, ArrangeResultVariant, MeasureContext, MeasureResult,
     MeasureResultVariant, Schedule,
 };
+use crate::quant::{ChannelId, Frequency, Phase, Time};
 
 trait SimpleElement {
-    fn channels(&self) -> &[String];
+    fn channels(&self) -> &[ChannelId];
 }
 
 impl<T> Schedule for T
 where
     T: SimpleElement,
 {
     fn measure(&self, _context: &MeasureContext) -> MeasureResult {
-        MeasureResult(0.0, MeasureResultVariant::Simple)
+        MeasureResult(Time::ZERO, MeasureResultVariant::Simple)
     }
 
     fn arrange(&self, _context: &ArrangeContext) -> Result<ArrangeResult> {
-        Ok(ArrangeResult(0.0, ArrangeResultVariant::Simple))
+        Ok(ArrangeResult(Time::ZERO, ArrangeResultVariant::Simple))
     }
 
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         self.channels()
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ShiftPhase {
-    channel_id: [String; 1],
-    phase: f64,
+    channel_id: [ChannelId; 1],
+    phase: Phase,
 }
 
 impl ShiftPhase {
-    pub fn new(channel_id: String, phase: f64) -> Result<Self> {
-        if !phase.is_finite() {
-            bail!("Invalid phase {}", phase);
+    pub fn new(channel_id: ChannelId, phase: Phase) -> Result<Self> {
+        if !phase.value().is_finite() {
+            bail!("Invalid phase {:?}", phase);
         }
         Ok(Self {
             channel_id: [channel_id],
             phase,
         })
     }
 
-    pub fn channel_id(&self) -> &str {
+    pub fn channel_id(&self) -> &ChannelId {
         &self.channel_id[0]
     }
 
-    pub fn phase(&self) -> f64 {
+    pub fn phase(&self) -> Phase {
         self.phase
     }
 }
 
 impl SimpleElement for ShiftPhase {
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct SetPhase {
-    channel_id: [String; 1],
-    phase: f64,
+    channel_id: [ChannelId; 1],
+    phase: Phase,
 }
 
 impl SetPhase {
-    pub fn new(channel_id: String, phase: f64) -> Result<Self> {
-        if !phase.is_finite() {
-            bail!("Invalid phase {}", phase);
+    pub fn new(channel_id: ChannelId, phase: Phase) -> Result<Self> {
+        if !phase.value().is_finite() {
+            bail!("Invalid phase {:?}", phase);
         }
         Ok(Self {
             channel_id: [channel_id],
             phase,
         })
     }
 
-    pub fn channel_id(&self) -> &str {
+    pub fn channel_id(&self) -> &ChannelId {
         &self.channel_id[0]
     }
 
-    pub fn phase(&self) -> f64 {
+    pub fn phase(&self) -> Phase {
         self.phase
     }
 }
 
 impl SimpleElement for SetPhase {
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ShiftFreq {
-    channel_id: [String; 1],
-    frequency: f64,
+    channel_id: [ChannelId; 1],
+    frequency: Frequency,
 }
 
 impl ShiftFreq {
-    pub fn new(channel_id: String, frequency: f64) -> Result<Self> {
-        if !frequency.is_finite() {
-            bail!("Invalid frequency {}", frequency);
+    pub fn new(channel_id: ChannelId, frequency: Frequency) -> Result<Self> {
+        if !frequency.value().is_finite() {
+            bail!("Invalid frequency {:?}", frequency);
         }
         Ok(Self {
             channel_id: [channel_id],
             frequency,
         })
     }
 
-    pub fn channel_id(&self) -> &str {
+    pub fn channel_id(&self) -> &ChannelId {
         &self.channel_id[0]
     }
 
-    pub fn frequency(&self) -> f64 {
+    pub fn frequency(&self) -> Frequency {
         self.frequency
     }
 }
 
 impl SimpleElement for ShiftFreq {
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct SetFreq {
-    channel_id: [String; 1],
-    frequency: f64,
+    channel_id: [ChannelId; 1],
+    frequency: Frequency,
 }
 
 impl SetFreq {
-    pub fn new(channel_id: String, frequency: f64) -> Result<Self> {
-        if !frequency.is_finite() {
-            bail!("Invalid frequency {}", frequency);
+    pub fn new(channel_id: ChannelId, frequency: Frequency) -> Result<Self> {
+        if !frequency.value().is_finite() {
+            bail!("Invalid frequency {:?}", frequency);
         }
         Ok(Self {
             channel_id: [channel_id],
             frequency,
         })
     }
 
-    pub fn channel_id(&self) -> &str {
+    pub fn channel_id(&self) -> &ChannelId {
         &self.channel_id[0]
     }
 
-    pub fn frequency(&self) -> f64 {
+    pub fn frequency(&self) -> Frequency {
         self.frequency
     }
 }
 
 impl SimpleElement for SetFreq {
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct SwapPhase {
-    channel_ids: [String; 2],
+    channel_ids: [ChannelId; 2],
 }
 
 impl SwapPhase {
-    pub fn new(channel_id1: String, channel_id2: String) -> Self {
+    pub fn new(channel_id1: ChannelId, channel_id2: ChannelId) -> Self {
         Self {
             channel_ids: [channel_id1, channel_id2],
         }
     }
 
-    pub fn channel_id1(&self) -> &str {
+    pub fn channel_id1(&self) -> &ChannelId {
         &self.channel_ids[0]
     }
 
-    pub fn channel_id2(&self) -> &str {
+    pub fn channel_id2(&self) -> &ChannelId {
         &self.channel_ids[1]
     }
 }
 
 impl SimpleElement for SwapPhase {
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Barrier {
-    channel_ids: Vec<String>,
+    channel_ids: Vec<ChannelId>,
 }
 
 impl Barrier {
-    pub fn new(channel_ids: Vec<String>) -> Self {
+    pub fn new(channel_ids: Vec<ChannelId>) -> Self {
         Self { channel_ids }
     }
 
-    pub fn channel_ids(&self) -> &[String] {
+    pub fn channel_ids(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
 
 impl SimpleElement for Barrier {
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
```

### Comparing `bosing-2.0.0b9/src/schedule/stack.rs` & `bosing-2.0.1/src/schedule/stack.rs`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,30 @@
 use hashbrown::HashMap;
 use itertools::{Either, Itertools as _};
 
 use super::{
     arrange, measure, ArrangeContext, ArrangeResult, ArrangeResultVariant, ElementRef,
     MeasureContext, MeasureResult, MeasureResultVariant, MeasuredElement, Schedule,
 };
-use crate::Direction;
+use crate::{
+    quant::{ChannelId, Time},
+    Direction,
+};
 
 #[derive(Debug, Clone)]
 pub struct Stack {
     children: Vec<ElementRef>,
     direction: Direction,
-    channel_ids: Vec<String>,
+    channel_ids: Vec<ChannelId>,
+}
+
+impl Default for Stack {
+    fn default() -> Self {
+        Self::new()
+    }
 }
 
 impl Stack {
     pub fn new() -> Self {
         Self {
             children: vec![],
             direction: Direction::Backward,
@@ -45,17 +54,17 @@
         self.direction
     }
 }
 
 impl Schedule for Stack {
     fn measure(&self, context: &MeasureContext) -> MeasureResult {
         let mut used_duration = if self.channel_ids.is_empty() {
-            Either::Left(0.0)
+            Either::Left(Time::ZERO)
         } else {
-            Either::Right(HashMap::<String, f64>::new())
+            Either::Right(HashMap::<ChannelId, Time>::new())
         };
         let mapper = |child: &ElementRef| {
             let child_channels = child.variant.channels();
             let channel_used_duration = get_channel_usage(&used_duration, child_channels);
             let child_available_duration = context.max_duration - channel_used_duration;
             let measured_child = measure(child.clone(), child_available_duration);
             let channel_used_duration = channel_used_duration + measured_child.duration;
@@ -72,30 +81,27 @@
             Direction::Backward => self.children.iter().rev().map(mapper).collect(),
         };
         if self.direction == Direction::Backward {
             measured_children.reverse();
         }
         let total_used_duration = match used_duration {
             Either::Left(v) => v,
-            Either::Right(d) => d
-                .into_values()
-                .max_by(|a, b| a.total_cmp(b))
-                .unwrap_or_default(),
+            Either::Right(d) => d.into_values().max().unwrap_or_default(),
         };
         MeasureResult(
             total_used_duration,
             super::MeasureResultVariant::Multiple(measured_children),
         )
     }
 
     fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult> {
         let mut used_duration = if self.channel_ids.is_empty() {
-            Either::Left(0.0)
+            Either::Left(Time::ZERO)
         } else {
-            Either::Right(HashMap::<String, f64>::new())
+            Either::Right(HashMap::<ChannelId, Time>::new())
         };
         let measured_children = match &context.measured_self.data {
             MeasureResultVariant::Multiple(v) => v,
             _ => bail!("Invalid measure data"),
         };
         let mapper = |child: &MeasuredElement| {
             let child_channels = child.element.variant.channels();
@@ -126,45 +132,42 @@
         }
         Ok(ArrangeResult(
             context.final_duration,
             ArrangeResultVariant::Multiple(arranged_children),
         ))
     }
 
-    fn channels(&self) -> &[String] {
+    fn channels(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
 
 fn update_channel_usage(
-    used_duration: &mut Either<f64, HashMap<String, f64>>,
-    new_duration: f64,
-    channels: &[String],
+    used_duration: &mut Either<Time, HashMap<ChannelId, Time>>,
+    new_duration: Time,
+    channels: &[ChannelId],
 ) {
     match used_duration {
         Either::Left(v) => *v = new_duration,
         Either::Right(d) => {
             for ch in channels {
                 d.insert(ch.clone(), new_duration);
             }
         }
     }
 }
 
 fn get_channel_usage(
-    used_duration: &Either<f64, HashMap<String, f64>>,
-    channels: &[String],
-) -> f64 {
+    used_duration: &Either<Time, HashMap<ChannelId, Time>>,
+    channels: &[ChannelId],
+) -> Time {
     match used_duration {
         Either::Left(v) => *v,
         Either::Right(d) => (if channels.is_empty() {
-            d.values().max_by(|a, b| a.total_cmp(b))
+            d.values().max()
         } else {
-            channels
-                .iter()
-                .filter_map(|i| d.get(i))
-                .max_by(|a, b| a.total_cmp(b))
+            channels.iter().filter_map(|i| d.get(i)).max()
         })
         .copied()
         .unwrap_or_default(),
     }
 }
```

### Comparing `bosing-2.0.0b9/src/schedule.rs` & `bosing-2.0.1/src/schedule.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use std::sync::Arc;
 
 use anyhow::{bail, Result};
-use enum_dispatch::enum_dispatch;
 
-use crate::Alignment;
+use crate::{
+    quant::{ChannelId, Time},
+    Alignment,
+};
 pub use absolute::{Absolute, AbsoluteEntry};
 pub use grid::{Grid, GridEntry};
 pub use play::Play;
 pub use repeat::Repeat;
 pub use simple::{Barrier, SetFreq, SetPhase, ShiftFreq, ShiftPhase, SwapPhase};
 pub use stack::Stack;
 
@@ -18,144 +20,59 @@
 mod simple;
 mod stack;
 
 pub type ElementRef = Arc<Element>;
 
 #[derive(Debug, Clone)]
 pub struct Element {
-    common: ElementCommon,
-    variant: ElementVariant,
+    pub common: ElementCommon,
+    pub variant: ElementVariant,
 }
 
 impl Element {
     pub fn new(common: ElementCommon, variant: impl Into<ElementVariant>) -> Self {
         Self {
             common,
             variant: variant.into(),
         }
     }
-
-    pub fn common(&self) -> &ElementCommon {
-        &self.common
-    }
-
-    pub fn variant(&self) -> &ElementVariant {
-        &self.variant
-    }
-
-    pub fn try_get_play(&self) -> Option<&Play> {
-        match &self.variant {
-            ElementVariant::Play(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_shift_phase(&self) -> Option<&ShiftPhase> {
-        match &self.variant {
-            ElementVariant::ShiftPhase(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_set_phase(&self) -> Option<&SetPhase> {
-        match &self.variant {
-            ElementVariant::SetPhase(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_shift_freq(&self) -> Option<&ShiftFreq> {
-        match &self.variant {
-            ElementVariant::ShiftFreq(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_set_freq(&self) -> Option<&SetFreq> {
-        match &self.variant {
-            ElementVariant::SetFreq(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_swap_phase(&self) -> Option<&SwapPhase> {
-        match &self.variant {
-            ElementVariant::SwapPhase(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_barrier(&self) -> Option<&Barrier> {
-        match &self.variant {
-            ElementVariant::Barrier(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_repeat(&self) -> Option<&Repeat> {
-        match &self.variant {
-            ElementVariant::Repeat(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_stack(&self) -> Option<&Stack> {
-        match &self.variant {
-            ElementVariant::Stack(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_absolute(&self) -> Option<&Absolute> {
-        match &self.variant {
-            ElementVariant::Absolute(v) => Some(v),
-            _ => None,
-        }
-    }
-
-    pub fn try_get_grid(&self) -> Option<&Grid> {
-        match &self.variant {
-            ElementVariant::Grid(v) => Some(v),
-            _ => None,
-        }
-    }
 }
 
 #[derive(Debug, Clone)]
 pub struct MeasuredElement {
     element: ElementRef,
     /// Desired duration without clipping. Doesn't include margin.
-    unclipped_duration: f64,
+    unclipped_duration: Time,
     /// Clipped desired duration. Used by scheduling system.
-    duration: f64,
+    duration: Time,
     data: MeasureResultVariant,
 }
 
 impl MeasuredElement {
-    pub fn duration(&self) -> f64 {
+    pub fn duration(&self) -> Time {
         self.duration
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ArrangedElement {
     element: ElementRef,
     /// Start time of the inner block without margin relative to its parent.
-    inner_time: f64,
+    inner_time: Time,
     /// Duration of the inner block without margin.
-    inner_duration: f64,
+    inner_duration: Time,
     data: ArrangeResultVariant,
 }
 
 impl ArrangedElement {
-    pub fn inner_time(&self) -> f64 {
+    pub fn inner_time(&self) -> Time {
         self.inner_time
     }
 
-    pub fn inner_duration(&self) -> f64 {
+    pub fn inner_duration(&self) -> Time {
         self.inner_duration
     }
 
     pub fn element(&self) -> &ElementRef {
         &self.element
     }
 
@@ -165,133 +82,114 @@
             _ => None,
         }
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ScheduleOptions {
-    pub time_tolerance: f64,
+    pub time_tolerance: Time,
     pub allow_oversize: bool,
 }
 
 #[derive(Debug, Clone)]
 enum MeasureResultVariant {
     Simple,
     Multiple(Vec<MeasuredElement>),
-    Grid(Vec<MeasuredElement>, Vec<f64>),
+    Grid(Vec<MeasuredElement>, Vec<Time>),
 }
 
 #[derive(Debug, Clone)]
-struct MeasureResult(f64, MeasureResultVariant);
+struct MeasureResult(Time, MeasureResultVariant);
 
 #[derive(Debug, Clone)]
 pub enum ArrangeResultVariant {
     Simple,
     Multiple(Vec<ArrangedElement>),
 }
 
 #[derive(Debug, Clone)]
-struct ArrangeResult(f64, ArrangeResultVariant);
+struct ArrangeResult(Time, ArrangeResultVariant);
 
 #[derive(Debug, Clone)]
 struct MeasureContext {
-    max_duration: f64,
+    max_duration: Time,
 }
 
 #[derive(Debug, Clone)]
 struct ArrangeContext<'a> {
-    final_duration: f64,
+    final_duration: Time,
     options: &'a ScheduleOptions,
     measured_self: &'a MeasuredElement,
 }
 
-#[enum_dispatch]
 trait Schedule {
     /// Measure the element and return desired inner size and measured children.
     fn measure(&self, context: &MeasureContext) -> MeasureResult;
     /// Arrange the element and return final inner size and arranged children.
     fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult>;
     /// Channels used by this element. Empty means all of parent's channels.
-    fn channels(&self) -> &[String];
+    fn channels(&self) -> &[ChannelId];
 }
 
-fn clamp_duration(duration: f64, min_duration: f64, max_duration: f64) -> f64 {
+fn clamp_duration(duration: Time, min_duration: Time, max_duration: Time) -> Time {
     duration.min(max_duration).max(min_duration)
 }
 
-pub fn measure(element: ElementRef, available_duration: f64) -> MeasuredElement {
-    assert!(available_duration >= 0.0 || available_duration.is_infinite());
+pub fn measure(element: ElementRef, available_duration: Time) -> MeasuredElement {
+    assert!(available_duration.value() >= 0.0);
     let common = &element.common;
-    let total_margin = common.margin.0 + common.margin.1;
-    assert!(total_margin.is_finite());
-    let max_duration = clamp_duration(
-        common.duration.unwrap_or(f64::INFINITY),
-        common.min_duration,
-        common.max_duration,
-    );
-    let min_duration = clamp_duration(
-        common.duration.unwrap_or(0.0),
-        common.min_duration,
-        common.max_duration,
-    );
-    let inner_duration = (available_duration - total_margin).max(0.0);
+    let total_margin = common.total_margin();
+    assert!(total_margin.value().is_finite());
+    let (min_duration, max_duration) = common.clamp_min_max_duration();
+    let inner_duration = (available_duration - total_margin).max(Time::ZERO);
     let inner_duration = clamp_duration(inner_duration, min_duration, max_duration);
     let result = element.variant.measure(&MeasureContext {
         max_duration: inner_duration,
     });
-    let unclipped_duration = (result.0 + total_margin).max(0.0);
+    let unclipped_duration = (result.0 + total_margin).max(Time::ZERO);
     let duration = clamp_duration(unclipped_duration, min_duration, max_duration) + total_margin;
-    let duration = clamp_duration(duration, 0.0, available_duration);
+    let duration = clamp_duration(duration, Time::ZERO, available_duration);
     MeasuredElement {
         element,
         unclipped_duration,
         duration,
         data: result.1,
     }
 }
 
 pub fn arrange(
     measured: &MeasuredElement,
-    time: f64,
-    duration: f64,
+    time: Time,
+    duration: Time,
     options: &ScheduleOptions,
 ) -> Result<ArrangedElement> {
     let MeasuredElement {
         element,
         unclipped_duration,
         ..
     } = measured;
     let common = &element.common;
     if duration < unclipped_duration - options.time_tolerance && !options.allow_oversize {
         bail!(
-            "Oversizing is configured to be disallowed: available duration {} < measured duration {}",
+            "Oversizing is configured to be disallowed: available duration {:?} < measured duration {:?}",
             duration,
             unclipped_duration
         );
     }
     let inner_time = time + common.margin.0;
-    assert!(inner_time.is_finite());
-    let max_duration = clamp_duration(
-        common.duration.unwrap_or(f64::INFINITY),
-        common.min_duration,
-        common.max_duration,
-    );
-    let min_duration = clamp_duration(
-        common.duration.unwrap_or(0.0),
-        common.min_duration,
-        common.max_duration,
-    );
-    let total_margin = common.margin.0 + common.margin.1;
-    let inner_duration = (duration - total_margin).max(0.0);
+    assert!(inner_time.value().is_finite());
+    let (min_duration, max_duration) = common.clamp_min_max_duration();
+    let total_margin = common.total_margin();
+    let inner_duration = (duration - total_margin).max(Time::ZERO);
     let inner_duration = clamp_duration(inner_duration, min_duration, max_duration);
     if inner_duration + total_margin < unclipped_duration - options.time_tolerance
         && !options.allow_oversize
     {
         bail!(
-            "Oversizing is configured to be disallowed: user requested duration {} < measured duration {}",
+            "Oversizing is configured to be disallowed: user requested duration {:?} < measured duration {:?}",
             inner_duration + total_margin,
             unclipped_duration
         );
     }
     let result = element.variant.arrange(&ArrangeContext {
         final_duration: inner_duration,
         options,
@@ -303,132 +201,198 @@
         inner_duration: result.0,
         data: result.1,
     })
 }
 
 #[derive(Debug, Clone)]
 pub struct ElementCommon {
-    margin: (f64, f64),
+    margin: (Time, Time),
     alignment: Alignment,
     phantom: bool,
-    duration: Option<f64>,
-    max_duration: f64,
-    min_duration: f64,
+    duration: Option<Time>,
+    max_duration: Time,
+    min_duration: Time,
 }
 
 impl ElementCommon {
-    pub fn margin(&self) -> (f64, f64) {
+    pub fn margin(&self) -> (Time, Time) {
         self.margin
     }
 
     pub fn alignment(&self) -> Alignment {
         self.alignment
     }
 
     pub fn phantom(&self) -> bool {
         self.phantom
     }
 
-    pub fn duration(&self) -> Option<f64> {
+    pub fn duration(&self) -> Option<Time> {
         self.duration
     }
 
-    pub fn max_duration(&self) -> f64 {
+    pub fn max_duration(&self) -> Time {
         self.max_duration
     }
 
-    pub fn min_duration(&self) -> f64 {
+    pub fn min_duration(&self) -> Time {
         self.min_duration
     }
+
+    fn clamp_min_max_duration(&self) -> (Time, Time) {
+        let max_duration = clamp_duration(
+            self.duration.unwrap_or(Time::INFINITY),
+            self.min_duration,
+            self.max_duration,
+        );
+        let min_duration = clamp_duration(
+            self.duration.unwrap_or(Time::ZERO),
+            self.min_duration,
+            self.max_duration,
+        );
+        (min_duration, max_duration)
+    }
+
+    fn total_margin(&self) -> Time {
+        self.margin.0 + self.margin.1
+    }
 }
 
 #[derive(Debug, Clone)]
 pub struct ElementCommonBuilder(ElementCommon);
 
 impl Default for ElementCommonBuilder {
     fn default() -> Self {
         Self(ElementCommon {
-            margin: (0.0, 0.0),
+            margin: Default::default(),
             alignment: Alignment::End,
             phantom: false,
             duration: None,
-            max_duration: f64::INFINITY,
-            min_duration: 0.0,
+            max_duration: Time::INFINITY,
+            min_duration: Default::default(),
         })
     }
 }
 
 impl ElementCommonBuilder {
     pub fn new() -> Self {
         Self::default()
     }
 
-    pub fn margin(&mut self, margin: (f64, f64)) -> &mut Self {
+    pub fn margin(&mut self, margin: (Time, Time)) -> &mut Self {
         self.0.margin = margin;
         self
     }
 
     pub fn alignment(&mut self, alignment: Alignment) -> &mut Self {
         self.0.alignment = alignment;
         self
     }
 
     pub fn phantom(&mut self, phantom: bool) -> &mut Self {
         self.0.phantom = phantom;
         self
     }
 
-    pub fn duration(&mut self, duration: Option<f64>) -> &mut Self {
+    pub fn duration(&mut self, duration: Option<Time>) -> &mut Self {
         self.0.duration = duration;
         self
     }
 
-    pub fn max_duration(&mut self, max_duration: f64) -> &mut Self {
+    pub fn max_duration(&mut self, max_duration: Time) -> &mut Self {
         self.0.max_duration = max_duration;
         self
     }
 
-    pub fn min_duration(&mut self, min_duration: f64) -> &mut Self {
+    pub fn min_duration(&mut self, min_duration: Time) -> &mut Self {
         self.0.min_duration = min_duration;
         self
     }
 
     pub fn validate(&self) -> Result<()> {
         let v = &self.0;
-        if !v.margin.0.is_finite() || !v.margin.1.is_finite() {
+        if !v.margin.0.value().is_finite() || !v.margin.1.value().is_finite() {
             bail!("Invalid margin {:?}", v.margin);
         }
         if let Some(v) = v.duration {
-            if !v.is_finite() || v < 0.0 {
-                bail!("Invalid duration {}", v);
+            if !v.value().is_finite() || v.value() < 0.0 {
+                bail!("Invalid duration {:?}", v);
             }
         }
-        if !v.min_duration.is_finite() || v.min_duration < 0.0 {
-            bail!("Invalid min_duration {}", v.min_duration);
+        if !v.min_duration.value().is_finite() || v.min_duration.value() < 0.0 {
+            bail!("Invalid min_duration {:?}", v.min_duration);
         }
-        if v.max_duration.is_nan() || v.max_duration < 0.0 {
-            bail!("Invalid max_duration {}", v.max_duration);
+        if v.max_duration.value() < 0.0 {
+            bail!("Invalid max_duration {:?}", v.max_duration);
         }
         Ok(())
     }
 
     pub fn build(&self) -> Result<ElementCommon> {
         self.validate()?;
         Ok(self.0.clone())
     }
 }
 
-#[enum_dispatch(Schedule)]
+macro_rules! impl_variant {
+    ($($variant:ident),*$(,)?) => {
 #[derive(Debug, Clone)]
 pub enum ElementVariant {
-    Play,
-    ShiftPhase,
-    SetPhase,
-    ShiftFreq,
-    SetFreq,
-    SwapPhase,
-    Barrier,
-    Repeat,
-    Stack,
-    Absolute,
-    Grid,
+    $($variant($variant),)*
+}
+
+$(
+impl From<$variant> for ElementVariant {
+    fn from(v: $variant) -> Self {
+        Self::$variant(v)
+    }
+}
+
+impl TryFrom<ElementVariant> for $variant {
+    type Error = anyhow::Error;
+
+    fn try_from(value: ElementVariant) -> Result<Self, Self::Error> {
+        match value {
+            ElementVariant::$variant(v) => Ok(v),
+            _ => bail!("Expected {} variant", stringify!($variant)),
+        }
+    }
+}
+
+impl<'a> TryFrom<&'a ElementVariant> for &'a $variant {
+    type Error = anyhow::Error;
+
+    fn try_from(value: &'a ElementVariant) -> Result<Self, Self::Error> {
+        match value {
+            ElementVariant::$variant(v) => Ok(v),
+            _ => bail!("Expected {} variant", stringify!($variant)),
+        }
+    }
+}
+)*
+
+impl Schedule for ElementVariant {
+    fn measure(&self, context: &MeasureContext) -> MeasureResult {
+        match self {
+            $(ElementVariant::$variant(v) => v.measure(context),)*
+        }
+    }
+
+    fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult> {
+        match self {
+            $(ElementVariant::$variant(v) => v.arrange(context),)*
+        }
+    }
+
+    fn channels(&self) -> &[ChannelId] {
+        match self {
+            $(ElementVariant::$variant(v) => v.channels(),)*
+        }
+    }
+}
+    };
 }
+
+impl_variant!(
+    Play, ShiftPhase, SetPhase, ShiftFreq, SetFreq, SwapPhase, Barrier, Repeat, Stack, Absolute,
+    Grid,
+);
```

### Comparing `bosing-2.0.0b9/tests/test_basic.py` & `bosing-2.0.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/Cargo.lock` & `bosing-2.0.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,19 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.0-beta.9"
+version = "2.0.1"
 dependencies = [
  "anyhow",
  "bspline",
  "cached",
- "enum_dispatch",
  "float-cmp",
  "hashbrown",
  "indoc",
  "itertools",
  "ndarray",
  "num",
  "numpy",
@@ -66,37 +65,37 @@
 dependencies = [
  "num-traits",
  "trait-set",
 ]
 
 [[package]]
 name = "cached"
-version = "0.49.3"
+version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e8e463fceca5674287f32d252fb1d94083758b8709c160efae66d263e5f4eba"
+checksum = "10a7d38ed2761b8a13ce42bc44b09d5a052b88da2f9fead624c779f31ac0729a"
 dependencies = [
  "ahash",
  "cached_proc_macro",
  "cached_proc_macro_types",
  "hashbrown",
  "instant",
  "once_cell",
  "thiserror",
 ]
 
 [[package]]
 name = "cached_proc_macro"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad9f16c0d84de31a2ab7fdf5f7783c14631f7075cf464eb3bb43119f61c9cb2a"
+checksum = "771aa57f3b17da6c8bcacb187bb9ec9bc81c8160e72342e67c329e0e1651a669"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "cached_proc_macro_types"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ade8366b8bd5ba243f0a58f036cc0ca8a2f069cff1a2351ef1cac6b083e16fc0"
@@ -130,66 +129,54 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "darling"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "either"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
-name = "enum_dispatch"
-version = "0.3.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
-dependencies = [
- "once_cell",
- "proc-macro2",
- "quote",
- "syn 2.0.58",
-]
-
-[[package]]
 name = "float-cmp"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
 dependencies = [
  "num-traits",
 ]
@@ -198,17 +185,17 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
  "rayon",
 ]
 
 [[package]]
@@ -294,17 +281,17 @@
  "num-traits",
  "rawpointer",
  "rayon",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -437,18 +424,19 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
+ "anyhow",
  "cfg-if",
  "hashbrown",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -456,49 +444,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
```

### Comparing `bosing-2.0.0b9/pyproject.toml` & `bosing-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b9/PKG-INFO` & `bosing-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.0b9
+Version: 2.0.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

