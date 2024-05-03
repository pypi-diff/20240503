# Comparing `tmp/deepdog-1.0.1.tar.gz` & `tmp/deepdog-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-1.0.1.tar", max compression
+gzip compressed data, was "deepdog-1.1.0.tar", max compression
```

## Comparing `deepdog-1.0.1.tar` & `deepdog-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
--rw-r--r--   0        0        0      605 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0     7661 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/bayes_run_with_ss.py
--rw-r--r--   0        0        0        0 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/cli/__init__.py
--rw-r--r--   0        0        0       80 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/cli/probs/__init__.py
--rw-r--r--   0        0        0     1389 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/cli/probs/args.py
--rw-r--r--   0        0        0     6243 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/cli/probs/dicts.py
--rw-r--r--   0        0        0     2945 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/cli/probs/main.py
--rw-r--r--   0        0        0      161 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/direct_monte_carlo/__init__.py
--rw-r--r--   0        0        0      461 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/direct_monte_carlo/compose_filter.py
--rw-r--r--   0        0        0     9191 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/direct_monte_carlo/direct_mc.py
--rw-r--r--   0        0        0     7127 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/direct_monte_carlo/dmc_filters.py
--rw-r--r--   0        0        0     1700 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/indexify/__init__.py
--rw-r--r--   0        0        0     2432 2024-05-02 02:09:25.194591 deepdog-1.0.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       73 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/meta.py
--rw-r--r--   0        0        0    12392 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     4858 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/results/__init__.py
--rw-r--r--   0        0        0     5927 2024-05-02 02:09:25.206592 deepdog-1.0.1/deepdog/results/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      110 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0      297 2024-05-02 02:09:25.186591 deepdog-1.0.1/deepdog/subset_simulation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9024 2024-05-02 02:09:25.190591 deepdog-1.0.1/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc
--rw-r--r--   0        0        0    11428 2024-05-02 02:08:52.868987 deepdog-1.0.1/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2024-05-02 02:08:52.872987 deepdog-1.0.1/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0     1084 2024-05-02 02:08:52.872987 deepdog-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      366 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/args.py
+-rw-r--r--   0        0        0     6243 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/dicts.py
+-rw-r--r--   0        0        0     2945 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/main.py
+-rw-r--r--   0        0        0      161 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-03 04:14:47.847241 deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7897 2024-05-03 04:14:47.851241 deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
+-rw-r--r--   0        0        0     3902 2024-05-03 04:14:47.855242 deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
+-rw-r--r--   0        0        0      461 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/compose_filter.py
+-rw-r--r--   0        0        0     9338 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/direct_mc.py
+-rw-r--r--   0        0        0     3393 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/dmc_filters.py
+-rw-r--r--   0        0        0     1700 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/indexify/__init__.py
+-rw-r--r--   0        0        0     2432 2024-05-03 04:14:47.911244 deepdog-1.1.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       73 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/meta.py
+-rw-r--r--   0        0        0    12392 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     4858 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/results/__init__.py
+-rw-r--r--   0        0        0     5927 2024-05-03 04:14:47.923245 deepdog-1.1.0/deepdog/results/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      110 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0    11428 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0     1084 2024-05-03 04:14:05.569158 deepdog-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.1.0/PKG-INFO
```

### Comparing `deepdog-1.0.1/deepdog/bayes_run_simulpairs.py` & `deepdog-1.1.0/deepdog/real_spectrum_run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,382 +1,442 @@
 import pdme.inputs
 import pdme.model
+import pdme.measurement
 import pdme.measurement.input_types
 import pdme.measurement.oscillating_dipole
 import pdme.util.fast_v_calc
 import pdme.util.fast_nonlocal_spectrum
-from typing import Sequence, Tuple, List
+from typing import Sequence, Tuple, List, Dict, Union, Optional
 import datetime
 import csv
 import multiprocessing
 import logging
 import numpy
-import numpy.random
 
 
 # TODO: remove hardcode
 CHUNKSIZE = 50
 
-# TODO: It's garbage to have this here duplicated from pdme.
-DotInput = Tuple[numpy.typing.ArrayLike, float]
-
 
 _logger = logging.getLogger(__name__)
 
 
