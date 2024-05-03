# Comparing `tmp/nrw-0.6.tar.gz` & `tmp/nrw-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrw-0.6.tar", last modified: Tue Oct 10 04:55:21 2023, max compression
+gzip compressed data, was "/home/mbowman/code/nix_random_wallpaper/dist/.tmp-15fd1lpg/nrw-0.7.tar", last modified: Fri May  3 00:09:50 2024, max compression
```

## Comparing `nrw-0.6.tar` & `nrw-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mbowman   (9001) mbowman   (9001)        0 2023-10-10 04:55:21.062524 nrw-0.6/
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)     1070 2023-10-10 03:21:49.000000 nrw-0.6/LICENSE
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)     6082 2023-10-10 04:55:21.062524 nrw-0.6/PKG-INFO
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)     4201 2022-05-31 05:12:11.000000 nrw-0.6/README.md
-drwxr-xr-x   0 mbowman   (9001) mbowman   (9001)        0 2023-10-10 04:55:21.062524 nrw-0.6/nrw/
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)        0 2022-01-12 00:22:57.000000 nrw-0.6/nrw/__init__.py
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)      915 2022-01-12 00:22:57.000000 nrw-0.6/nrw/config.yaml
--rwxr-xr-x   0 mbowman   (9001) mbowman   (9001)    10270 2023-10-10 04:40:53.000000 nrw-0.6/nrw/nix_random_wallpaper.py
-drwxr-xr-x   0 mbowman   (9001) mbowman   (9001)        0 2023-10-10 04:55:21.062524 nrw-0.6/nrw.egg-info/
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)     6082 2023-10-10 04:55:21.000000 nrw-0.6/nrw.egg-info/PKG-INFO
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)      256 2023-10-10 04:55:21.000000 nrw-0.6/nrw.egg-info/SOURCES.txt
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)        1 2023-10-10 04:55:21.000000 nrw-0.6/nrw.egg-info/dependency_links.txt
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)       54 2023-10-10 04:55:21.000000 nrw-0.6/nrw.egg-info/entry_points.txt
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)       45 2023-10-10 04:55:21.000000 nrw-0.6/nrw.egg-info/requires.txt
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)        4 2023-10-10 04:55:21.000000 nrw-0.6/nrw.egg-info/top_level.txt
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)      836 2023-10-10 04:38:06.000000 nrw-0.6/pyproject.toml
--rw-r--r--   0 mbowman   (9001) mbowman   (9001)       38 2023-10-10 04:55:21.062524 nrw-0.6/setup.cfg
+drwxr-xr-x   0 mbowman   (9001) mbowman   (9001)        0 2024-05-03 00:09:50.000000 nrw-0.7/
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)     1070 2023-10-10 03:21:49.000000 nrw-0.7/LICENSE
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)     6539 2024-05-03 00:09:50.000000 nrw-0.7/PKG-INFO
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)     4748 2024-05-02 05:44:23.000000 nrw-0.7/README.md
+drwxr-xr-x   0 mbowman   (9001) mbowman   (9001)        0 2024-05-03 00:09:50.000000 nrw-0.7/nrw/
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)        0 2022-01-12 00:22:57.000000 nrw-0.7/nrw/__init__.py
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)      925 2024-05-02 05:35:32.000000 nrw-0.7/nrw/config.yaml
+-rwxr-xr-x   0 mbowman   (9001) mbowman   (9001)    14564 2024-05-02 05:35:32.000000 nrw-0.7/nrw/nix_random_wallpaper.py
+drwxr-xr-x   0 mbowman   (9001) mbowman   (9001)        0 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)     6539 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/PKG-INFO
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)      256 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/SOURCES.txt
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)        1 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/dependency_links.txt
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)       54 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/entry_points.txt
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)       45 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/requires.txt
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)        4 2024-05-03 00:09:50.000000 nrw-0.7/nrw.egg-info/top_level.txt
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)      836 2024-05-03 00:08:25.000000 nrw-0.7/pyproject.toml
+-rw-r--r--   0 mbowman   (9001) mbowman   (9001)       38 2024-05-03 00:09:50.000000 nrw-0.7/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nrw-0.6/LICENSE` & `nrw-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nrw-0.6/PKG-INFO` & `nrw-0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrw
-Version: 0.6
+Version: 0.7
 Summary: A simple program that sets random images as desktop wallpaper in *nix operating systems.
 Author-email: Marcus Bowman <miliarch.mb@gmail.com>
 Maintainer-email: Marcus Bowman <miliarch.mb@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Marcus Bowman
         
