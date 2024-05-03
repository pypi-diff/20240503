# Comparing `tmp/mutwo.timeline-0.5.0.tar.gz` & `tmp/mutwo_timeline-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.timeline-0.5.0.tar", last modified: Thu Oct 19 21:47:24 2023, max compression
+gzip compressed data, was "mutwo_timeline-0.6.0.tar", last modified: Fri May  3 14:26:46 2024, max compression
```

## Comparing `mutwo.timeline-0.5.0.tar` & `mutwo_timeline-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1890 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1279 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.854372 mutwo.timeline-0.5.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/mutwo/timeline_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12442 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_converters/timelines.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/mutwo/timeline_interfaces/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_interfaces/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24877 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_interfaces/timelines.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/mutwo/timeline_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1975 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_utilities/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/mutwo/timeline_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/mutwo/timeline_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/mutwo.timeline.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1890 2023-10-19 21:47:24.000000 mutwo.timeline-0.5.0/mutwo.timeline.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-10-19 21:47:24.000000 mutwo.timeline-0.5.0/mutwo.timeline.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-10-19 21:47:24.000000 mutwo.timeline-0.5.0/mutwo.timeline.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-10-19 21:47:24.000000 mutwo.timeline-0.5.0/mutwo.timeline.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-10-19 21:47:24.000000 mutwo.timeline-0.5.0/mutwo.timeline.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-10-19 21:47:24.858372 mutwo.timeline-0.5.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1200 2023-10-19 21:47:14.000000 mutwo.timeline-0.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.404775 mutwo_timeline-0.6.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1857 2024-05-03 14:26:46.404775 mutwo_timeline-0.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1279 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.400775 mutwo_timeline-0.6.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.400775 mutwo_timeline-0.6.0/mutwo/timeline_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12172 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_converters/timelines.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.400775 mutwo_timeline-0.6.0/mutwo/timeline_interfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_interfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25266 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_interfaces/timelines.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.400775 mutwo_timeline-0.6.0/mutwo/timeline_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1975 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_utilities/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.400775 mutwo_timeline-0.6.0/mutwo/timeline_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/mutwo/timeline_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-03 14:26:46.400775 mutwo_timeline-0.6.0/mutwo.timeline.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1857 2024-05-03 14:26:46.000000 mutwo_timeline-0.6.0/mutwo.timeline.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2024-05-03 14:26:46.000000 mutwo_timeline-0.6.0/mutwo.timeline.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-03 14:26:46.000000 mutwo_timeline-0.6.0/mutwo.timeline.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-05-03 14:26:46.000000 mutwo_timeline-0.6.0/mutwo.timeline.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-03 14:26:46.000000 mutwo_timeline-0.6.0/mutwo.timeline.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-03 14:26:46.404775 mutwo_timeline-0.6.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1170 2024-05-03 14:26:36.000000 mutwo_timeline-0.6.0/setup.py
```

### Comparing `mutwo.timeline-0.5.0/LICENSE` & `mutwo_timeline-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.timeline-0.5.0/PKG-INFO` & `mutwo_timeline-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: mutwo.timeline
-Version: 0.5.0
+Version: 0.6.0
 Summary: timeline extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.timeline
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.3.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
-Requires-Dist: numpy<2.00,>=1.18
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.timeline
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.timeline.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.timeline)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.timeline-0.5.0/README.md` & `mutwo_timeline-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.timeline-0.5.0/mutwo/timeline_converters/timelines.py` & `mutwo_timeline-0.6.0/mutwo/timeline_converters/timelines.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import random
 import typing
 
-import numpy as np
 import ranges
 
 from mutwo import core_converters
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 from mutwo import timeline_interfaces
 
 __all__ = (
     "TimeLineToEventPlacementDict",
-    "TimeLineToSimultaneousEvent",
+    "TimeLineToConcurrence",
     "TimeLineToEventPlacementTuple",
     "EventPlacementTupleToGaplessEventPlacementTuple",
     "EventPlacementTupleToSplitEventPlacementDict",
 )
 
 Tag: typing.TypeAlias = "str"
 
@@ -32,49 +32,49 @@
                 tag_to_event_placement_list[tag].append(event_placement)
         return {
             tag: tuple(event_placement_list)
             for tag, event_placement_list in tag_to_event_placement_list.items()
         }
 
 
-class TimeLineToSimultaneousEvent(core_converters.abc.Converter):
-    """Create event with SimultaneousEvent for each tag.
+class TimeLineToConcurrence(core_converters.abc.Converter):
+    """Create event with Concurrence for each tag.
 
     :param random_seed: Seed for random operation in case
         `start_or_start_range` or `end_or_end_range` of an
         :class:`mutwo.timeline_interfaces.EventPlacement` is a