-def get_a_simul_result_using_pairs(input) -> numpy.ndarray:
+def get_a_result_fast_filter_pairs(input) -> int:
 	(
 		model,
 		dot_inputs,
+		lows,
+		highs,
 		pair_inputs,
-		local_lows,
-		local_highs,
-		nonlocal_lows,
-		nonlocal_highs,
+		pair_lows,
+		pair_highs,
 		monte_carlo_count,
-		monte_carlo_cycles,
-		max_frequency,
 		seed,
 	) = input
 
 	rng = numpy.random.default_rng(seed)
-	local_total = 0
-	combined_total = 0
+	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
+	sample_dipoles = model.get_monte_carlo_dipole_inputs(
+		monte_carlo_count, None, rng_to_use=rng
+	)
+
+	current_sample = sample_dipoles
+	for di, low, high in zip(dot_inputs, lows, highs):
+
+		if len(current_sample) < 1:
+			break
+		vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(
+			numpy.array([di]), current_sample
+		)
+
+		current_sample = current_sample[numpy.all((vals > low) & (vals < high), axis=1)]
+
+	for pi, plow, phigh in zip(pair_inputs, pair_lows, pair_highs):
+		if len(current_sample) < 1:
+			break
+		vals = pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
+			numpy.array([pi]), current_sample
+		)
+
+		current_sample = current_sample[
+			numpy.all(
+				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
+				axis=1,
+			)
+		]
+	return len(current_sample)
+
 
+def get_a_result_fast_filter_potential_pair_phase_only(input) -> int:
+	(
+		model,
+		pair_inputs,
+		pair_phase_lows,
+		pair_phase_highs,
+		monte_carlo_count,
+		seed,
+	) = input
+
+	rng = numpy.random.default_rng(seed)
+	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
 	sample_dipoles = model.get_monte_carlo_dipole_inputs(
-		monte_carlo_count, max_frequency, rng_to_use=rng
+		monte_carlo_count, None, rng_to_use=rng
 	)
-	local_vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(dot_inputs, sample_dipoles)
-	local_matches = pdme.util.fast_v_calc.between(local_vals, local_lows, local_highs)
-	nonlocal_vals = pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
-		pair_inputs, sample_dipoles
+
+	current_sample = sample_dipoles
+
+	for pi, plow, phigh in zip(pair_inputs, pair_phase_lows, pair_phase_highs):
+		if len(current_sample) < 1:
+			break
+		vals = pdme.util.fast_nonlocal_spectrum.signarg(
+			pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
+				numpy.array([pi]), current_sample
+			)
+		)
+
+		current_sample = current_sample[
+			numpy.all(
+				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
+				axis=1,
+			)
+		]
+	return len(current_sample)
+
+
+def get_a_result_fast_filter_tarucha_spin_qubit_pair_phase_only(input) -> int:
+	(
+		model,
+		pair_inputs,
+		pair_phase_lows,
+		pair_phase_highs,
+		monte_carlo_count,
+		seed,
+	) = input
+
+	rng = numpy.random.default_rng(seed)
+	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
+	sample_dipoles = model.get_monte_carlo_dipole_inputs(
+		monte_carlo_count, None, rng_to_use=rng
 	)
-	nonlocal_matches = pdme.util.fast_v_calc.between(
-		nonlocal_vals, nonlocal_lows, nonlocal_highs
+
+	current_sample = sample_dipoles
+
+	for pi, plow, phigh in zip(pair_inputs, pair_phase_lows, pair_phase_highs):
+		if len(current_sample) < 1:
+			break
+
+		###
+		# This should be  abstracted out, but we're going to dump it here for time pressure's sake
+		###
+		# vals = pdme.util.fast_nonlocal_spectrum.signarg(
+		# 	pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
+		# 		numpy.array([pi]), current_sample
+		# 	)
+		#
+		vals = pdme.util.fast_nonlocal_spectrum.signarg(
+			pdme.util.fast_nonlocal_spectrum.fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
+				numpy.array([pi]), current_sample
+			)
+		)
+		current_sample = current_sample[
+			numpy.all(
+				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
+				axis=1,
+			)
+		]
+	return len(current_sample)
+
+
+def get_a_result_fast_filter(input) -> int:
+	model, dot_inputs, lows, highs, monte_carlo_count, seed = input
+
+	rng = numpy.random.default_rng(seed)
+	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
+	sample_dipoles = model.get_monte_carlo_dipole_inputs(
+		monte_carlo_count, None, rng_to_use=rng
 	)