@@ -28,17 +28,14 @@
         
 Project-URL: Documentation, https://github.com/miliarch/nrw
 Project-URL: Repository, https://github.com/miliarch/nrw.git
 Keywords: gnome,cinnamon,nitrogen,linux,random,wallpaper,desktop,background,unsplash
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow>=9.4.0
-Requires-Dist: PyYAML>=5.4.1
-Requires-Dist: requests>=2.26.0
 
 # Nix Random Wallpaper
 
 A simple program that sets random wallpaper images as desktop backgrounds in nix based operating systems / window managers. It fetches images from a local directory or Unsplash, composes a new image to match display size and arrangement, and sets the new image as the desktop background.
 
 This project was forked from [Gnome Random Wallpaper](https://github.com/miliarch/gnome_random_wallpaper), which while great at its original limited scope, is no longer maintained.
 
@@ -56,15 +53,15 @@
 * The user will configure some external scheduler to prompt the `nrw` command to run in the background
 * The user doesn't usually want to keep the generated wallpaper images forever
   * The last image that was generated is replaced by the newly generated image
   * The default output directory is `/tmp/random` - `/tmp` is commonly a tmpfs filesystem and exists only in memory (while the system remains powered on)
     * Note: The default output directory can and probably should be changed to a non-volatile location in [configuration](#configuration). Specifying a non-volatile directory will prevent temporary auto-selection of a system default wallpaper by the window manager on login after a fresh boot cycle, which can be disorienting.
 * The user won't interact directly with the program often, making command line argument support unnecessary
 
-Simply running `nrw` will fetch images from either the [Unsplash API](https://source.unsplash.com/) or the image directory (`images_dir`) defined in configuration, resize and compose the images on a spanned canvas matching your current display arrangement, save the resulting wallpaper image to the output directory (`output_dir`), and update your desktop background.
+Simply running `nrw` will fetch images from either the [Unsplash API](https://source.unsplash.com/) or the image directory (`images_dir`) defined in configuration, then prepare and set the wallpaper based on the configured setter. In xorg, all setters resize and compose the images on a spanned canvas matching your current display arrangement, save the resulting wallpaper image to the output directory (`output_dir`), and update your desktop background. In wayland (currently only hyprland), images are placed on their own right-sized canvases, saved separately, and update the desktop background individually on each screen.
 
 Some suggested steps to take in your environment:
 * Configure a cron job or timer of some sort to run `nrw` at regular intervals (every 15 minutes works well for me - `*/15 * * * * /path/to/nrw`)
 * Configure a Startup Application to run `nrw` on login
 
 ## Installation
 
@@ -96,22 +93,25 @@
 
 Vertical arrangements, including mixed vertical/horizontal arrangements, are currently unsupported. Support may be implemented in the future.
 
 ## Tested configurations
 
 ### Window managers
 
-* Cinnamon 5.0.5-5.0.7
-* awesome v4.3
+* Cinnamon 5.0.5-5.0.7 (xorg)
+* awesome v4.3 (xorg)
+* hyprland v0.39.1 (wayland)
 
 ### Wallpaper setters
 
-* gnome (via gsettings)
-* [nitrogen](https://github.com/l3ib/nitrogen) (recommended)
+* gnome (via gsettings; xorg only)
+* [nitrogen](https://github.com/l3ib/nitrogen) (recommended for xorg)
+* [hyprpaper](https://github.com/hyprwm/hyprpaper) (hyprland/wayland only)
 
 ### Resolutions
 * 1920x1080
 * 2560x1440
 * 3840x2160
 
 ### Display arrangements
 * Dual monitor, landscape orientation, horizontal arrangement (side-by-side)
+* In hyprland/wayland, images are set independently by active monitor instead of being placed on a large canvas; any arrangement should be supported
```

### Comparing `nrw-0.6/README.md` & `nrw-0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 * The user will configure some external scheduler to prompt the `nrw` command to run in the background
 * The user doesn't usually want to keep the generated wallpaper images forever
   * The last image that was generated is replaced by the newly generated image
   * The default output directory is `/tmp/random` - `/tmp` is commonly a tmpfs filesystem and exists only in memory (while the system remains powered on)
     * Note: The default output directory can and probably should be changed to a non-volatile location in [configuration](#configuration). Specifying a non-volatile directory will prevent temporary auto-selection of a system default wallpaper by the window manager on login after a fresh boot cycle, which can be disorienting.
 * The user won't interact directly with the program often, making command line argument support unnecessary
 
-Simply running `nrw` will fetch images from either the [Unsplash API](https://source.unsplash.com/) or the image directory (`images_dir`) defined in configuration, resize and compose the images on a spanned canvas matching your current display arrangement, save the resulting wallpaper image to the output directory (`output_dir`), and update your desktop background.
+Simply running `nrw` will fetch images from either the [Unsplash API](https://source.unsplash.com/) or the image directory (`images_dir`) defined in configuration, then prepare and set the wallpaper based on the configured setter. In xorg, all setters resize and compose the images on a spanned canvas matching your current display arrangement, save the resulting wallpaper image to the output directory (`output_dir`), and update your desktop background. In wayland (currently only hyprland), images are placed on their own right-sized canvases, saved separately, and update the desktop background individually on each screen.
 
 Some suggested steps to take in your environment:
 * Configure a cron job or timer of some sort to run `nrw` at regular intervals (every 15 minutes works well for me - `*/15 * * * * /path/to/nrw`)
 * Configure a Startup Application to run `nrw` on login
 
 ## Installation
 
@@ -58,22 +58,25 @@
 
 Vertical arrangements, including mixed vertical/horizontal arrangements, are currently unsupported. Support may be implemented in the future.
 
 ## Tested configurations
 
 ### Window managers
 
-* Cinnamon 5.0.5-5.0.7
-* awesome v4.3
+* Cinnamon 5.0.5-5.0.7 (xorg)
+* awesome v4.3 (xorg)
+* hyprland v0.39.1 (wayland)
 
 ### Wallpaper setters
 
-* gnome (via gsettings)
-* [nitrogen](https://github.com/l3ib/nitrogen) (recommended)
+* gnome (via gsettings; xorg only)
+* [nitrogen](https://github.com/l3ib/nitrogen) (recommended for xorg)
+* [hyprpaper](https://github.com/hyprwm/hyprpaper) (hyprland/wayland only)
 
 ### Resolutions
 * 1920x1080
 * 2560x1440
 * 3840x2160
 
 ### Display arrangements
 * Dual monitor, landscape orientation, horizontal arrangement (side-by-side)
+* In hyprland/wayland, images are set independently by active monitor instead of being placed on a large canvas; any arrangement should be supported
```

### Comparing `nrw-0.6/nrw/config.yaml` & `nrw-0.7/nrw/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 unsplash_resolution_w: 3840  # width of images fetched from unsplash
 unsplash_resolution_h: 2160  # height of images fetched from unsplash
 unsplash_orientation: landscape  # orientation of images fetched from unsplash (https://source.unsplash.com/)
 images_dir: null  # directory containing images to select from (only needed if unsplash is false)
 output_dir: /tmp/random  # directory for output image; /tmp by default as a common in-memory filesystem
 output_image_name: wallpaper.jpg  # full name of output file (include extension)
 output_image_format: jpeg  # pillow/PIL output image file format (https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)
-wallpaper_setter: gnome  # back-end used to set wallpaper [gnome|nitrogen]
+wallpaper_setter: gnome  # back-end used to set wallpaper [gnome|nitrogen|hyprpaper]
```

### Comparing `nrw-0.6/nrw/nix_random_wallpaper.py` & `nrw-0.7/nrw/nix_random_wallpaper.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,21 +14,26 @@
 
 # Path configuration
 BASE_DIR = Path(__file__).resolve().parents[0]
 USER_HOME_PATH = Path.home()
 CONFIG_DIR = Path(f"{USER_HOME_PATH}/.config/nix_random_wallpaper")
 CONFIG_DIR.mkdir(parents=True, exist_ok=True)
 CONFIG_FILE = Path(f'{CONFIG_DIR}/config.yaml')
+SETTERS_XORG = ('gnome', 'nitrogen')
+SETTERS_WAYLAND = ('hyprpaper')
+DISPLAY_SPANNED_IMAGE_SETTERS = ('gnome', 'nitrogen')
+DISPLAY_INDEPENDENT_IMAGES_SETTERS = ('hyprpaper')
 
 
 class Display:
-    def __init__(self, resolution, offset_w, offset_h):
+    def __init__(self, resolution, offset_w, offset_h, name=None):
         self.resolution_w, self.resolution_h = map(int, resolution.split('x'))
         self.offset_w = int(offset_w)
         self.offset_h = int(offset_h)
+        self.name = name
 
 
 def calculate_canvas_dimensions(displays):
     """Calculate canvas dimensions from given Display objects
 
     Assume a horizontal layout - sum width, largest height (this can be improved)
     """
@@ -68,14 +73,23 @@
         # Return size based on display height - adjusted image width is
         # too small to fill display
         return (adjusted_width, display.resolution_h)
     # Return size based on display width in the common case
     return (display.resolution_w, adjusted_height)
 
 
+def compose_image(display, image):
+    canvas = Image.new('RGB', (display.resolution_w, display.resolution_h))
+    new_dimensions = calculate_proportional_dimensions(display, image)
+    image = image.resize(new_dimensions)
+    image = image.crop(box=calculate_crop_box(display, image))
+    canvas.paste(image, (0, 0))
+    return canvas
+
+
 def compose_images(displays, images):
     """Compose images on canvas that spans displays"""
     total_width, total_height = calculate_canvas_dimensions(displays)
     canvas = Image.new('RGB', (total_width, total_height))
     for display in displays:
         image = images.pop(0)
         new_dimensions = calculate_proportional_dimensions(display, image)
@@ -96,29 +110,38 @@
 
         # Get DBUS_SESSION_BUS_ADDRESS from environment
         cmd_str = f'grep -z DBUS_SESSION_BUS_ADDRESS /proc/{pid}/environ|cut -d= -f2-'
         cmd = run(cmd_str, shell=True, capture_output=True)
         dbus_sba = cmd.stdout.decode('utf-8').replace('\n', '').replace('\x00', '')
 
         env['DBUS_SESSION_BUS_ADDRESS'] = dbus_sba
+    if setter == 'hyprpaper':
+        # instance fe7b748eb668136dd0558b7c8279bfcd7ab4d759_1714609691:
+        cmd = run(['hyprctl', 'instances'], capture_output=True)
+        output = cmd.stdout.decode('utf-8')
+        # critical assumption that the user will only use a single hyprland instance
+        # grab first line of output, isolate signature:, strip :, left with first instance sig
+        instance_signature = output.split('\n')[0].split(' ')[-1].split(':')[0]
+        env = environ
+        env['HYPRLAND_INSTANCE_SIGNATURE'] = instance_signature
     return env
 
 
 def ensure_image_source(images_dir, unsplash):
     """Ensure that at least one valid image source is specified"""
     if images_dir:
         if not images_dir.exists() or not images_dir.is_dir():
             help_str = f"images_dir is invalid: {images_dir}"
             exit(help_str)
     elif not unsplash:
         help_str = "No file source specified, check configuration"
         exit(help_str)
 
 
-def gather_displays():
+def gather_displays_xorg():
     """Gather and return list of Display objects representing physical
     displays connected to the system
     """
 
     # Capture display resolution and arrangement information
     cmd_str = 'xrandr | grep " connected"'
     cmd = run(cmd_str, env=configure_environment(), shell=True, capture_output=True)
@@ -138,14 +161,26 @@
     if len(displays) == 0:
         help_str = 'No displays detected - environment not supported'
         exit(help_str)
 
     return displays
 
 
+def gather_displays_wayland(wallpaper_setter):
+    setter_to_cmd = {
+        'hyprpaper': ['hyprctl', 'monitors'],
+    }
+    env = configure_environment(wallpaper_setter)
+    cmd = run(setter_to_cmd[wallpaper_setter], env=env, capture_output=True)
+    output = cmd.stdout.decode('utf-8')
+    if wallpaper_setter == 'hyprpaper':
+        displays = parse_hyprctl_monitors(output)
+    return displays
+
+
 def gather_random_local_images(displays, images_dir):
     """Gather collection of random local images to match count of displays"""
     image_paths = []
     for i in range(len(displays)):
         image_paths.append(select_random_child_path(images_dir))
     return [Image.open(ip) for ip in image_paths]
 
@@ -193,20 +228,42 @@
     except IOError:
         # Config file doesn't exist - load the default
         with open(BASE_DIR.joinpath('config.yaml'), 'r') as f:
             config = yaml.load(f, Loader=yaml.FullLoader)
     return config
 
 
+def parse_hyprctl_monitors(output):
+    output_by_monitor = output.split('\n\n')[:-1]
+    displays = []
+    for monitor_output in output_by_monitor:
+        data = {}
+        for line in monitor_output.split('\n'):
+            if '\t' not in line and '(ID ' in line:
+                # Monitor DP-2 (ID 1):
+                data['name'] = line.split('Monitor ')[-1].split(' (ID')[0]
+            if ':' not in line and '@' in line:
+                # \t3840x2160@59.99700 at 3840x0
+                data['resolution'] = line.split('@')[0].split('\t')[-1]
+                offset = line.split(' ')[-1].split('x')
+                data['offset_w'], data['offset_h'] = offset
+        display = Display(data['resolution'], data['offset_w'], data['offset_h'], data['name'])
+        displays.append(display)
+    return displays
+
+
 def select_random_child_path(parent_path):
     return str(choice([x for x in Path(parent_path).glob('*')]))
 
 
-def set_wallpaper(wallpaper_setter, image_file_path):
-    wallpaper_setter(image_file_path)
+def set_wallpaper(wallpaper_setter, image_file_path, display_name=None):
+    if not display_name:
+        wallpaper_setter(image_file_path)
+    else:
+        wallpaper_setter(image_file_path, display_name)
 
 
 def set_wallpaper_gnome(image_file_path):
     # Configure environment
     env = configure_environment('gnome')
 
     # Set newly generated image as background
@@ -229,14 +286,28 @@
         'nitrogen',
         '--set-tiled',
         str(image_file_path)
     ]
     run(cmd_list, env=env, capture_output=True)
 
 
+def set_wallpaper_hyprpaper(image_file_path, display_name):
+    # Configure environment
+    env = configure_environment('hyprpaper')
+
+    # Set newly generated image as background
+    command_sequence = [
+        [f'hyprctl hyprpaper preload {image_file_path}'],
+        [f'hyprctl hyprpaper wallpaper "{display_name},{image_file_path}"'],
+        [f'hyprctl hyprpaper unload {image_file_path}'],
+    ]
+    for cmd in command_sequence:
+        run(cmd, env=env, shell=True, capture_output=True)
+
+
 def main():
     # Import config
     config = import_config()
 
     # Unsplash configuration
     unsplash = config['unsplash']
     unsplash_collections = config['unsplash_collections']
@@ -245,32 +316,34 @@
     unsplash_orientation = config['unsplash_orientation']
 
     # File path configuration
     images_dir = Path(config['images_dir']) if config['images_dir'] else None
     image_format = config['output_image_format']
     output_dir = Path(config['output_dir'])
     timestamp = datetime.now().strftime("%Y-%m-%d_%H:%M:%S")
-    temp_file = Path(f'{output_dir}/{timestamp}_nrw_out.{image_format}')
-    output_file = Path(f'{output_dir}/{config["output_image_name"]}')
 
     # Configure wallpaper setter and function mappings
     wallpaper_setter = config['wallpaper_setter']
     wallpaper_setters = {
         'gnome': set_wallpaper_gnome,
         'nitrogen': set_wallpaper_nitrogen,
+        'hyprpaper': set_wallpaper_hyprpaper,
     }
 
     # Ensure that image source has been specified
     ensure_image_source(images_dir, unsplash)
 
     # Ensure that output_dir exists
     output_dir.mkdir(parents=True, exist_ok=True)
 
     # Gather list of Display objects
-    displays = gather_displays()
+    if wallpaper_setter in SETTERS_XORG:
+        displays = gather_displays_xorg()
+    elif wallpaper_setter in SETTERS_WAYLAND:
+        displays = gather_displays_wayland(wallpaper_setter)
 
     # Sort displays by offset_w (arrangement based on offset, left to right)
     displays.sort(key=lambda x: x.offset_w)
 
     # Stage Image objects for composition
     if unsplash:
         # Fetch unsplash images
@@ -280,22 +353,54 @@
             unsplash_max_resolution_h,
             unsplash_collections,
             unsplash_orientation)
     else:
         # Fetch random local image paths
         images = gather_random_local_images(displays, images_dir)
 
-    # Compose images on canvas
-    canvas = compose_images(displays, images)
+    if wallpaper_setter in DISPLAY_SPANNED_IMAGE_SETTERS:
+        # Compose images on canvas
+        canvas = compose_images(displays, images)
+
+        # Configure file paths
+        temp_file = Path(f'{output_dir}/{timestamp}_nrw_out.{image_format}')
+        output_file = Path(f'{output_dir}/{config["output_image_name"]}')
+
+        # Save canvas to temp file
+        canvas.save(temp_file, format=image_format)
+
+        # Move temp file to output file (initial image write is slow)
+        move(temp_file, output_file)
+
+        # Set wallpaper
+        set_wallpaper(wallpaper_setters[wallpaper_setter], output_file)
+    elif wallpaper_setter in DISPLAY_INDEPENDENT_IMAGES_SETTERS:
+        for idx, display in enumerate(displays):
+
+            # Configure unique output image name
+            config_output_file_path = Path(config['output_image_name'])
+            base_name = config_output_file_path.stem
+            extension = config_output_file_path.suffix
+            filename = f'{base_name}_{idx}{extension}'
+
+            # Configure file paths
+            temp_file = Path(f'{output_dir}/{timestamp}_nrw_out{extension}')
+            output_file = Path(f'{output_dir}/{filename}')
+
+            # Select image
+            image = images[idx]
+
+            # Compose image on canvas
+            canvas = compose_image(display, image)
 
-    # Save canvas to temp file
-    canvas.save(temp_file, format=image_format)
+            # Save canvas to temp files
+            canvas.save(temp_file, format=image_format)
 
-    # Move temp file to output file (initial image write is slow)
-    move(temp_file, output_file)
+            # Move temp file to output file
+            move(temp_file, output_file)
 
-    # Set wallpaper
-    set_wallpaper(wallpaper_setters[wallpaper_setter], output_file)
+            # Set wallpaper
+            set_wallpaper(wallpaper_setters[wallpaper_setter], output_file, display.name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `nrw-0.6/nrw.egg-info/PKG-INFO` & `nrw-0.7/nrw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrw
-Version: 0.6
+Version: 0.7
 Summary: A simple program that sets random images as desktop wallpaper in *nix operating systems.
 Author-email: Marcus Bowman <miliarch.mb@gmail.com>
 Maintainer-email: Marcus Bowman <miliarch.mb@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Marcus Bowman
         
@@ -28,17 +28,14 @@
         
 Project-URL: Documentation, https://github.com/miliarch/nrw
 Project-URL: Repository, https://github.com/miliarch/nrw.git
 Keywords: gnome,cinnamon,nitrogen,linux,random,wallpaper,desktop,background,unsplash
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow>=9.4.0
-Requires-Dist: PyYAML>=5.4.1
-Requires-Dist: requests>=2.26.0
 
 # Nix Random Wallpaper
 
 A simple program that sets random wallpaper images as desktop backgrounds in nix based operating systems / window managers. It fetches images from a local directory or Unsplash, composes a new image to match display size and arrangement, and sets the new image as the desktop background.
 
 This project was forked from [Gnome Random Wallpaper](https://github.com/miliarch/gnome_random_wallpaper), which while great at its original limited scope, is no longer maintained.
 
@@ -56,15 +53,15 @@
 * The user will configure some external scheduler to prompt the `nrw` command to run in the background
 * The user doesn't usually want to keep the generated wallpaper images forever
   * The last image that was generated is replaced by the newly generated image
   * The default output directory is `/tmp/random` - `/tmp` is commonly a tmpfs filesystem and exists only in memory (while the system remains powered on)
     * Note: The default output directory can and probably should be changed to a non-volatile location in [configuration](#configuration). Specifying a non-volatile directory will prevent temporary auto-selection of a system default wallpaper by the window manager on login after a fresh boot cycle, which can be disorienting.
 * The user won't interact directly with the program often, making command line argument support unnecessary
 
-Simply running `nrw` will fetch images from either the [Unsplash API](https://source.unsplash.com/) or the image directory (`images_dir`) defined in configuration, resize and compose the images on a spanned canvas matching your current display arrangement, save the resulting wallpaper image to the output directory (`output_dir`), and update your desktop background.
+Simply running `nrw` will fetch images from either the [Unsplash API](https://source.unsplash.com/) or the image directory (`images_dir`) defined in configuration, then prepare and set the wallpaper based on the configured setter. In xorg, all setters resize and compose the images on a spanned canvas matching your current display arrangement, save the resulting wallpaper image to the output directory (`output_dir`), and update your desktop background. In wayland (currently only hyprland), images are placed on their own right-sized canvases, saved separately, and update the desktop background individually on each screen.
 
 Some suggested steps to take in your environment:
 * Configure a cron job or timer of some sort to run `nrw` at regular intervals (every 15 minutes works well for me - `*/15 * * * * /path/to/nrw`)
 * Configure a Startup Application to run `nrw` on login
 
 ## Installation
 
@@ -96,22 +93,25 @@
 
 Vertical arrangements, including mixed vertical/horizontal arrangements, are currently unsupported. Support may be implemented in the future.
 
 ## Tested configurations
 
 ### Window managers
 
-* Cinnamon 5.0.5-5.0.7
-* awesome v4.3
+* Cinnamon 5.0.5-5.0.7 (xorg)
+* awesome v4.3 (xorg)
+* hyprland v0.39.1 (wayland)
 
 ### Wallpaper setters
 
-* gnome (via gsettings)
-* [nitrogen](https://github.com/l3ib/nitrogen) (recommended)
+* gnome (via gsettings; xorg only)
+* [nitrogen](https://github.com/l3ib/nitrogen) (recommended for xorg)
+* [hyprpaper](https://github.com/hyprwm/hyprpaper) (hyprland/wayland only)
 
 ### Resolutions
 * 1920x1080
 * 2560x1440
 * 3840x2160
 
 ### Display arrangements
 * Dual monitor, landscape orientation, horizontal arrangement (side-by-side)
+* In hyprland/wayland, images are set independently by active monitor instead of being placed on a large canvas; any arrangement should be supported
```

### Comparing `nrw-0.6/pyproject.toml` & `nrw-0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nrw"
-version = "0.6"
+version = "0.7"
 description = "A simple program that sets random images as desktop wallpaper in *nix operating systems."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["gnome", "cinnamon", "nitrogen", "linux", "random", "wallpaper", "desktop", "background", "unsplash"]
 authors = [
   {name = "Marcus Bowman", email = "miliarch.mb@gmail.com"},
```