-        `ranges.Range` and :class:`TimeLineToSimultaneousEvent`
+        `ranges.Range` and :class:`TimeLineToConcurrence`
         needs to pick a value within the given range.
     :type random_seed: int
 
     The main intention of this converter is to convert a
     :class:`TimeLine` into a representation which is useable
     for concrete third party converters like
     :class:`mutwo.midi_converters.EventToMidiFile`.
 
     To be successful the tagged events in the
     :class:`mutwo.timeline_interfaces.EventPlacement` in the
     :class:`mutwo.timeline_interfaces.TimeLine` which is
     converted need a specific structure: the deepest nested
     structure they can follow is:
 
-        core_events.SimultaneousEvent[
-            core_events.SequentialEvent[
-                core_events.SimpleEvent
+        core_events.Concurrence[
+            core_events.Consecution[
+                core_events.Chronon
             ]
         ]
 
     Because this will be the final structure. This clean
     ordering is necessary to be functional with various third
     party converters as e.g.
     :class:`mutwo.midi_converters.EventToMidiFile`.
     """
 
     def __init__(self, random_seed: int = 100):
-        self._random = np.random.default_rng(random_seed)
+        self._random = random.Random(random_seed)
 
     def _time_or_time_range_to_time(
         self, time_or_time_range: ranges.Range | core_parameters.abc.Duration
     ) -> core_parameters.abc.Duration:
         if isinstance(time_or_time_range, ranges.Range):
             return core_parameters.DirectDuration(
                 self._random.uniform(
@@ -90,88 +90,88 @@
             self._time_or_time_range_to_time(event_placement.start_or_start_range),
             self._time_or_time_range_to_time(event_placement.end_or_end_range),
         )
 
     def _append_to_simultaneous_event(
         self,
         start: core_parameters.abc.Duration,
-        simultaneous_event: core_events.TaggedSimultaneousEvent,
-        event_to_append: core_events.SimultaneousEvent[
-            core_events.SequentialEvent[core_events.SimpleEvent]
+        simultaneous_event: core_events.Concurrence,
+        event_to_append: core_events.Concurrence[
+            core_events.Consecution[core_events.Chronon]
         ],
     ):
         if start > (simultaneous_event_duration := simultaneous_event.duration):
-            # In case our simultaneous event is still empty, 'extend_until'
-            # will do nothing (because it only extends sequential events,
-            # but ignores simultaneous events). Therefore we need to explicitly
-            # add a sequential event before extending.
+            # In case our concurrence is still empty, 'extend_until'
+            # will do nothing (because it only extends consecutions,
+            # but ignores concurrences). Therefore we need to explicitly
+            # add a consecution before extending.
             if not simultaneous_event:
-                simultaneous_event.append(core_events.SequentialEvent([]))
+                simultaneous_event.append(core_events.Consecution([]))
             simultaneous_event.extend_until(start)
         # We have an overlap
         elif start < simultaneous_event_duration:
             # TODO(We need to check for overlaps. If we find overlaps:
             #       (a) with prohibit flag
             #       (b) with allow flag
             #
             #       (a) raise Exception
-            #       (b) check for all other SequentialEvents,
+            #       (b) check for all other Consecutions,
             #           how many are they where we don't have
             #           any conflicts? Where are they? (save in list)
-            #           If there aren't enough, add new sequential events.
-            #           Then: only append to the sequential events without
+            #           If there aren't enough, add new consecutions.
+            #           Then: only append to the consecutions without
             #           conflicts.
             # elif rest_duration < 0
             raise NotImplementedError("Overlap handler isn't implemented yet!")
 
         try:
             simultaneous_event.concatenate_by_tag(event_to_append)
         except core_utilities.NoTagError:
             simultaneous_event.concatenate_by_index(event_to_append)
 
     def _add_tagged_event_to_simultaneous_event(
         self,
         start: core_parameters.abc.Duration,
-        simultaneous_event: core_events.TaggedSimultaneousEvent,
-        tagged_event: core_events.TaggedSimpleEvent
-        | core_events.TaggedSequentialEvent
-        | core_events.TaggedSimultaneousEvent,
+        simultaneous_event: core_events.Concurrence,
+        tagged_event: core_events.Chronon
+        | core_events.Consecution
+        | core_events.Concurrence,
     ):
-        if isinstance(tagged_event, core_events.SimpleEvent):
-            tagged_event = core_events.SimultaneousEvent(
-                [core_events.SequentialEvent([tagged_event])]
+        if isinstance(tagged_event, core_events.Chronon):
+            tagged_event = core_events.Concurrence(
+                [core_events.Consecution([tagged_event])]
             )
-        elif isinstance(tagged_event, core_events.SequentialEvent):
-            tagged_event = core_events.SimultaneousEvent([tagged_event])
+        elif isinstance(tagged_event, core_events.Consecution):
+            tagged_event = core_events.Concurrence([tagged_event])
         self._append_to_simultaneous_event(start, simultaneous_event, tagged_event)
 
     def _event_placement_to_event(
         self,
         event_placement: timeline_interfaces.EventPlacement,
         start: core_parameters.abc.Duration,
         end: core_parameters.abc.Duration,
-    ) -> typing.Optional[core_events.SimultaneousEvent]:
+    ) -> typing.Optional[core_events.Concurrence]:
         event_duration = end - start
         try:
-            return event_placement.event.set("duration", event_duration, mutate=False)
-        except core_utilities.CannotSetDurationOfEmptyComplexEvent:
+            return event_placement.event.copy().set("duration", event_duration)
+        except core_utilities.CannotSetDurationOfEmptyCompound:
             return None
 
     def convert(
         self, timeline_to_convert: timeline_interfaces.TimeLine
-    ) -> core_events.SimultaneousEvent[
-        core_events.TaggedSimultaneousEvent[
-            core_events.SequentialEvent[core_events.SimpleEvent]
+    ) -> core_events.Concurrence[
+        core_events.Concurrence[
+            core_events.Consecution[core_events.Chronon]
         ]
     ]:
         duration = timeline_to_convert.duration
         tag_tuple = tuple(sorted(timeline_to_convert.tag_set))
 
         tag_to_tagged_simultaneous_event = {
-            tag: core_events.TaggedSimultaneousEvent([], tag=tag) for tag in tag_tuple
+            tag: core_events.Concurrence([], tag=tag) for tag in tag_tuple
         }
 
         timeline_to_convert.sort()
         for event_placement in timeline_to_convert.event_placement_tuple:
             start, end = self._event_placement_to_start_and_end(event_placement)
             # If the event of our event placement doesn't have any children,
             # this is `None` and we just need to ignore it.
@@ -188,15 +188,15 @@
                 )
 
         duration = duration or max(
             (e.duration for e in tag_to_tagged_simultaneous_event.values())
         )
         [e.extend_until(duration) for e in tag_to_tagged_simultaneous_event.values()]
 
-        return core_events.SimultaneousEvent(
+        return core_events.Concurrence(
             tuple(tag_to_tagged_simultaneous_event.values())
         )
 
 
 class TimeLineToEventPlacementTuple(core_converters.abc.Converter):
     """Fetch from :class:`~mutwo.timeline_interfaces.TimeLine` all :class:`~mutwo.timeline_interfaces.EventPlacement` which contains of user defined tags.
 
@@ -244,15 +244,15 @@
                     event_placement_list = tag_to_event_placement_list[event.tag]
                 except KeyError:
                     event_placement_list = []
                     tag_to_event_placement_list.update(
                         {event.tag: event_placement_list}
                     )
                 new_event_placement = event_placement.copy()
-                new_event_placement.event = core_events.SimultaneousEvent(
+                new_event_placement.event = core_events.Concurrence(
                     [new_event_placement.event[event_index]]
                 )
                 event_placement_list.append(new_event_placement)
         return {
             tag: tuple(event_placement_list)
             for tag, event_placement_list in tag_to_event_placement_list.items()
         }
@@ -269,16 +269,16 @@
         duration: typing.Optional[core_parameters.abc.Duration] = None,
     ) -> tuple[timeline_interfaces.EventPlacement, ...]:
         def add_rest(
             start: core_parameters.abc.Duration, end: core_parameters.abc.Duration
         ):
             new_event_placement_list.append(
                 timeline_interfaces.EventPlacement(
-                    core_events.SimultaneousEvent(
-                        [core_events.TaggedSimpleEvent(0, tag=tag)]
+                    core_events.Concurrence(
+                        [core_events.Chronon(0, tag=tag)]
                     ),
                     start,
                     end,
                 )
             )
 
         event_placement_list = sorted(
```

### Comparing `mutwo.timeline-0.5.0/mutwo/timeline_interfaces/__init__.py` & `mutwo_timeline-0.6.0/mutwo/timeline_interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.timeline-0.5.0/mutwo/timeline_interfaces/timelines.py` & `mutwo_timeline-0.6.0/mutwo/timeline_interfaces/timelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 import ranges
 
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 from mutwo import timeline_utilities
 
-UnspecificTime: typing.TypeAlias = "core_parameters.abc.Duration | typing.Any"
+UnspecificTime: typing.TypeAlias = core_parameters.abc.Duration.Type
 UnspecificTimeOrTimeRange: typing.TypeAlias = "UnspecificTime | ranges.Range"
 TimeOrTimeRange: typing.TypeAlias = "core_parameters.abc.Duration | ranges.Range"
 
 __all__ = (
     "EventPlacement",
     "TimeLine",
     "Conflict",
     "ConflictResolutionStrategy",
     "AlwaysLeftStrategy",
     "AlternatingStrategy",
     "TagCountStrategy",
 )
 
 
-class EventPlacement(object):
+class EventPlacement(core_utilities.MutwoObject):
     """Place any event at specific start and end times.
 
     :param event: The event to be placed on a :class:`TimeLine`.
         This needs to be filled with events with a `tag` property. Each
         child event represents a specific object (e.g. instrument or
         player) The tag is necessary to concatenate two events on a
         `TimeLine` which belong to the same object (e.g. same instrument
         or same player).
-    :type event: core_events.SimultaneousEvent[core_events.TaggedSimpleEvent | core_events.TaggedSequentialEvent | core_events.SimultaneousEvent]
+    :type event: core_events.Concurrence[core_events.Chronon | core_events.Consecution | core_events.Concurrence]
     :param start_or_start_range: Sets when the event starts. This can
         be a single :class:`mutwo.core_parameters.abc.Duration` or a
         :class:`ranges.Range` of two durations. In the second case
         the placement is flexible within the given area.
     :type start_or_start_range: UnspecificTimeOrTimeRange
     :param end_or_end_range: Sets when the event ends. This can
         be a single :class:`mutwo.core_parameters.abc.Duration` or a
@@ -54,18 +54,18 @@
 
     An :class:`EventPlacement` itself is not an event and can't be treated
     like an event.
     """
 
     def __init__(
         self,
-        event: core_events.SimultaneousEvent[
-            core_events.TaggedSimpleEvent
-            | core_events.TaggedSequentialEvent
-            | core_events.SimultaneousEvent
+        event: core_events.Concurrence[
+            core_events.Chronon
+            | core_events.Consecution
+            | core_events.Concurrence
         ],
         start_or_start_range: UnspecificTimeOrTimeRange,
         end_or_end_range: UnspecificTimeOrTimeRange,
     ):
         self.start_or_start_range = start_or_start_range
         self.end_or_end_range = end_or_end_range
         self.event = event
@@ -79,15 +79,15 @@
         self,
         unspecified_time_or_time_range: UnspecificTimeOrTimeRange,
     ) -> TimeOrTimeRange:
         # Ensure we get ranges filled with Duration objects or single
         # duration objects.
         if isinstance(unspecified_time_or_time_range, ranges.Range):
             start, end = tuple(
-                core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
+                core_parameters.abc.Duration.from_any(unknown_object)
                 for unknown_object in (
                     unspecified_time_or_time_range.start,
                     unspecified_time_or_time_range.end,
                 )
             )
             try:
                 return ranges.Range(start, end)
@@ -102,26 +102,26 @@
                 self._logger.warning(
                     timeline_utilities.TooSmallRangeWarning(
                         self, unspecified_time_or_time_range
                     )
                 )
                 return start
         else:
-            return core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
+            return core_parameters.abc.Duration.from_any(
                 unspecified_time_or_time_range
             )
 
     @staticmethod
     def _get_mean_of_time_or_time_range(
         time_or_time_range: TimeOrTimeRange,
     ) -> core_parameters.abc.Duration:
         if isinstance(time_or_time_range, ranges.Range):
             return core_parameters.DirectDuration(
                 statistics.mean(
-                    (time_or_time_range.start.duration, time_or_time_range.end.duration)
+                    (time_or_time_range.start.beat_count, time_or_time_range.end.beat_count)
                 )
             )
         else:
             return time_or_time_range
 
     @staticmethod
     def _get_extrema_of_time_or_time_range(
@@ -231,17 +231,16 @@
     # ###################################################################### #
     #                          public methods                                #
     # ###################################################################### #
 
     def is_overlapping(self, other: EventPlacement) -> bool:
         return not self.time_range.isdisjoint(other.time_range)
 
-    @core_utilities.add_copy_option
     def move_by(self, duration: UnspecificTime) -> EventPlacement:
-        duration = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
+        duration = core_parameters.abc.Duration.from_any(duration)
         self.start_or_start_range, self.end_or_end_range = (
             EventPlacement._move_time_or_time_range(time_or_time_range, duration)
             for time_or_time_range in (self.start_or_start_range, self.end_or_end_range)
         )
         return self
 
     def copy(self) -> EventPlacement:
@@ -249,15 +248,28 @@
             self.event.copy(),
             copy.copy(self.start_or_start_range),
             copy.copy(self.end_or_end_range),
         )
 
 
 @dataclasses.dataclass(frozen=True)
-class Conflict(object):
+class Conflict(core_utilities.MutwoObject):
+    """A conflict represents two overlapping :class:`EventPlacement`
+
+    :param left: The earlier :class:`EventPlacement`.
+    :type left: EventPlacement
+    :param right: The later :class:`EventPlacement`.
+    :type right: EventPlacement
+
+    Two overlapping :class:`EventPlacement` are mostly only a problem
+    if their instruments are the same. Nevertheless the precise definition
+    of a :class:`Conflict` depends on the callable passed to the 'is_conflict'
+    parameter of the :func:`TimeLine.resolve_conflicts` method.
+    """
+
     left: EventPlacement
     right: EventPlacement
 
 
 class ConflictResolutionStrategy(abc.ABC):
     """Abstract base class for overlapping solving classes.
 
@@ -339,15 +351,15 @@
         if not self._prefer_more:
             sorted_event_placement_tuple = tuple(reversed(sorted_event_placement_tuple))
 
         timeline.unregister(sorted_event_placement_tuple[0])
         return True
 
 
-class TimeLine(object):
+class TimeLine(core_utilities.MutwoObject):
     """Timeline to place events on.
 
     :param duration: If this is set to `None` the ``duration``
         property of the `TimeLine` is dynamically calculated
         (by the end times of all registered :class:`EventPlacement`.
         If the duration is not `None`, then the duration is statically
         set to this time. If the user tries to register an
@@ -362,15 +374,14 @@
     """
 
     def __init__(
         self,
         event_placement_sequence: typing.Sequence[EventPlacement] = [],
         duration: typing.Optional[UnspecificTime] = None,
     ):
-
         self._dynamic_duration = duration is None
         self._duration = duration
         self._event_placement_list: list[EventPlacement] = list(
             event_placement_sequence
         )
 
     # ###################################################################### #
@@ -449,28 +460,27 @@
         """
         # We don't use 'self._event_placement_list.index(event_placement)',
         # because this results in expensive '__eq__' calls (they are expensive,
         # because mutwo event comparison is complex).
         # 'EventPlacement' are mostly complex objects and it's difficult to
         # reproduce them, so the 'normal' API of this method expects anyway
         # that we have access to the original 'EventPlacement' (either via
-        # 'get_event_placement' or because we are iteration over
+        # 'get_event_placement' or because we are iterating over
         # 'event_placement_tuple').
         ep_id = id(event_placement)
         for i, ep in enumerate(self.event_placement_tuple):
             if id(ep) == ep_id:
                 del self._event_placement_list[i]
                 return
         raise timeline_utilities.EventPlacementNotFoundError(
             event_placement=event_placement
         )
 
-    @core_utilities.add_copy_option
-    def sort(self, mutate: bool = True) -> TimeLine:
-        """Sort :class:`EventPlacement`s by start time (and if equal by end time)."""
+    def sort(self) -> TimeLine:
+        """Sort all :class:`EventPlacement` by start time (and if equal by end time)."""
 
         self._event_placement_list.sort(
             key=lambda event_placement: (
                 event_placement.min_start,
                 event_placement.max_end,
             )
         )
```

### Comparing `mutwo.timeline-0.5.0/mutwo/timeline_utilities/exceptions.py` & `mutwo_timeline-0.6.0/mutwo/timeline_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutwo.timeline-0.5.0/mutwo.timeline.egg-info/PKG-INFO` & `mutwo_timeline-0.6.0/mutwo.timeline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: mutwo.timeline
-Version: 0.5.0
+Version: 0.6.0
 Summary: timeline extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.timeline
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.3.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
-Requires-Dist: numpy<2.00,>=1.18
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.timeline
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.timeline.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.timeline)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.timeline-0.5.0/setup.py` & `mutwo_timeline-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,13 @@
         for package in setuptools.find_namespace_packages(
             include=["mutwo.*", "mutwo_third_party.*"]
         )
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=1.3.0, <2.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
         "python-ranges>=1.2.0, <2.0.0",
-        "numpy>=1.18, <2.00",
     ],
     extras_require=extras_require,
     python_requires=">=3.10, <4",
 )
```