-	combined_matches = numpy.logical_and(local_matches, nonlocal_matches)
 
-	local_total += numpy.count_nonzero(local_matches)
-	combined_total += numpy.count_nonzero(combined_matches)
-	return numpy.array([local_total, combined_total])
+	current_sample = sample_dipoles
+	for di, low, high in zip(dot_inputs, lows, highs):
+
+		if len(current_sample) < 1:
+			break
+		vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(
+			numpy.array([di]), current_sample
+		)
+
+		current_sample = current_sample[numpy.all((vals > low) & (vals < high), axis=1)]
+	return len(current_sample)
 
 
-class BayesRunSimulPairs:
+class RealSpectrumRun:
 	"""
-	A dual pairs-nonpairs Bayes run for a given set of dots.
+	A bayes run given some real data.
 
 	Parameters
 	----------
-	dot_inputs : Sequence[DotInput]
+	measurements : Sequence[pdme.measurement.DotRangeMeasurement]
 	The dot inputs for this bayes run.
 
 	models_with_names : Sequence[Tuple(str, pdme.model.DipoleModel)]
 	The models to evaluate.
 
 	actual_model : pdme.model.DipoleModel
-	The modoel for the model which is actually correct.
+	The model which is actually correct.
 
 	filename_slug : str
 	The filename slug to include.
 
 	run_count: int
 	The number of runs to do.
+
+	If pair_measurements is not None, uses pair measurement method (and single measurements too).
+	If pair_phase_measurements is not None, ignores measurements and uses phase measurements _only_
+	This is lazy design on my part.
+
 	"""
 
 	def __init__(
 		self,
-		dot_positions: Sequence[numpy.typing.ArrayLike],
-		frequency_range: Sequence[float],
+		measurements: Sequence[pdme.measurement.DotRangeMeasurement],
 		models_with_names: Sequence[Tuple[str, pdme.model.DipoleModel]],
-		actual_model: pdme.model.DipoleModel,
 		filename_slug: str,
-		run_count: int = 100,
-		low_error: float = 0.9,
-		high_error: float = 1.1,
-		pairs_high_error=None,
-		pairs_low_error=None,
 		monte_carlo_count: int = 10000,
 		monte_carlo_cycles: int = 10,
 		target_success: int = 100,
 		max_monte_carlo_cycles_steps: int = 10,
-		max_frequency: float = 20,
-		end_threshold: float = None,
 		chunksize: int = CHUNKSIZE,
+		initial_seed: int = 12345,
+		cap_core_count: int = 0,
+		pair_measurements: Optional[
+			Sequence[pdme.measurement.DotPairRangeMeasurement]
+		] = None,
+		pair_phase_measurements: Optional[
+			Sequence[pdme.measurement.DotPairRangeMeasurement]
+		] = None,
 	) -> None:
-		self.dot_inputs = pdme.inputs.inputs_with_frequency_range(
-			dot_positions, frequency_range
-		)
+		self.measurements = measurements
+		self.dot_inputs = [(measure.r, measure.f) for measure in self.measurements]
+
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
 			self.dot_inputs
 		)
 
-		self.dot_pair_inputs = pdme.inputs.input_pairs_with_frequency_range(
-			dot_positions, frequency_range
-		)
-		self.dot_pair_inputs_array = (
-			pdme.measurement.input_types.dot_pair_inputs_to_array(self.dot_pair_inputs)
-		)
+		if pair_measurements is not None:
+			self.pair_measurements = pair_measurements
+			self.use_pair_measurements = True
+			self.use_pair_phase_measurements = False
+
+			self.dot_pair_inputs = [
+				(measure.r1, measure.r2, measure.f)
+				for measure in self.pair_measurements
+			]
+			self.dot_pair_inputs_array = (
+				pdme.measurement.input_types.dot_pair_inputs_to_array(
+					self.dot_pair_inputs
+				)
+			)
+		elif pair_phase_measurements is not None:
+			self.use_pair_measurements = False
+			self.use_pair_phase_measurements = True
+			self.pair_phase_measurements = pair_phase_measurements
+			self.dot_pair_inputs = [
+				(measure.r1, measure.r2, measure.f)
+				for measure in self.pair_phase_measurements
+			]
+			self.dot_pair_inputs_array = (
+				pdme.measurement.input_types.dot_pair_inputs_to_array(
+					self.dot_pair_inputs
+				)
+			)
+		else:
+			self.use_pair_measurements = False
+			self.use_pair_phase_measurements = False
 
