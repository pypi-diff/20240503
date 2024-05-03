# Comparing `tmp/lemon8-1.3.10.tar.gz` & `tmp/lemon8-1.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon8-1.3.10.tar", max compression
+gzip compressed data, was "lemon8-1.3.11.tar", max compression
```

## Comparing `lemon8-1.3.10.tar` & `lemon8-1.3.11.tar`

### file list

```diff
@@ -1,26 +1,16 @@
--rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.10/LICENSE
--rw-r--r--   0        0        0     3772 2024-05-02 17:56:04.430031 lemon8-1.3.10/lemon8/__main__.py
--rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.10/lemon8/beep.mp3
--rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.10/lemon8/bin/FONT
--rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.10/lemon8/bin/ibm.ch8
--rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.10/lemon8/components/__init__.py
--rw-r--r--   0        0        0      260 2024-05-02 13:14:11.199127 lemon8-1.3.10/lemon8/components/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      337 2024-05-02 17:00:27.180486 lemon8-1.3.10/lemon8/components/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      346 2024-05-02 13:14:11.199127 lemon8-1.3.10/lemon8/components/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0      391 2024-05-02 17:00:27.190486 lemon8-1.3.10/lemon8/components/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0    13300 2024-05-02 13:14:11.199127 lemon8-1.3.10/lemon8/components/__pycache__/cpu.cpython-310.pyc
--rw-r--r--   0        0        0    21353 2024-05-02 17:32:51.070218 lemon8-1.3.10/lemon8/components/__pycache__/cpu.cpython-311.pyc
--rw-r--r--   0        0        0     3266 2024-05-02 13:14:11.199127 lemon8-1.3.10/lemon8/components/__pycache__/display.cpython-310.pyc
--rw-r--r--   0        0        0     5014 2024-05-02 17:32:51.070218 lemon8-1.3.10/lemon8/components/__pycache__/display.cpython-311.pyc
--rw-r--r--   0        0        0     3159 2024-05-02 17:00:27.330486 lemon8-1.3.10/lemon8/components/__pycache__/keypad.cpython-311.pyc
--rw-r--r--   0        0        0     1714 2024-05-02 17:00:27.330486 lemon8-1.3.10/lemon8/components/__pycache__/memory.cpython-311.pyc
--rw-r--r--   0        0        0     3383 2024-05-02 17:00:27.330486 lemon8-1.3.10/lemon8/components/__pycache__/opcode.cpython-311.pyc
--rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.10/lemon8/components/constants.py
--rw-r--r--   0        0        0    12155 2024-05-02 17:32:47.890218 lemon8-1.3.10/lemon8/components/cpu.py
--rw-r--r--   0        0        0     2871 2024-05-02 17:32:05.700224 lemon8-1.3.10/lemon8/components/display.py
--rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.10/lemon8/components/keypad.py
--rw-r--r--   0        0        0      739 2024-05-02 17:56:14.870029 lemon8-1.3.10/lemon8/components/memory.py
--rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.10/lemon8/components/opcode.py
--rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.10/lemon8/lemon.png
--rw-r--r--   0        0        0      537 2024-05-02 17:56:27.730028 lemon8-1.3.10/pyproject.toml
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 lemon8-1.3.10/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.11/LICENSE
+-rw-r--r--   0        0        0     1496 2024-05-03 06:52:27.999014 lemon8-1.3.11/README.md
+-rw-r--r--   0        0        0     3815 2024-05-03 06:38:22.679100 lemon8-1.3.11/lemon8/__main__.py
+-rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.11/lemon8/bin/FONT
+-rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.11/lemon8/bin/ibm.ch8
+-rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.11/lemon8/components/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.11/lemon8/components/constants.py
+-rw-r--r--   0        0        0    12202 2024-05-02 18:16:10.489865 lemon8-1.3.11/lemon8/components/cpu.py
+-rw-r--r--   0        0        0     2898 2024-05-02 18:16:58.589859 lemon8-1.3.11/lemon8/components/display.py
+-rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.11/lemon8/components/keypad.py
+-rw-r--r--   0        0        0      701 2024-05-03 06:50:15.659028 lemon8-1.3.11/lemon8/components/memory.py
+-rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.11/lemon8/components/opcode.py
+-rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.11/lemon8/static/beep.mp3
+-rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.11/lemon8/static/lemon.png
+-rw-r--r--   0        0        0      558 2024-05-03 06:47:09.249048 lemon8-1.3.11/pyproject.toml
+-rw-r--r--   0        0        0     2012 1970-01-01 00:00:00.000000 lemon8-1.3.11/PKG-INFO
```

### Comparing `lemon8-1.3.10/LICENSE` & `lemon8-1.3.11/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.10/lemon8/__main__.py` & `lemon8-1.3.11/lemon8/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import logging
-import importlib.resources as ilr
+from importlib.resources import files
+
 import pygame
 
 from .components import (CPU, INIT_LOC_CONSTANT, TICK, WAVE, Display, Keypad,
-                        Memory)
+                         Memory)
 
 logging.basicConfig(
     format="%(asctime)s:%(msecs)03d (%(levelname)s/%(module)s): %(message)s",
     level=logging.DEBUG,
     encoding="utf-8",
     datefmt="%M:%S",
 )
@@ -48,15 +49,15 @@
             display=self.display, memory=self.memory, keypad=self.keypad
         )
 
     def load_font(self) -> None:
         """
         Load Font from the `/bin/FONT` file in memory from location `0x0`
         """