-		self.models = [mod for (_, mod) in models_with_names]
+		self.models = [model for (_, model) in models_with_names]
 		self.model_names = [name for (name, _) in models_with_names]
-		self.actual_model = actual_model
-
-		self.n: int
-		try:
-			self.n = self.actual_model.n  # type: ignore
-		except AttributeError:
-			self.n = 1
-
 		self.model_count = len(self.models)
+
 		self.monte_carlo_count = monte_carlo_count
 		self.monte_carlo_cycles = monte_carlo_cycles
 		self.target_success = target_success
 		self.max_monte_carlo_cycles_steps = max_monte_carlo_cycles_steps
-		self.run_count = run_count
-		self.low_error = low_error
-		self.high_error = high_error
-		if pairs_low_error is None:
-			self.pairs_low_error = self.low_error
-		else:
-			self.pairs_low_error = pairs_low_error
-		if pairs_high_error is None:
-			self.pairs_high_error = self.high_error
-		else:
-			self.pairs_high_error = pairs_high_error
 
 		self.csv_fields = []
-		for i in range(self.n):
-			self.csv_fields.extend(
-				[
-					f"dipole_moment_{i+1}",
-					f"dipole_location_{i+1}",
-					f"dipole_frequency_{i+1}",
-				]
-			)
+
 		self.compensate_zeros = True
 		self.chunksize = chunksize
 		for name in self.model_names:
 			self.csv_fields.extend([f"{name}_success", f"{name}_count", f"{name}_prob"])
 
-		self.probabilities_no_pairs = [1 / self.model_count] * self.model_count
-		self.probabilities_pairs = [1 / self.model_count] * self.model_count
+		# for now initialise priors as uniform.
+		self.probabilities = [1 / self.model_count] * self.model_count
 
 		timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-		self.filename_pairs = f"{timestamp}-{filename_slug}.simulpairs.yespairs.csv"
-		self.filename_no_pairs = f"{timestamp}-{filename_slug}.simulpairs.noopairs.csv"
 
-		self.max_frequency = max_frequency
+		ff_string = "fast_filter"
 
-		if end_threshold is not None:
-			if 0 < end_threshold < 1:
-				self.end_threshold: float = end_threshold
-				self.use_end_threshold = True
-				_logger.info(f"Will abort early, at {self.end_threshold}.")
-			else:
-				raise ValueError(
-					f"end_threshold should be between 0 and 1, but is actually {end_threshold}"
-				)
+		self.filename = f"{timestamp}-{filename_slug}.realdata.{ff_string}.bayesrun.csv"
+		self.initial_seed = initial_seed
+
+		self.cap_core_count = cap_core_count
 
 	def go(self) -> None:
-		with open(self.filename_pairs, "a", newline="") as outfile:
+		with open(self.filename, "a", newline="") as outfile:
 			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
 			writer.writeheader()
-		with open(self.filename_no_pairs, "a", newline="") as outfile:
-			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
-			writer.writeheader()
-
-		for run in range(1, self.run_count + 1):
 
-			# Generate the actual dipoles
-			actual_dipoles = self.actual_model.get_dipoles(self.max_frequency)
+		(
+			lows,
+			highs,
+		) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
+			self.measurements
+		)
 
-			dots = actual_dipoles.get_percent_range_dot_measurements(
-				self.dot_inputs, self.low_error, self.high_error
-			)
+		pair_lows = None
+		pair_highs = None
+		if self.use_pair_measurements:
 			(
-				lows,
-				highs,
+				pair_lows,
+				pair_highs,
 			) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
-				dots
+				self.pair_measurements
 			)
 
-			pair_lows, pair_highs = (None, None)
-			pair_measurements = actual_dipoles.get_percent_range_dot_pair_measurements(
-				self.dot_pair_inputs, self.pairs_low_error, self.pairs_high_error
-			)
+		pair_phase_lows = None
+		pair_phase_highs = None
+		if self.use_pair_phase_measurements:
 			(
-				pair_lows,
-				pair_highs,
+				pair_phase_lows,
+				pair_phase_highs,
 			) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
-				pair_measurements
+				self.pair_phase_measurements
 			)
 
-			_logger.info(f"Going to work on dipole at {actual_dipoles.dipoles}")
-
-			# define a new seed sequence for each run
-			seed_sequence = numpy.random.SeedSequence(run)
+		# define a new seed sequence for each run
+		seed_sequence = numpy.random.SeedSequence(self.initial_seed)
 
-			results_pairs = []
-			results_no_pairs = []
-			_logger.debug("Going to iterate over models now")
-			for model_count, model in enumerate(self.models):
-				_logger.debug(f"Doing model #{model_count}")
-
-				core_count = multiprocessing.cpu_count() - 1 or 1
-				with multiprocessing.Pool(core_count) as pool:
-					cycle_count = 0
-					cycle_success_pairs = 0
-					cycle_success_no_pairs = 0
-					cycles = 0
-					while (cycles < self.max_monte_carlo_cycles_steps) and (
-						min(cycle_success_pairs, cycle_success_no_pairs)
-						<= self.target_success
-					):
-						_logger.debug(f"Starting cycle {cycles}")
-
-						cycles += 1
-						current_success_pairs = 0
-						current_success_no_pairs = 0
-						cycle_count += self.monte_carlo_count * self.monte_carlo_cycles
-
-						# generate a seed from the sequence for each core.
-						# note this needs to be inside the loop for monte carlo cycle steps!
-						# that way we get more stuff.
-
-						seeds = seed_sequence.spawn(self.monte_carlo_cycles)
-						_logger.debug(f"Creating {self.monte_carlo_cycles} seeds")
-						current_success_both = numpy.array(
-							sum(
-								pool.imap_unordered(
-									get_a_simul_result_using_pairs,
-									[
-										(
-											model,
-											self.dot_inputs_array,
-											self.dot_pair_inputs_array,
-											lows,
-											highs,
-											pair_lows,
-											pair_highs,
-											self.monte_carlo_count,
-											self.monte_carlo_cycles,
-											self.max_frequency,
-											seed,
-										)
-										for seed in seeds
-									],
-									self.chunksize,
-								)
+		results = []
+		_logger.debug("Going to iterate over models now")
+		core_count = multiprocessing.cpu_count() - 1 or 1
+		if (self.cap_core_count >= 1) and (self.cap_core_count < core_count):
+			core_count = self.cap_core_count
+		_logger.info(f"Using {core_count} cores")
+		for model_count, (model, model_name) in enumerate(
+			zip(self.models, self.model_names)
+		):
+			_logger.debug(f"Doing model #{model_count}: {model_name}")
+			with multiprocessing.Pool(core_count) as pool:
+				cycle_count = 0
+				cycle_success = 0
+				cycles = 0
+				while (cycles < self.max_monte_carlo_cycles_steps) and (
+					cycle_success <= self.target_success
+				):
+					_logger.debug(f"Starting cycle {cycles}")
+					cycles += 1
+					current_success = 0
+					cycle_count += self.monte_carlo_count * self.monte_carlo_cycles
+
+					# generate a seed from the sequence for each core.
+					# note this needs to be inside the loop for monte carlo cycle steps!
+					# that way we get more stuff.
+					seeds = seed_sequence.spawn(self.monte_carlo_cycles)
+
+					if self.use_pair_measurements:
+						_logger.debug("using pair measurements")
+						current_success = sum(
+							pool.imap_unordered(
+								get_a_result_fast_filter_pairs,
+								[
+									(
+										model,
+										self.dot_inputs_array,
+										lows,
+										highs,
+										self.dot_pair_inputs_array,
+										pair_lows,
+										pair_highs,
+										self.monte_carlo_count,
+										seed,
+									)
+									for seed in seeds
+								],
+								self.chunksize,
+							)
+						)
+					elif self.use_pair_phase_measurements:
+						_logger.debug("using pair phase measurements")
+						_logger.debug("specifically using tarucha")
+						current_success = sum(
+							pool.imap_unordered(
+								get_a_result_fast_filter_tarucha_spin_qubit_pair_phase_only,
+								[
+									(
+										model,
+										self.dot_pair_inputs_array,
+										pair_phase_lows,
+										pair_phase_highs,
+										self.monte_carlo_count,
+										seed,
+									)
+									for seed in seeds
+								],
+								self.chunksize,
 							)
 						)
-						current_success_no_pairs = current_success_both[0]
-						current_success_pairs = current_success_both[1]
+					else:
 
-						cycle_success_no_pairs += current_success_no_pairs
-						cycle_success_pairs += current_success_pairs
-						_logger.debug(
-							f"(pair, no_pair) successes are {(cycle_success_pairs, cycle_success_no_pairs)}"
+						current_success = sum(
+							pool.imap_unordered(
+								get_a_result_fast_filter,
+								[
+									(
+										model,
+										self.dot_inputs_array,
+										lows,
+										highs,
+										self.monte_carlo_count,
+										seed,
+									)
+									for seed in seeds
+								],
+								self.chunksize,
+							)
 						)
-					results_pairs.append((cycle_count, cycle_success_pairs))
-					results_no_pairs.append((cycle_count, cycle_success_no_pairs))
 
-			_logger.debug("Done, constructing output now")
-			row_pairs = {
-				"dipole_moment_1": actual_dipoles.dipoles[0].p,
-				"dipole_location_1": actual_dipoles.dipoles[0].s,
-				"dipole_frequency_1": actual_dipoles.dipoles[0].w,
-			}
-			row_no_pairs = {
-				"dipole_moment_1": actual_dipoles.dipoles[0].p,
-				"dipole_location_1": actual_dipoles.dipoles[0].s,
-				"dipole_frequency_1": actual_dipoles.dipoles[0].w,
-			}
-			for i in range(1, self.n):
-				try:
-					current_dipoles = actual_dipoles.dipoles[i]
-					row_pairs[f"dipole_moment_{i+1}"] = current_dipoles.p
-					row_pairs[f"dipole_location_{i+1}"] = current_dipoles.s
-					row_pairs[f"dipole_frequency_{i+1}"] = current_dipoles.w
-					row_no_pairs[f"dipole_moment_{i+1}"] = current_dipoles.p
-					row_no_pairs[f"dipole_location_{i+1}"] = current_dipoles.s
-					row_no_pairs[f"dipole_frequency_{i+1}"] = current_dipoles.w
-				except IndexError:
-					_logger.info(f"Not writing anymore, saw end after {i}")
-					break
-
-			successes_pairs: List[float] = []
-			successes_no_pairs: List[float] = []
-			counts: List[int] = []
-			for model_index, (
-				name,
-				(count_pair, result_pair),
-				(count_no_pair, result_no_pair),
-			) in enumerate(zip(self.model_names, results_pairs, results_no_pairs)):
-
-				row_pairs[f"{name}_success"] = result_pair
-				row_pairs[f"{name}_count"] = count_pair
-				successes_pairs.append(max(result_pair, 0.5))
-
-				row_no_pairs[f"{name}_success"] = result_no_pair
-				row_no_pairs[f"{name}_count"] = count_no_pair
-				successes_no_pairs.append(max(result_no_pair, 0.5))
-
-				counts.append(count_pair)
-
-			success_weight_pair = sum(
-				[
-					(succ / count) * prob
-					for succ, count, prob in zip(
-						successes_pairs, counts, self.probabilities_pairs
-					)
-				]
-			)
-			success_weight_no_pair = sum(
-				[
-					(succ / count) * prob
-					for succ, count, prob in zip(
-						successes_no_pairs, counts, self.probabilities_no_pairs
-					)
-				]
-			)
-			new_probabilities_pair = [
-				(succ / count) * old_prob / success_weight_pair
-				for succ, count, old_prob in zip(
-					successes_pairs, counts, self.probabilities_pairs
-				)
-			]
-			new_probabilities_no_pair = [
-				(succ / count) * old_prob / success_weight_no_pair
-				for succ, count, old_prob in zip(
-					successes_no_pairs, counts, self.probabilities_no_pairs
-				)
+					cycle_success += current_success
+					_logger.debug(f"current running successes: {cycle_success}")
+				results.append((cycle_count, cycle_success))
+
+		_logger.debug("Done, constructing output now")
+		row: Dict[str, Union[int, float, str]] = {}
+
+		successes: List[float] = []
+		counts: List[int] = []
+		for model_index, (name, (count, result)) in enumerate(
+			zip(self.model_names, results)
+		):
+
+			row[f"{name}_success"] = result
+			row[f"{name}_count"] = count
+			successes.append(max(result, 0.5))
+			counts.append(count)
+
+		success_weight = sum(
+			[
+				(succ / count) * prob
+				for succ, count, prob in zip(successes, counts, self.probabilities)
 			]
-			self.probabilities_pairs = new_probabilities_pair
-			self.probabilities_no_pairs = new_probabilities_no_pair
-			for name, probability_pair, probability_no_pair in zip(
-				self.model_names, self.probabilities_pairs, self.probabilities_no_pairs
-			):
-				row_pairs[f"{name}_prob"] = probability_pair
-				row_no_pairs[f"{name}_prob"] = probability_no_pair
-			_logger.debug(row_pairs)
-			_logger.debug(row_no_pairs)
-
-			with open(self.filename_pairs, "a", newline="") as outfile:
-				writer = csv.DictWriter(
-					outfile, fieldnames=self.csv_fields, dialect="unix"
-				)
-				writer.writerow(row_pairs)
-			with open(self.filename_no_pairs, "a", newline="") as outfile:
-				writer = csv.DictWriter(
-					outfile, fieldnames=self.csv_fields, dialect="unix"
-				)
-				writer.writerow(row_no_pairs)
+		)
+		new_probabilities = [
+			(succ / count) * old_prob / success_weight
+			for succ, count, old_prob in zip(successes, counts, self.probabilities)
+		]
+		self.probabilities = new_probabilities
+		for name, probability in zip(self.model_names, self.probabilities):
+			row[f"{name}_prob"] = probability
+		_logger.info(row)
 
-			if self.use_end_threshold:
-				max_prob = min(
-					max(self.probabilities_pairs), max(self.probabilities_no_pairs)
-				)
-				if max_prob > self.end_threshold:
-					_logger.info(
-						f"Aborting early, because {max_prob} is greater than {self.end_threshold}"
-					)
-					break
+		with open(self.filename, "a", newline="") as outfile:
+			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
+			writer.writerow(row)
```

### Comparing `deepdog-1.0.1/deepdog/cli/probs/args.py` & `deepdog-1.1.0/deepdog/cli/probs/args.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/deepdog/cli/probs/dicts.py` & `deepdog-1.1.0/deepdog/cli/probs/dicts.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/deepdog/cli/probs/main.py` & `deepdog-1.1.0/deepdog/cli/probs/main.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/deepdog/direct_monte_carlo/direct_mc.py` & `deepdog-1.1.0/deepdog/direct_monte_carlo/direct_mc.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 	max_monte_carlo_cycles_steps: int = 10
 	monte_carlo_seed: int = 1234
 	write_successes_to_file: bool = False
 	tag: str = ""
 	cap_core_count: int = 0  # 0 means cap at num cores - 1
 	chunk_size: int = 50
 	write_bayesrun_file = True
+	bayesrun_file_timestamp = True
 	# chunk size of some kind
 
 
 # Aliasing dict as a generic data container
 DirectMonteCarloData = NewType("DirectMonteCarloData", Dict[str, Any])
 
 
@@ -280,17 +281,22 @@
 						likelihood=total_success / total_count,
 						model_name=model_name_pair[0],
 					)
 				)
 
 		if self.config.write_bayesrun_file:
 
+			if self.config.bayesrun_file_timestamp:
+				timestamp_str = f"{timestamp}-"
+			else:
+				timestamp_str = ""
 			filename = (
-				f"{timestamp}-{self.config.tag}.realdata.fast_filter.bayesrun.csv"
+				f"{timestamp_str}{self.config.tag}.realdata.fast_filter.bayesrun.csv"
 			)
+
 			_logger.info(f"Going to write to file [{filename}]")
 			# row: Dict[str, Union[int, float, str]] = {}
 			row = {}
 
 			num_models = len(self.model_name_pairs)
 			success_weight = sum(
 				[
```

### Comparing `deepdog-1.0.1/deepdog/indexify/__init__.py` & `deepdog-1.1.0/deepdog/indexify/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.1.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 02:08:52 2024 UTC, .py size: 1700 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b4f5 3266 a406 0000  a.........2f....
+00000000: 610d 0d0a 0000 0000 8d64 3466 a406 0000  a........d4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6503 a005 6506 a101 5a07 6403 6404  Z.e...e...Z.d.d.
 00000060: 8400 5a08 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000070: 5a09 6402 5300 2907 7ac7 0a50 726f 6261  Z.d.S.).z..Proba
@@ -41,15 +41,15 @@
 00000280: 8302 8301 5600 0100 7102 6400 5300 a901  ....V...q.d.S...
 00000290: 4e29 03da 0464 6963 74da 037a 6970 da04  N)...dict..zip..
 000002a0: 6b65 7973 2902 da02 2e30 da01 78a9 01da  keys)....0..x...
 000002b0: 0564 6963 7473 a900 fa56 2f68 6f6d 652f  .dicts...V/home/
 000002c0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 000002d0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 000002e0: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-000002f0: 302e 312f 6465 6570 646f 672f 696e 6465  0.1/deepdog/inde
+000002f0: 312e 302f 6465 6570 646f 672f 696e 6465  1.0/deepdog/inde
 00000300: 7869 6679 2f5f 5f69 6e69 745f 5f2e 7079  xify/__init__.py
 00000310: da09 3c67 656e 6578 7072 3e17 0000 00f3  ..<genexpr>.....
 00000320: 0000 0000 7a20 5f64 6963 745f 7072 6f64  ....z _dict_prod
 00000330: 7563 742e 3c6c 6f63 616c 733e 2e3c 6765  uct.<locals>.<ge
 00000340: 6e65 7870 723e 2904 da04 6c69 7374 da09  nexpr>)...list..
 00000350: 6974 6572 746f 6f6c 73da 0770 726f 6475  itertools..produ
 00000360: 6374 da06 7661 6c75 6573 7208 0000 0072  ct..valuesr....r