-        self.memory.load_binary(ilr.open_binary("lemon8.bin", "FONT").read())
+        self.memory.load_binary(files("lemon8.bin").joinpath("FONT").read_bytes())
         logging.info(f"{TICK} Successfully loaded Fontset at location 0x0")
 
     def load_rom(self, rom: str) -> None:
         """
         Load ROM in memory from location `0x200` (512)
 
         Args:
@@ -71,15 +72,14 @@
         """
         Method representing a single tick from the emulator.
         """
         for ic in range(10):
             if not self.cpu.halt:
                 self.cpu.cycle()
                 self.cpu.sync = not ic
-
             self.display.render()
 
         self.cpu.handle_timers()
 
     def run(self) -> None:
         """
         Step through the emulation indefinitely.
@@ -106,15 +106,19 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         prog="Lemon", description="Chip-8 Virtual Machine."
     )
     parser.add_argument("rom", help="Path to the rom file.")
     parser.add_argument(
-        "-S", "--scale", help="Scale up or down the display window.", type=int, default=10
+        "-S",
+        "--scale",
+        help="Scale up or down the display window.",
+        type=int,
+        default=10,
     )
     args = parser.parse_args()
 
     lemon = Lemon(args.rom, args.scale)
 
     try:
         lemon.run()
```

### Comparing `lemon8-1.3.10/lemon8/beep.mp3` & `lemon8-1.3.11/lemon8/static/beep.mp3`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.10/lemon8/components/cpu.py` & `lemon8-1.3.11/lemon8/components/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import typing as t
+from importlib.resources import files
 from random import randint
-import importlib.resources as ir
+
 import pygame
 
 from .constants import COLUMNS, CROSS, INIT_LOC_CONSTANT, ROWS
 from .display import Display
 from .keypad import Keypad
 from .memory import Memory
 from .opcode import Opcode
@@ -59,15 +60,17 @@
             halt (bool): Flag to check if the CPU is halted.
             sync (bool): Flag to sync the display with the timer.
         """
         # devices
         self.display = display
         self.memory = memory
         self.keypad = keypad
-        self.sound: pygame.mixer.Sound = pygame.mixer.Sound(ir.open_binary("lemon8","beep.mp3"))
+        self.sound: pygame.mixer.Sound = pygame.mixer.Sound(
+            files("lemon8.static").joinpath("beep.mp3").open("rb")
+        )
         self.op: Opcode = Opcode(inst=0x0000)
 
         # registers
         self.V: t.List[int] = [0] * 16
         self.I: int = 0
         self.DT: int = 0
         self.ST: int = 0
```

### Comparing `lemon8-1.3.10/lemon8/components/display.py` & `lemon8-1.3.11/lemon8/components/display.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import typing as t
+from importlib.resources import files
 
 import pygame
-import importlib.resources as ir
+
 from .constants import COLORS, COLUMNS, ROWS
 
 pygame.init()
-img = pygame.image.load(ir.open_binary("lemon8", "lemon.png"))
+icon = pygame.image.load(files("lemon8.static").joinpath("lemon.png").open("rb"))
+
 __all__ = ("Display",)
 
 
 class Display:
     """
     Object for handling creation, rendering and deletion of the emulator
     window.
@@ -40,15 +42,15 @@
         Args:
             multiplier: Constant for scaling the window.
         """
         screen = pygame.display.set_mode(
             (COLUMNS * multiplier, ROWS * multiplier), vsync=True
         )
         pygame.display.set_caption("Lemon")
-        pygame.display.set_icon(img)
+        pygame.display.set_icon(icon)
         self = cls(screen, multiplier)
 
         return self
 
     def refresh(self) -> None:
         """
         Refresh the display using
```

### Comparing `lemon8-1.3.10/lemon8/components/keypad.py` & `lemon8-1.3.11/lemon8/components/keypad.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.10/lemon8/components/memory.py` & `lemon8-1.3.11/lemon8/components/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import importlib.resources as ilr
-
 __all__ = ("Memory",)
 
 
 class Memory:
     """
     Primary Memory of the CPU.
     """
@@ -17,15 +15,15 @@
         Attributes:
             space (bytearray): A bytearray of size 4096 virtually representing CHP-8 memory.
         """
         self.space: bytearray = bytearray(4096)
 
     def load_binary(self, binary: bytes, offset: int = 0) -> None:
         """
-        Load file onto the RAM.
+        Load bytes onto the RAM.
 
         Arguments:
-            binary: Path to the binary.
+            binary: a bytes object.
             offset: From where to start loading the elements of the binary.
         """
         for i, data in enumerate(binary):
             self.space[i + offset] = data
```

### Comparing `lemon8-1.3.10/lemon8/components/opcode.py` & `lemon8-1.3.11/lemon8/components/opcode.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.10/lemon8/lemon.png` & `lemon8-1.3.11/lemon8/static/lemon.png`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.10/pyproject.toml` & `lemon8-1.3.11/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "lemon8"
-version = "1.3.10"
+version = "1.3.11"
 description = "A CHIP-8 emulator written in Python."
 authors = ["mooncell07 <80042274+mooncell07@users.noreply.github.com>"]
 license = "MIT"
+readme = "README.md"
 documentation = "https://mooncell07.github.io/lemon.pie/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pygame = "^2.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