```

### Comparing `deepdog-1.0.1/deepdog/results/__init__.py` & `deepdog-1.1.0/deepdog/results/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/deepdog/results/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.1.0/deepdog/results/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 02:08:52 2024 UTC, .py size: 4858 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b4f5 3266 fa12 0000  a.........2f....
+00000000: 610d 0d0a 0000 0000 8d64 3466 fa12 0000  a........d4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6503 a008 6509 a101 5a0a  d.l.Z.e...e...Z.
 00000070: 6402 5a0b 6403 6701 5a0c 6404 6405 6702  d.Z.d.g.Z.d.d.g.
@@ -59,15 +59,15 @@
 000003a0: 6c6e 616d 655f 5fda 0373 7472 da0f 5f5f  lname__..str..__
 000003b0: 616e 6e6f 7461 7469 6f6e 735f 5fda 0770  annotations__..p
 000003c0: 6174 686c 6962 da04 5061 7468 a900 720d  athlib..Path..r.
 000003d0: 0000 0072 0d00 0000 fa55 2f68 6f6d 652f  ...r.....U/home/
 000003e0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 000003f0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 00000400: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-00000410: 302e 312f 6465 6570 646f 672f 7265 7375  0.1/deepdog/resu
+00000410: 312e 302f 6465 6570 646f 672f 7265 7375  1.0/deepdog/resu
 00000420: 6c74 732f 5f5f 696e 6974 5f5f 2e70 7972  lts/__init__.pyr
 00000430: 0200 0000 1700 0000 7306 0000 000a 0208  ........s.......
 00000440: 0108 0172 0200 0000 6300 0000 0000 0000  ...r....c.......
 00000450: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 00000460: 0073 3000 0000 6500 5a01 6400 5a02 6401  .s0...e.Z.d.Z.d.
 00000470: 5a03 6504 6a05 6506 6506 6602 1900 6402  Z.e.j.e.e.f...d.
 00000480: 9c01 6403 6404 8404 5a07 6405 6406 8400  ..d.d...Z.d.d...
```

### Comparing `deepdog-1.0.1/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-1.1.0/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-1.1.0/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.0.1/pyproject.toml` & `deepdog-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "deepdog"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
-pdme = "^1.0.0"
+pdme = "^1.2.0"
 numpy = "1.22.3"
 scipy = "1.10"
 tqdm = "^4.66.2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
```

