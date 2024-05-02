# Comparing `tmp/usports_basketball-0.0.3.tar.gz` & `tmp/usports_basketball-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usports_basketball-0.0.3.tar", last modified: Tue Apr 30 06:46:13 2024, max compression
+gzip compressed data, was "usports_basketball-1.0.0.tar", last modified: Thu May  2 22:05:04 2024, max compression
```

## Comparing `usports_basketball-0.0.3.tar` & `usports_basketball-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:46:13.074633 usports_basketball-0.0.3/
--rw-rw-rw-   0        0        0     1088 2024-04-04 21:08:28.000000 usports_basketball-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3209 2024-04-30 06:46:13.072513 usports_basketball-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2552 2024-04-30 04:50:17.000000 usports_basketball-0.0.3/README.md
--rw-rw-rw-   0        0        0      942 2024-04-30 06:45:09.000000 usports_basketball-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 06:46:13.075636 usports_basketball-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-30 05:47:08.000000 usports_basketball-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:46:13.044064 usports_basketball-0.0.3/test/
--rw-rw-rw-   0        0        0     1473 2024-04-30 06:08:30.000000 usports_basketball-0.0.3/test/test.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:46:13.046877 usports_basketball-0.0.3/usports_basketball/
--rw-rw-rw-   0        0        0     1419 2024-04-26 05:07:23.000000 usports_basketball-0.0.3/usports_basketball/__init__.py
--rw-rw-rw-   0        0        0    11109 2024-04-26 04:40:02.000000 usports_basketball-0.0.3/usports_basketball/player_stats.py
--rw-rw-rw-   0        0        0    15251 2024-04-26 04:38:24.000000 usports_basketball-0.0.3/usports_basketball/team_stats.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:46:13.069518 usports_basketball-0.0.3/usports_basketball.egg-info/
--rw-rw-rw-   0        0        0     3209 2024-04-30 06:46:13.000000 usports_basketball-0.0.3/usports_basketball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-04-30 06:46:13.000000 usports_basketball-0.0.3/usports_basketball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:46:13.000000 usports_basketball-0.0.3/usports_basketball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-30 06:46:13.000000 usports_basketball-0.0.3/usports_basketball.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-30 06:46:13.000000 usports_basketball-0.0.3/usports_basketball.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.125507 usports_basketball-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.125507 usports_basketball-1.0.0/usports_basketball/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/usports_basketball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/usports_basketball/player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14902 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/usports_basketball/team_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/usports_basketball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/top_level.txt
```

### Comparing `usports_basketball-0.0.3/PKG-INFO` & `usports_basketball-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,108 @@
-Metadata-Version: 2.1
-Name: usports-basketball
-Version: 0.0.3
-Summary: A Python package for USports basketball stats.
-Author-email: OJ Adeyemi <ojieadeyemi@gmail.com>
-Maintainer-email: OJ Adeyemi <ojieadeyemi@gmail.com>
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: beautifulsoup4>=4.12.0
-Requires-Dist: pandas>=2.2.0
-
-# USports Basketball Statistics Package
-
-## Introduction
-
-The USports Basketball Statistics Package is a Python package designed to retrieve and analyze basketball statistics data from the USports website. This package provides functions for web scraping and processing both team and player statistics, allowing users to gather data for analysis and insights.
-
-## Installation
-
-You can install the package via pip:
-
-```bash
-pip install usports-basketball
-```
-
-## Dependencies
-
-This package relies on the following dependencies:
-- requests
-- BeautifulSoup (bs4)
-- pandas
-
-Make sure you have these dependencies installed before using the package.
-
-## Functions
-
-### `usports_team_stats`
-
-This function fetches and processes team statistics data, including standings, win-loss totals, shooting percentages, and other relevant team metrics for the current USports basketball season.
-
-#### Parameters
-
-- `league` (str): The conference for which you want to retrieve team statistics. Valid values are `'men'` and `'women'`.
-
-#### Returns
-
-- `DataFrame`: A pandas DataFrame containing the team statistics data.
-
-### `usports_player_stats`
-
-This function fetches and processes player statistics data, including total games played, points scored, shooting percentages, rebounds, assists, turnovers, steals, blocks, and other individual player metrics for the current USports basketball season.
-
-#### Parameters
-
-- `league` (str): The conference for which you want to retrieve player statistics. Valid values are `'men'` and `'women'`.
-
-#### Returns
-
-- `DataFrame`: A pandas DataFrame containing the player statistics data.
-
-## Example Usage
-
-```python
-from usports_basketball import usports_team_stats, usports_player_stats
-
-# Fetching and processing men's team statistics
-men_team_stats_df = usports_team_stats('men')
-
-# Fetching and processing men's player statistics
-men_player_stats_df = usports_player_stats('men')
-```
-
-## Note
-
-- This package is based on the current USports basketball season only. To access statistics from previous seasons, manual adjustments to the web scraping code may be required.
-
-## Author
-
-This package was developed by OJ Adeyemi.
-
-## Contributing
-
-Contributions, bug reports, and feature requests are welcome! Please feel free to open an issue or submit a pull request on [GitHub](https://github.com/ojadeyemi/usports-basketball).
-
-## License
-
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
-for details.
+Metadata-Version: 2.1
+Name: usports-basketball
+Version: 1.0.0
+Summary: A Python package for USports basketball stats.
+Author-email: OJ Adeyemi <ojieadeyemi@gmail.com>
+Maintainer-email: OJ Adeyemi <ojieadeyemi@gmail.com>
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: requests>=2.31.0
+Requires-Dist: beautifulsoup4>=4.12.0
+Requires-Dist: pandas>=2.2.0
+
+# USports Basketball Statistics Package
+
+## Introduction
+
+The USports Basketball Statistics Package is a Python package designed to retrieve and analyze basketball statistics data from the USports website. This package provides functions for web scraping and processing both team and player statistics, allowing users to gather data for analysis and insights.
+
+## Installation
+
+You can install the package via pip:
+
+```bash
+pip install usports-basketball
+```
+
+## Dependencies
+
+This package relies on the following dependencies:
+- requests
+- BeautifulSoup (bs4)
+- pandas
+
+Make sure you have these dependencies installed before using the package.
+
+## Functions
+
+### `usports_team_stats`
+
+This function fetches and processes team statistics data, including standings, win-loss totals, shooting percentages, and other relevant team metrics for the current USports basketball season.
+
+#### Parameters
+
+- `arg` (str): The conference for which you want to retrieve team statistics. Valid values are `'men'` and `'women'`.
+
+#### Returns
+
+- `DataFrame`: A pandas DataFrame containing the team statistics data.
+
+### `usports_player_stats`
+
+This function fetches and processes player statistics data, including total games played, points scored, shooting percentages, rebounds, assists, turnovers, steals, blocks, and other individual player metrics for the current USports basketball season.
+
+#### Parameters
+
+- `arg` (str): The conference for which you want to retrieve player statistics. Valid values are `'men'` and `'women'`.
+
+#### Returns
+
+- `DataFrame`: A pandas DataFrame containing the player statistics data.
+
+## Example Usage
+
+```python
+from usports_basketball import usports_team_stats, usports_player_stats
+
+# Fetching and processing men's team statistics
+men_team_stats_df = usports_team_stats('men')
+
+# Fetching and processing men's player statistics
+men_player_stats_df = usports_player_stats('men')
+```
+
+You can use the `.dtype` function to retrieve the data types of all columns in the DataFrame. This can be useful for understanding the structure of the data you've fetched. Here's how you can use it:
+
+```python
+# Assuming `usports_player_stats` returns a DataFrame named `men_player_stats_df`
+# Fetching and processing men's player statistics
+men_player_stats_df = usports_player_stats('men')
+
+# Get the data types of all columns with their column names
+column_dtypes = men_player_stats_df.dtypes
+
+# Print the column names and their corresponding data types
+print(column_dtypes)
+```
+
+## Note
+
+- This package is based on the current USports basketball season only. To access statistics from previous seasons, manual adjustments to the web scraping code may be required.
+
+## Author
+
+This package was developed by OJ Adeyemi.
+
+## Contributing
+
+Contributions, bug reports, and feature requests are welcome! Please feel free to open an issue or submit a pull request on [GitHub](https://github.com/ojadeyemi/usports-basketball).
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
+for details.
```

### Comparing `usports_basketball-0.0.3/pyproject.toml` & `usports_basketball-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[project]
-name = "usports-basketball"
-version = "0.0.3"
-description = "A Python package for USports basketball stats."
-readme = "README.md"
-license = {file = "LICENSE.txt"}
-authors = [{name = "OJ Adeyemi", email = "ojieadeyemi@gmail.com"}]
-maintainers = [{name = "OJ Adeyemi", email = "ojieadeyemi@gmail.com"}]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-]
-requires-python = ">=3.8"
-dependencies = [
-    "requests>=2.31.0",
-    "beautifulsoup4>=4.12.0",
-    "pandas>=2.2.0",
-]
-
-[build-system]
-requires = ["setuptools>=46.1.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.pytest.ini_options]
-testpaths = ["tests"]
-filterwarnings = [
-    "error",
-]
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.4"
-
+[project]
+name = "usports-basketball"
+version = "1.0.0"
+description = "A Python package for USports basketball stats."
+readme = "README.md"
+license = {file = "LICENSE.txt"}
+authors = [{name = "OJ Adeyemi", email = "ojieadeyemi@gmail.com"}]
+maintainers = [{name = "OJ Adeyemi", email = "ojieadeyemi@gmail.com"}]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Developers",
+]
+requires-python = ">=3.8"
+dependencies = [
+    "requests>=2.31.0",
+    "beautifulsoup4>=4.12.0",
+    "pandas>=2.2.0",
+]
+
+[build-system]
+requires = ["setuptools>=46.1.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+filterwarnings = [
+    "error",
+]
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4"
+
 [project.urls]
```

### Comparing `usports_basketball-0.0.3/test/test.py` & `usports_basketball-1.0.0/test/test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import pytest
-
-import pandas as pd
-
-from usports_basketball import usports_team_stats, usports_player_stats
-
-def test_usports_team_stats_returns_dataframe():
-    team_stats_df = usports_team_stats('men')
-    assert isinstance(team_stats_df, pd.DataFrame)
-
-def test_usports_player_stats_returns_dataframe():
-    player_stats_df = usports_player_stats('women')
-    assert isinstance(player_stats_df, pd.DataFrame)
-
-def test_usports_team_stats_non_empty():
-    team_stats_df = usports_team_stats('women')
-    assert not team_stats_df.empty, "Team statistics DataFrame is empty"
-
-def test_usports_player_stats_non_empty():
-    player_stats_df = usports_player_stats('men')
-    assert not player_stats_df.empty, "Player statistics DataFrame is empty"
-
-def test_usports_team_stats_columns():
-    team_stats_df = usports_team_stats('men')
-    expected_columns = [
-        'team_name',
-        'games_played',
-        # Add more expected columns as needed
-    ]
-    assert all(column in team_stats_df.columns for column in expected_columns), "Missing columns in team statistics DataFrame"
-
-def test_usports_player_stats_columns():
-    player_stats_df = usports_player_stats('men')
-    expected_columns = [
-        'lastname_initials',
-        'first_name',
-        # Add more expected columns as needed
-    ]
-    assert all(column in player_stats_df.columns for column in expected_columns), "Missing columns in player statistics DataFrame"
-
+import pytest
+
+import pandas as pd
+
+from usports_basketball import usports_team_stats, usports_player_stats
+
+def test_usports_team_stats_returns_dataframe():
+    team_stats_df = usports_team_stats('men')
+    assert isinstance(team_stats_df, pd.DataFrame)
+
+def test_usports_player_stats_returns_dataframe():
+    player_stats_df = usports_player_stats('women')
+    assert isinstance(player_stats_df, pd.DataFrame)
+
+def test_usports_team_stats_non_empty():
+    team_stats_df = usports_team_stats('women')
+    assert not team_stats_df.empty, "Team statistics DataFrame is empty"
+
+def test_usports_player_stats_non_empty():
+    player_stats_df = usports_player_stats('men')
+    assert not player_stats_df.empty, "Player statistics DataFrame is empty"
+
+def test_usports_team_stats_columns():
+    team_stats_df = usports_team_stats('men')
+    expected_columns = [
+        'team_name',
+        'games_played',
+        # Add more expected columns as needed
+    ]
+    assert all(column in team_stats_df.columns for column in expected_columns), "Missing columns in team statistics DataFrame"
+
+def test_usports_player_stats_columns():
+    player_stats_df = usports_player_stats('men')
+    expected_columns = [
+        'lastname_initials',
+        'first_name',
+        # Add more expected columns as needed
+    ]
+    assert all(column in player_stats_df.columns for column in expected_columns), "Missing columns in player statistics DataFrame"
+
```

### Comparing `usports_basketball-0.0.3/usports_basketball/__init__.py` & `usports_basketball-1.0.0/usports_basketball/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-
-"""
-USports Basketball Statistics Web Scraping and Processing Package
-
-This package provides functions for web scraping and processing basketball statistics data from the USports website. It encompasses functionality for retrieving both team and player statistics.
-
-Dependencies:
-    - requests
-    - BeautifulSoup (bs4)
-    - pandas
-    
-Functions:
-- usports_team_stats: Fetches and processes team statistics data, including standings, win-loss totals, and other relevant team metrics.
-- usports_player_stats: Fetches and processes player statistics data, including total games played, total points scored, field goal percentage, and other individual player metrics.
-
-These functions return pandas DataFrames containing the respective statistics data.
-Note: This is based on current season only, to get stats from previous season you'll need to manually make changes in both team and players webscraping files
-
-# Example:
->>> from usportsbballstats import usports_team_stats, usports_player_stats
-#Fetching and processing men's team and players statistics 
->>> men_team_stats_df = usports_team_stats('men')
-# Fetching and processing player statistics data for men's players
->>> men_player_stats_df = usports_player_stats('men') \n
-
-Author:
-    OJ Adeyemi
-
-Date Created:
-    March 1, 2024
-"""
-from .team_stats import usports_team_stats
-from .player_stats import usports_player_stats
-
+
+"""
+USports Basketball Statistics Web Scraping and Processing Package
+
+This package provides functions for web scraping and processing basketball statistics data from the USports website. It encompasses functionality for retrieving both team and player statistics.
+
+Dependencies:
+    - requests
+    - BeautifulSoup (bs4)
+    - pandas
+    
+Functions:
+- usports_team_stats: Fetches and processes team statistics data, including standings, win-loss totals, and other relevant team metrics.
+- usports_player_stats: Fetches and processes player statistics data, including total games played, total points scored, field goal percentage, and other individual player metrics.
+
+These functions return pandas DataFrames containing the respective statistics data.
+Note: This is based on current season only, to get stats from previous season you'll need to manually make changes in both team and players webscraping files
+
+# Example:
+>>> from usportsbballstats import usports_team_stats, usports_player_stats
+#Fetching and processing men's team and players statistics 
+>>> men_team_stats_df = usports_team_stats('men')
+# Fetching and processing player statistics data for men's players
+>>> men_player_stats_df = usports_player_stats('men') \n
+
+Author:
+    OJ Adeyemi
+
+Date Created:
+    March 1, 2024
+"""
+from .team_stats import usports_team_stats
+from .player_stats import usports_player_stats
+
```

### Comparing `usports_basketball-0.0.3/usports_basketball/player_stats.py` & `usports_basketball-1.0.0/usports_basketball/player_stats.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-import requests
-from bs4 import BeautifulSoup
-import pandas as pd
-
-def __usports_player_offense_data(offense_url:str) -> pd.DataFrame:
-    """
-    Fetches and processes player offense statistics data from the given URL.
-
-    Args:
-        offense_url (str): URL of the player offense statistics data.
-
-    Returns:
-        pd.DataFrame: DataFrame containing processed player offense statistics.
-    """ 
-    offense_page = requests.get(offense_url)
-
-    # Parse the HTML using BeautifulSoup
-   
-    offense_soup = BeautifulSoup(offense_page.content, 'html.parser')
-
-    offense_rows = offense_soup.find_all('tr')
-
-    # Initialize lists to store data
-    data = {
-        'lastname_initials': [],
-        'first_name': [],
-        'school': [],
-        'minutes_played': [],
-        'field_goal_made': [],
-        'field_goal_attempted': [],
-        'field_goal_percentage': [],
-        'three_pointers_made': [],
-        'three_pointers_attempted': [],
-        'three_pointers_percentage': [],
-        'free_throws_made': [],
-        'free_throws_attempted': [],
-        'free_throws_percentage': [],
-        'total_points': [],
-    }
-    # Iterate through each row
-    for row in offense_rows:
-        cols = row.find_all('td')  # Find all <td> tags with class 'text'
-        if len(cols) > 0:
-            player_lastname_initials = cols[1].get_text(strip=True).split()[0]  # Assuming lastname initials are the first letter of the second <td> content
-            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  # Assuming firstname is the rest of the content after lastname initials
-            school = cols[2].get_text(strip=True)
-            minutes_played = cols[5].get_text(strip=True)
-            field_goals_made, field_goals_attempted = cols[6].get_text(strip=True).split('-')
-            field_goal_percentage = cols[7].get_text(strip=True)
-            three_points_made,three_points_attempted = cols[8].get_text(strip=True).split('-')
-            three_points_percentage = cols[9].get_text(strip=True)
-            free_throws_made,free_throws_attempted = cols[10].get_text(strip=True).split('-')
-            free_throw_percentage = cols[11].get_text(strip=True)
-            total_points = cols[12].get_text(strip=True)
-
-            # Append data to lists
-            data['lastname_initials'].append(player_lastname_initials)
-            data['first_name'].append(firstname)
-            data['school'].append(school)
-            data['minutes_played'].append(minutes_played)
-            data['field_goal_made'].append(field_goals_made)
-            data['field_goal_attempted'].append(field_goals_attempted)
-            data['field_goal_percentage'].append(field_goal_percentage)
-            data['three_pointers_made'].append(three_points_made)
-            data['three_pointers_attempted'].append(three_points_attempted)
-            data['three_pointers_percentage'].append(three_points_percentage)
-            data['free_throws_made'].append(free_throws_made)
-            data['free_throws_attempted'].append(free_throws_attempted)
-            data['free_throws_percentage'].append(free_throw_percentage)
-            data['total_points'].append(total_points)
-
-    # Create DataFrame
-    df = pd.DataFrame(data)
-    return df
-
-
-def __usports_player_defense_data(defense_url:str) -> pd.DataFrame:
-    """
-    Fetches and processes player offense statistics data from the given URL.
-
-    Args:
-        defense_url (str): URL of the player defense statistics data.
-
-    Returns:
-        pd.DataFrame: DataFrame containing processed player defense statistics.
-    """ 
-    defense_page = requests.get(defense_url)
-
-    # Parse the HTML using BeautifulSoup
-   
-    defense_soup = BeautifulSoup(defense_page.content, 'html.parser')
-
-    # Initialize lists to store data
-    data = {
-        'lastname_initials': [],
-        'first_name': [],
-        'school': [],
-        'games_played': [],
-        'games_started': [],
-        'minutes_played': [],
-        'offensive_rebounds': [],
-        'defensive_rebounds': [],
-        'total_rebounds': [],
-        'personal_fouls': [],
-        'disqualifications': [],
-        'assists': [],
-        'turnovers': [],
-        'assist_per_turnover': [],
-        'steals': [],
-        'blocks': []
-    }
-
-    # Find all <tr> tags
-    defense_rows = defense_soup.find_all('tr')
-
-    # Iterate through each row
-    for row in defense_rows:
-        cols = row.find_all('td')  # Find all <td> tags with class 'text'
-        if len(cols) > 0:
-            player_lastname_initials = cols[1].get_text(strip=True).split()[0]  # Assuming lastname initials are the first letter of the second <td> content
-            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  # Assuming firstname is the rest of the content after lastname initials
-            school = cols[2].get_text(strip=True)
-            games_played = cols[3].get_text(strip=True)
-            games_started = cols[4].get_text(strip=True)
-            minutes_played = cols[5].get_text(strip=True)
-            off_reb = cols[6].get_text(strip=True)
-            def_reb = cols[7].get_text(strip=True)
-            total_reb = cols[8].get_text(strip=True)
-            personal_fouls = cols[9].get_text(strip=True)
-            disqualifications = cols[10].get_text(strip=True)
-            
-            # Assuming the following columns correspond to assist, turnovers, assist/turnover, steals, and blocks
-            assists = cols[11].get_text(strip=True)
-            turnovers = cols[12].get_text(strip=True)
-            assist_turnover = cols[13].get_text(strip=True)
-            steals = cols[14].get_text(strip=True)
-            blocks = cols[15].get_text(strip=True)
-            
-            # Append data to lists
-            data['lastname_initials'].append(player_lastname_initials)
-            data['first_name'].append(firstname)
-            data['school'].append(school)
-            data['games_played'].append(games_played)
-            data['games_started'].append(games_started)
-            data['minutes_played'].append(minutes_played)
-            data['offensive_rebounds'].append(off_reb)
-            data['defensive_rebounds'].append(def_reb)
-            data['total_rebounds'].append(total_reb)
-            data['personal_fouls'].append(personal_fouls)
-            data['disqualifications'].append(disqualifications)
-            data['assists'].append(assists)
-            data['turnovers'].append(turnovers)
-            data['assist_per_turnover'].append(assist_turnover)
-            data['steals'].append(steals)
-            data['blocks'].append(blocks)
-
-    # Create DataFrame
-    df = pd.DataFrame(data)
-
-    return df
-
-
-def usports_player_stats(arg:str) -> pd.DataFrame:
-    """
-    Fetches and processes player statistics data from USports website.
-
-    Args:
-        arg (str): Gender of the players. Should be either 'men' or 'women'.
-
-    Returns:
-        pd.DataFrame: DataFrame containing processed player statistics.
-    """
-    if(arg == 'men'):
-            players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=st&r=0')
-            players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=bt&r=0')
-    elif (arg == 'women'):
-        players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/wbkb/2023-24/players?view=&pos=st&r=0')
-        players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/wbkb/2023-24/players?view=&pos=bt&r=0')
-
-    players_stats_df = pd.merge(players_def_stats_df, players_off_stats_df, on=['lastname_initials','first_name','school', 'minutes_played'], how='inner')
-    
-    players_stats_df['games_played'] = pd.to_numeric(players_stats_df['games_played'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['games_started'] = pd.to_numeric(players_stats_df['games_started'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['minutes_played'] = pd.to_numeric(players_stats_df['minutes_played'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['offensive_rebounds'] = pd.to_numeric(players_stats_df['offensive_rebounds'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['defensive_rebounds'] = pd.to_numeric(players_stats_df['defensive_rebounds'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['total_rebounds'] = pd.to_numeric(players_stats_df['total_rebounds'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['personal_fouls'] = pd.to_numeric(players_stats_df['personal_fouls'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['disqualifications'] = pd.to_numeric(players_stats_df['disqualifications'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['assists'] = pd.to_numeric(players_stats_df['assists'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['turnovers'] = pd.to_numeric(players_stats_df['turnovers'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['assist_per_turnover'] = pd.to_numeric(players_stats_df['assist_per_turnover'], errors='coerce').fillna(0).astype(float)
-    players_stats_df['steals'] = pd.to_numeric(players_stats_df['steals'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['blocks'] = pd.to_numeric(players_stats_df['blocks'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['field_goal_made'] = pd.to_numeric(players_stats_df['field_goal_made'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['field_goal_attempted'] = pd.to_numeric(players_stats_df['field_goal_attempted'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['field_goal_percentage'] = pd.to_numeric(players_stats_df['field_goal_percentage'], errors='coerce').fillna(0).astype(float)
-    players_stats_df['three_pointers_made'] = pd.to_numeric(players_stats_df['three_pointers_made'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['three_pointers_attempted'] = pd.to_numeric(players_stats_df['three_pointers_attempted'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['three_pointers_percentage'] = pd.to_numeric(players_stats_df['three_pointers_percentage'], errors='coerce').fillna(0).astype(float)
-    players_stats_df['free_throws_made'] = pd.to_numeric(players_stats_df['free_throws_made'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['free_throws_attempted'] = pd.to_numeric(players_stats_df['free_throws_attempted'], errors='coerce').fillna(0).astype(int)
-    players_stats_df['free_throws_percentage'] = pd.to_numeric(players_stats_df['free_throws_percentage'], errors='coerce').fillna(0).astype(float)
-    players_stats_df['total_points'] = pd.to_numeric(players_stats_df['total_points'], errors='coerce').fillna(0).astype(int)
-
+import requests
+from bs4 import BeautifulSoup
+import pandas as pd
+
+def __usports_player_offense_data(offense_url:str) -> pd.DataFrame:
+    """
+    Fetches and processes player offense statistics data from the given URL.
+
+    Args:
+        offense_url (str): URL of the player offense statistics data.
+
+    Returns:
+        pd.DataFrame: DataFrame containing processed player offense statistics.
+    """ 
+    offense_page = requests.get(offense_url)
+
+    # Parse the HTML using BeautifulSoup
+   
+    offense_soup = BeautifulSoup(offense_page.content, 'html.parser')
+
+    offense_rows = offense_soup.find_all('tr')
+
+    # Initialize lists to store data
+    data = {
+        'lastname_initials': [],
+        'first_name': [],
+        'school': [],
+        'minutes_played': [],
+        'field_goal_made': [],
+        'field_goal_attempted': [],
+        'field_goal_percentage': [],
+        'three_pointers_made': [],
+        'three_pointers_attempted': [],
+        'three_pointers_percentage': [],
+        'free_throws_made': [],
+        'free_throws_attempted': [],
+        'free_throws_percentage': [],
+        'total_points': [],
+    }
+    # Iterate through each row
+    for row in offense_rows:
+        cols = row.find_all('td')  # Find all <td> tags with class 'text'
+        if len(cols) > 0:
+            player_lastname_initials = cols[1].get_text(strip=True).split()[0]  # Assuming lastname initials are the first letter of the second <td> content
+            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  # Assuming firstname is the rest of the content after lastname initials
+            school = cols[2].get_text(strip=True)
+            minutes_played = cols[5].get_text(strip=True)
+            field_goals_made, field_goals_attempted = cols[6].get_text(strip=True).split('-')
+            field_goal_percentage = cols[7].get_text(strip=True)
+            three_points_made,three_points_attempted = cols[8].get_text(strip=True).split('-')
+            three_points_percentage = cols[9].get_text(strip=True)
+            free_throws_made,free_throws_attempted = cols[10].get_text(strip=True).split('-')
+            free_throw_percentage = cols[11].get_text(strip=True)
+            total_points = cols[12].get_text(strip=True)
+
+            # Append data to lists
+            data['lastname_initials'].append(player_lastname_initials)
+            data['first_name'].append(firstname)
+            data['school'].append(school)
+            data['minutes_played'].append(minutes_played)
+            data['field_goal_made'].append(field_goals_made)
+            data['field_goal_attempted'].append(field_goals_attempted)
+            data['field_goal_percentage'].append(field_goal_percentage)
+            data['three_pointers_made'].append(three_points_made)
+            data['three_pointers_attempted'].append(three_points_attempted)
+            data['three_pointers_percentage'].append(three_points_percentage)
+            data['free_throws_made'].append(free_throws_made)
+            data['free_throws_attempted'].append(free_throws_attempted)
+            data['free_throws_percentage'].append(free_throw_percentage)
+            data['total_points'].append(total_points)
+
+    # Create DataFrame
+    df = pd.DataFrame(data)
+    return df
+
+
+def __usports_player_defense_data(defense_url:str) -> pd.DataFrame:
+    """
+    Fetches and processes player offense statistics data from the given URL.
+
+    Args:
+        defense_url (str): URL of the player defense statistics data.
+
+    Returns:
+        pd.DataFrame: DataFrame containing processed player defense statistics.
+    """ 
+    defense_page = requests.get(defense_url)
+
+    # Parse the HTML using BeautifulSoup
+   
+    defense_soup = BeautifulSoup(defense_page.content, 'html.parser')
+
+    # Initialize lists to store data
+    data = {
+        'lastname_initials': [],
+        'first_name': [],
+        'school': [],
+        'games_played': [],
+        'games_started': [],
+        'minutes_played': [],
+        'offensive_rebounds': [],
+        'defensive_rebounds': [],
+        'total_rebounds': [],
+        'personal_fouls': [],
+        'disqualifications': [],
+        'assists': [],
+        'turnovers': [],
+        'assist_per_turnover': [],
+        'steals': [],
+        'blocks': []
+    }
+
+    # Find all <tr> tags
+    defense_rows = defense_soup.find_all('tr')
+
+    # Iterate through each row
+    for row in defense_rows:
+        cols = row.find_all('td')  # Find all <td> tags with class 'text'
+        if len(cols) > 0:
+            player_lastname_initials = cols[1].get_text(strip=True).split()[0]  # Assuming lastname initials are the first letter of the second <td> content
+            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  # Assuming firstname is the rest of the content after lastname initials
+            school = cols[2].get_text(strip=True)
+            games_played = cols[3].get_text(strip=True)
+            games_started = cols[4].get_text(strip=True)
+            minutes_played = cols[5].get_text(strip=True)
+            off_reb = cols[6].get_text(strip=True)
+            def_reb = cols[7].get_text(strip=True)
+            total_reb = cols[8].get_text(strip=True)
+            personal_fouls = cols[9].get_text(strip=True)
+            disqualifications = cols[10].get_text(strip=True)
+            
+            # Assuming the following columns correspond to assist, turnovers, assist/turnover, steals, and blocks
+            assists = cols[11].get_text(strip=True)
+            turnovers = cols[12].get_text(strip=True)
+            assist_turnover = cols[13].get_text(strip=True)
+            steals = cols[14].get_text(strip=True)
+            blocks = cols[15].get_text(strip=True)
+            
+            # Append data to lists
+            data['lastname_initials'].append(player_lastname_initials)
+            data['first_name'].append(firstname)
+            data['school'].append(school)
+            data['games_played'].append(games_played)
+            data['games_started'].append(games_started)
+            data['minutes_played'].append(minutes_played)
+            data['offensive_rebounds'].append(off_reb)
+            data['defensive_rebounds'].append(def_reb)
+            data['total_rebounds'].append(total_reb)
+            data['personal_fouls'].append(personal_fouls)
+            data['disqualifications'].append(disqualifications)
+            data['assists'].append(assists)
+            data['turnovers'].append(turnovers)
+            data['assist_per_turnover'].append(assist_turnover)
+            data['steals'].append(steals)
+            data['blocks'].append(blocks)
+
+    # Create DataFrame
+    df = pd.DataFrame(data)
+
+    return df
+
+
+def usports_player_stats(arg:str) -> pd.DataFrame:
+    """
+    Fetches and processes player statistics data from USports website.
+
+    Args:
+        arg (str): Gender of the players. Should be either 'men' or 'women'.
+
+    Returns:
+        pd.DataFrame: DataFrame containing processed player statistics.
+    """
+    if(arg == 'men'):
+            players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=st&r=0')
+            players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=bt&r=0')
+    elif (arg == 'women'):
+        players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/wbkb/2023-24/players?view=&pos=st&r=0')
+        players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/wbkb/2023-24/players?view=&pos=bt&r=0')
+
+    players_stats_df = pd.merge(players_def_stats_df, players_off_stats_df, on=['lastname_initials','first_name','school', 'minutes_played'], how='inner')
+    
+    players_stats_df['games_played'] = pd.to_numeric(players_stats_df['games_played'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['games_started'] = pd.to_numeric(players_stats_df['games_started'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['minutes_played'] = pd.to_numeric(players_stats_df['minutes_played'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['offensive_rebounds'] = pd.to_numeric(players_stats_df['offensive_rebounds'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['defensive_rebounds'] = pd.to_numeric(players_stats_df['defensive_rebounds'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['total_rebounds'] = pd.to_numeric(players_stats_df['total_rebounds'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['personal_fouls'] = pd.to_numeric(players_stats_df['personal_fouls'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['disqualifications'] = pd.to_numeric(players_stats_df['disqualifications'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['assists'] = pd.to_numeric(players_stats_df['assists'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['turnovers'] = pd.to_numeric(players_stats_df['turnovers'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['assist_per_turnover'] = pd.to_numeric(players_stats_df['assist_per_turnover'], errors='coerce').fillna(0).astype(float)
+    players_stats_df['steals'] = pd.to_numeric(players_stats_df['steals'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['blocks'] = pd.to_numeric(players_stats_df['blocks'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['field_goal_made'] = pd.to_numeric(players_stats_df['field_goal_made'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['field_goal_attempted'] = pd.to_numeric(players_stats_df['field_goal_attempted'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['field_goal_percentage'] = pd.to_numeric(players_stats_df['field_goal_percentage'], errors='coerce').fillna(0).astype(float)
+    players_stats_df['three_pointers_made'] = pd.to_numeric(players_stats_df['three_pointers_made'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['three_pointers_attempted'] = pd.to_numeric(players_stats_df['three_pointers_attempted'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['three_pointers_percentage'] = pd.to_numeric(players_stats_df['three_pointers_percentage'], errors='coerce').fillna(0).astype(float)
+    players_stats_df['free_throws_made'] = pd.to_numeric(players_stats_df['free_throws_made'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['free_throws_attempted'] = pd.to_numeric(players_stats_df['free_throws_attempted'], errors='coerce').fillna(0).astype(int)
+    players_stats_df['free_throws_percentage'] = pd.to_numeric(players_stats_df['free_throws_percentage'], errors='coerce').fillna(0).astype(float)
+    players_stats_df['total_points'] = pd.to_numeric(players_stats_df['total_points'], errors='coerce').fillna(0).astype(int)
+
     return players_stats_df
```

### Comparing `usports_basketball-0.0.3/usports_basketball/team_stats.py` & `usports_basketball-1.0.0/usports_basketball/team_stats.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,350 +1,350 @@
-#importing libraries
-import requests
-from bs4 import BeautifulSoup
-import pandas as pd
-
-def __usports_team_data(stats_url: str, standings_url: str, no_of_teams: int) -> pd.DataFrame:
-    '''
-    This function takes the URL of the USport's team stats and the number of teams and returns a
-    DataFrame of the team and their stats, removing any rows of teams that didn't play that season.
-
-    Args:
-        stats_url (str): URL of the team statistics data.
-        standings_url (str): URL of the standings page.
-        no_of_teams (int): Number of teams.
-
-    Returns:
-        pd.DataFrame: DataFrame containing processed team statistics.
-    '''
-    #perfrom GET request to the URL and returns the server response to the HTTP request
-    page = requests.get(stats_url)
-   
-    if(page.status_code != 200):
-        print("USport's Server did not respond with HTTP request")
-
-    #parse html document
-    soup = BeautifulSoup(page.content, 'html.parser')
-
-    #Find the table containing stats
-    rows = soup.find_all('tr')
-    
-    #Intialize lists to store data
-    team_names =[]
-    games_played = []
-    field_goals = []
-    field_goal_percentage = []
-    three_pointers = []
-    three_point_percentage = []
-    free_throws = []
-    free_throw_percentage = []
-    off_rebounds_per_game = []
-    def_rebounds_per_game = []
-    total_rebounds_per_game = []
-    assists_per_game = []
-    turnovers_per_game = []
-    steals_per_game = []
-    blocks_per_game = []
-    fouls_per_game = []
-    points_per_game = []
-    off_efficiency = []
-    net_efficiency = []
-    field_goals_against = []
-    field_goal_against_percentage = []
-    three_pointers_against = []
-    three_point_against_percentage = []
-    off_rebounds_per_game_against = []
-    def_rebounds_per_game_against = []
-    total_rebounds_per_game_against = []
-    assists_per_game_against = []
-    turnovers_per_game_against = []
-    steals_per_game_against = []
-    blocks_per_game_against = []
-    fouls_per_game_against = []
-    points_per_game_against = []
-    def_efficiency = []
-
-    #Loop through each row(skip the first row as it's the header)
-    for index, row in enumerate(rows[1:]):
-
-        #exit loop when we reached end of table
-        if index >= no_of_teams:
-            break
-
-        #Extract team name
-        school_name = row.find('td', class_='pinned-col text').text.strip()
-   
-        team_names.append(school_name)
-
-        #Extract data from other columns
-        columns = row.find_all('td', align = 'center')
-        games_played.append(columns[0].text.strip())
-        field_goals.append(columns[1].text.strip())
-        field_goal_percentage.append(columns[2].text.strip())
-        three_pointers.append(columns[3].text.strip())
-        three_point_percentage.append(columns[4].text.strip())
-        free_throws.append(columns[5].text.strip())
-        free_throw_percentage.append(columns[6].text.strip())
-        off_rebounds_per_game.append(columns[7].text.strip())
-        def_rebounds_per_game.append(columns[8].text.strip())
-        total_rebounds_per_game.append(columns[9].text.strip())
-        assists_per_game.append(columns[10].text.strip())
-        turnovers_per_game.append(columns[11].text.strip())
-        steals_per_game.append(columns[12].text.strip())
-        blocks_per_game.append(columns[13].text.strip())
-        fouls_per_game.append(columns[14].text.strip())
-        points_per_game.append(columns[15].text.strip())
-        off_efficiency.append(columns[16].text.strip())
-        net_efficiency.append(columns[17].text.strip())
-
-    #Loop through defensive stats row (skip first row(header) and second row which contains game played)
-    for index, row in enumerate(rows[no_of_teams+2:]):
-        
-        #exit loop when we reached end of table
-        if index >= no_of_teams:
-            break
-
-        #Extract data from other columns
-        columns = row.find_all('td', align = 'center')
-        field_goals_against.append(columns[1].text.strip())
-        field_goal_against_percentage.append(columns[2].text.strip())
-        three_pointers_against.append(columns[3].text.strip())
-        three_point_against_percentage.append(columns[4].text.strip())
-        off_rebounds_per_game_against.append(columns[5].text.strip())
-        def_rebounds_per_game_against.append(columns[6].text.strip())
-        total_rebounds_per_game_against.append(columns[7].text.strip())
-        assists_per_game_against.append(columns[9].text.strip())
-        turnovers_per_game_against.append(columns[10].text.strip())
-        steals_per_game_against.append(columns[11].text.strip())
-        blocks_per_game_against.append(columns[12].text.strip())
-        fouls_per_game_against.append(columns[13].text.strip())
-        points_per_game_against.append(columns[14].text.strip())
-        def_efficiency.append(columns[15].text.strip())   
-
-    data_collected = {
-        'team_name': team_names,
-        'games_played': games_played,
-        'points_per_game': points_per_game,
-        'field_goals': field_goals,
-        'field_goal_percentage': field_goal_percentage,
-        'three_points': three_pointers,
-        'three_point_percentage': three_point_percentage,
-        'free_throws': free_throws,
-        'free_throw_percentage': free_throw_percentage,
-        'offensive_rebounds_per_game': off_rebounds_per_game,
-        'defensive_rebounds_per_game': def_rebounds_per_game,
-        'total_rebounds_per_game': total_rebounds_per_game,
-        'assists_per_game' : assists_per_game,
-        'turnovers_per_game': turnovers_per_game,
-        'steals_per_game': steals_per_game,
-        'blocks_per_game': blocks_per_game,
-        'team_fouls_per_game': fouls_per_game,
-        'offensive_efficiency': off_efficiency,
-        'defensive_efficiency': def_efficiency,
-        'Net_efficiency': net_efficiency,
-        'field_goals_against': field_goals_against,
-        'field_goals_percentage_against': field_goal_against_percentage,
-        'three_points_against': three_pointers_against,
-        'three_points_percentage_against': three_point_against_percentage,
-        'offensive_rebounds_per_game_against': off_rebounds_per_game_against,
-        'defensive_rebounds_per_game_against': def_rebounds_per_game_against,
-        'total_rebounds_per_game_against': total_rebounds_per_game_against,
-        'assists_per_game_against': assists_per_game_against,
-        'turnovers_per_game_against': turnovers_per_game_against,
-        'steals_per_game_against': steals_per_game_against,
-        'blocks_per_game_against': blocks_per_game_against,
-        'team_fouls_per_game_against': fouls_per_game_against,
-        'points_per_game_against': points_per_game_against
-        }
-    
-    
-    #create dictionary that maps university sports team to respective conference
-    team_conference = {
-    'Acadia': 'AUS',
-    'Alberta': 'CW',
-    'Algoma': 'OUA West',
-    'Bishop\'s': 'RSEQ',
-    'Brandon': 'CW',
-    'Brock': 'OUA Central',
-    'Calgary': 'CW',
-    'Cape Breton': 'AUS',
-    'Carleton': 'OUA East',
-    'Concordia': 'RSEQ',
-    'Dalhousie': 'AUS',
-    'Guelph': 'OUA West',
-    'Lakehead': 'OUA Central',
-    'Laurentian': 'OUA East',
-    'Laurier': 'OUA West',
-    'Laval': 'RSEQ',
-    'Lethbridge': 'CW',
-    'MacEwan': 'CW',
-    'Manitoba': 'CW',
-    'McGill': 'RSEQ',
-    'McMaster': 'OUA Central',
-    'Memorial': 'AUS',
-    'Mount Royal': 'CW',
-    'Nipissing': 'OUA East',
-    'Ontario Tech': 'OUA East',
-    'Ottawa': 'OUA East',
-    'Queen\'s': 'OUA East',
-    'Regina': 'CW',
-    'Saint Mary\'s': 'AUS',
-    'Saskatchewan': 'CW',
-    'StFX': 'AUS',
-    'Thompson Rivers': 'CW',
-    'Toronto': 'OUA Central',
-    'Toronto Metropolitan': 'OUA Central',
-    'Trinity Western': 'CW',
-    'UBC': 'CW',
-    'UBC Okanagan': 'CW',
-    'UFV': 'CW',
-    'UNB': 'AUS',
-    'UNBC': 'CW',
-    'UPEI': 'AUS',
-    'UQAM': 'RSEQ',
-    'Victoria': 'CW',
-    'Waterloo': 'OUA West',
-    'Western': 'OUA West',
-    'Windsor': 'OUA West',
-    'Winnipeg': 'CW',
-    'York': 'OUA Central'
-    }
-
-    #Create a DataFrame
-    df = pd.DataFrame(data_collected)
-
-    #remove rows with null vlaues
-    df = df[df['games_played'] != '-']
-
-    # Add a new column based on the dictionary
-    df['conference'] = df['team_name'].map(team_conference).astype('category')
-
-    #make new columns for fieldgoal_made and fieldgoal taken
-    df[['field_goal_made', 'field_goal_attempted']] = df['field_goals'].str.split('-', expand=True).astype(int)
-    df[['three_pointers_made', 'three_pointers_attempted']] = df['three_points'].str.split('-', expand=True).astype(int)
-    df[['free_throws_made', 'free_throws_attempted']] = df['free_throws'].str.split('-', expand=True).astype(int)
-    df[['field_goal_made_against', 'field_goal_attempted_against']] = df['field_goals_against'].str.split('-', expand=True).astype(int)
-    df[['three_pointers_made_against', 'three_pointers_attempted_against']] = df['three_points_against'].str.split('-', expand=True).astype(int)
-    #delete original field_goal and three point columns
-    df.drop(columns=['field_goals','three_points','free_throws','field_goals_against','three_points_against'], inplace=True)
-
-    # Convert columns to their respective data types
-    df['games_played'] = df['games_played'].astype(int)
-    df['field_goal_percentage'] = df['field_goal_percentage'].astype(float)
-    #df['three_points'] = df['three_points'].astype(str)
-    df['three_point_percentage'] = df['three_point_percentage'].astype(float)
-    #df['free_throws'] = df['free_throws'].astype(str)
-    df['free_throw_percentage'] = df['free_throw_percentage'].astype(float)
-    df['offensive_rebounds_per_game'] = df['offensive_rebounds_per_game'].astype(float)
-    df['defensive_rebounds_per_game'] = df['defensive_rebounds_per_game'].astype(float)
-    df['total_rebounds_per_game'] = df['total_rebounds_per_game'].astype(float)
-    df['assists_per_game'] = df['assists_per_game'].astype(float)
-    df['turnovers_per_game'] = df['turnovers_per_game'].astype(float)
-    df['steals_per_game'] = df['steals_per_game'].astype(float)
-    df['blocks_per_game'] = df['blocks_per_game'].astype(float)
-    df['team_fouls_per_game'] = df['team_fouls_per_game'].astype(float)
-    df['points_per_game'] = df['points_per_game'].astype(float)
-    #df['field_goals_against'] = df['field_goals_against'].astype(str)
-    df['field_goals_percentage_against'] = df['field_goals_percentage_against'].astype(float)
-    #df['three_points_against'] = df['three_points_against'].astype(str)
-    df['three_points_percentage_against'] = df['three_points_percentage_against'].astype(float)
-    df['offensive_rebounds_per_game_against'] = df['offensive_rebounds_per_game_against'].astype(float)
-    df['defensive_rebounds_per_game_against'] = df['defensive_rebounds_per_game_against'].astype(float)
-    df['total_rebounds_per_game_against'] = df['total_rebounds_per_game_against'].astype(float)
-    df['assists_per_game_against'] = df['assists_per_game_against'].astype(float)
-    df['turnovers_per_game_against'] = df['turnovers_per_game_against'].astype(float)
-    df['steals_per_game_against'] = df['steals_per_game_against'].astype(float)
-    df['blocks_per_game_against'] = df['blocks_per_game_against'].astype(float)
-    df['team_fouls_per_game_against'] = df['team_fouls_per_game_against'].astype(float)
-    df['points_per_game_against'] = df['points_per_game_against'].astype(float)
-    try:
-        df['offensive_efficiency'] = df['offensive_efficiency'].astype(float)
-        df['defensive_efficiency'] = df['defensive_efficiency'].astype(float)
-        df['Net_efficiency'] = df['Net_efficiency'].astype(float)
-    except:
-        print(f"Some team's_efficiency was not recorded")
-
-    #page from second url
-    page = requests.get(standings_url)
-   
-    if(page.status_code != 200):
-        print("USport's Server did not respond with HTTP request")
-
-    #parse html document
-    soup = BeautifulSoup(page.content, 'html.parser')
-
-    #initialize list to stroe data
-    team_names = []
-    total_wins = []
-    total_losses = []
-    win_percentage = []
-    last_ten_games = []
-    streak = []
-    league_points_for = []
-    league_points_against = []
-    league_points = []
-
-    # Find all <tr> blocks within <table> elements with class="stats-table"
-    tr_blocks = soup.select('table.stats-table tr')
-
-    # Iterate through each <tr> block
-    for block in tr_blocks:
-        # Check if the <tr> block contains a team name (i.e., <a> element)
-        team_name_element = block.select_one('td.stats-team a')
-        if team_name_element:
-            # Extract team name
-            team_names.append(team_name_element.text.strip())
-
-            #Extraact other stats
-            stats_elements = block.select('td')
-            total_wins.append(int(stats_elements[2].text.strip()))
-            total_losses.append(int(stats_elements[3].text.strip()))
-            win_percentage.append(float(stats_elements[4].text.strip()))
-            last_ten_games.append(stats_elements[5].text.strip())
-            streak.append(stats_elements[6].text.strip())
-            league_points_for.append(int(stats_elements[7].text.strip()))
-            league_points_against.append(int(stats_elements[8].text.strip()))
-            league_points.append(int(stats_elements[9].text.strip()))
-    
-    # Assuming last_ten_games contains a list of strings like "Won 3" or "Lost 2"
-    modified_streak = []
-
-    for game_result in streak:
-        if "Won" in game_result:
-            modified_streak.append("W" + game_result[3:])
-        elif "Lost" in game_result:
-            modified_streak.append("L" + game_result[4:])
-
-    data_collected = {
-    'team_name': team_names,
-    'total_wins': total_wins,
-    'total_losses': total_losses,
-    'win_percentage': win_percentage,
-    'last_ten_games': last_ten_games,
-    'streak' : modified_streak,
-    'total_points': league_points_for,
-    'total_points_against':league_points_against
-}
-    #Create a DataFrame
-    df2 = pd.DataFrame(data_collected)
-    df = pd.merge(df,df2,on='team_name', how='inner')
-    return df
-
-
-def usports_team_stats(arg:str) -> pd.DataFrame:
-    """
-    Fetches and processes team statistics data from USports website.
-
-    Args:
-        arg (str): Gender of the teams. Should be either 'men' or 'women'.
-
-    Returns:
-        pd.DataFrame: DataFrame containing processed team statistics.
-    """
-    if(arg.lower() == 'men'):
-        team = ('https://universitysport.prestosports.com/sports/mbkb/2023-24/teams?sort=&r=0&pos=off',
-             'https://universitysport.prestosports.com/sports/mbkb/2023-24/standings-conf', 52)
-    elif(arg.lower() == 'women'):
-        team = ('https://universitysport.prestosports.com/sports/wbkb/2023-24/teams?sort=&r=0&pos=off',
-               'https://universitysport.prestosports.com/sports/wbkb/2023-24/standings-conf', 48)
-    team_stats_df = __usports_team_data(team[0], team[1], team[2])
+#importing libraries
+import requests
+from bs4 import BeautifulSoup
+import pandas as pd
+
+def __usports_team_data(stats_url: str, standings_url: str, no_of_teams: int) -> pd.DataFrame:
+    '''
+    This function takes the URL of the USport's team stats and the number of teams and returns a
+    DataFrame of the team and their stats, removing any rows of teams that didn't play that season.
+
+    Args:
+        stats_url (str): URL of the team statistics data.
+        standings_url (str): URL of the standings page.
+        no_of_teams (int): Number of teams.
+
+    Returns:
+        pd.DataFrame: DataFrame containing processed team statistics.
+    '''
+    #perfrom GET request to the URL and returns the server response to the HTTP request
+    page = requests.get(stats_url)
+   
+    if(page.status_code != 200):
+        print("USport's Server did not respond with HTTP request")
+
+    #parse html document
+    soup = BeautifulSoup(page.content, 'html.parser')
+
+    #Find the table containing stats
+    rows = soup.find_all('tr')
+    
+    #Intialize lists to store data
+    team_names =[]
+    games_played = []
+    field_goals = []
+    field_goal_percentage = []
+    three_pointers = []
+    three_point_percentage = []
+    free_throws = []
+    free_throw_percentage = []
+    off_rebounds_per_game = []
+    def_rebounds_per_game = []
+    total_rebounds_per_game = []
+    assists_per_game = []
+    turnovers_per_game = []
+    steals_per_game = []
+    blocks_per_game = []
+    fouls_per_game = []
+    points_per_game = []
+    off_efficiency = []
+    net_efficiency = []
+    field_goals_against = []
+    field_goal_against_percentage = []
+    three_pointers_against = []
+    three_point_against_percentage = []
+    off_rebounds_per_game_against = []
+    def_rebounds_per_game_against = []
+    total_rebounds_per_game_against = []
+    assists_per_game_against = []
+    turnovers_per_game_against = []
+    steals_per_game_against = []
+    blocks_per_game_against = []
+    fouls_per_game_against = []
+    points_per_game_against = []
+    def_efficiency = []
+
+    #Loop through each row(skip the first row as it's the header)
+    for index, row in enumerate(rows[1:]):
+
+        #exit loop when we reached end of table
+        if index >= no_of_teams:
+            break
+
+        #Extract team name
+        school_name = row.find('td', class_='pinned-col text').text.strip()
+   
+        team_names.append(school_name)
+
+        #Extract data from other columns
+        columns = row.find_all('td', align = 'center')
+        games_played.append(columns[0].text.strip())
+        field_goals.append(columns[1].text.strip())
+        field_goal_percentage.append(columns[2].text.strip())
+        three_pointers.append(columns[3].text.strip())
+        three_point_percentage.append(columns[4].text.strip())
+        free_throws.append(columns[5].text.strip())
+        free_throw_percentage.append(columns[6].text.strip())
+        off_rebounds_per_game.append(columns[7].text.strip())
+        def_rebounds_per_game.append(columns[8].text.strip())
+        total_rebounds_per_game.append(columns[9].text.strip())
+        assists_per_game.append(columns[10].text.strip())
+        turnovers_per_game.append(columns[11].text.strip())
+        steals_per_game.append(columns[12].text.strip())
+        blocks_per_game.append(columns[13].text.strip())
+        fouls_per_game.append(columns[14].text.strip())
+        points_per_game.append(columns[15].text.strip())
+        off_efficiency.append(columns[16].text.strip())
+        net_efficiency.append(columns[17].text.strip())
+
+    #Loop through defensive stats row (skip first row(header) and second row which contains game played)
+    for index, row in enumerate(rows[no_of_teams+2:]):
+        
+        #exit loop when we reached end of table
+        if index >= no_of_teams:
+            break
+
+        #Extract data from other columns
+        columns = row.find_all('td', align = 'center')
+        field_goals_against.append(columns[1].text.strip())
+        field_goal_against_percentage.append(columns[2].text.strip())
+        three_pointers_against.append(columns[3].text.strip())
+        three_point_against_percentage.append(columns[4].text.strip())
+        off_rebounds_per_game_against.append(columns[5].text.strip())
+        def_rebounds_per_game_against.append(columns[6].text.strip())
+        total_rebounds_per_game_against.append(columns[7].text.strip())
+        assists_per_game_against.append(columns[9].text.strip())
+        turnovers_per_game_against.append(columns[10].text.strip())
+        steals_per_game_against.append(columns[11].text.strip())
+        blocks_per_game_against.append(columns[12].text.strip())
+        fouls_per_game_against.append(columns[13].text.strip())
+        points_per_game_against.append(columns[14].text.strip())
+        def_efficiency.append(columns[15].text.strip())   
+
+    data_collected = {
+        'team_name': team_names,
+        'games_played': games_played,
+        'points_per_game': points_per_game,
+        'field_goals': field_goals,
+        'field_goal_percentage': field_goal_percentage,
+        'three_points': three_pointers,
+        'three_point_percentage': three_point_percentage,
+        'free_throws': free_throws,
+        'free_throw_percentage': free_throw_percentage,
+        'offensive_rebounds_per_game': off_rebounds_per_game,
+        'defensive_rebounds_per_game': def_rebounds_per_game,
+        'total_rebounds_per_game': total_rebounds_per_game,
+        'assists_per_game' : assists_per_game,
+        'turnovers_per_game': turnovers_per_game,
+        'steals_per_game': steals_per_game,
+        'blocks_per_game': blocks_per_game,
+        'team_fouls_per_game': fouls_per_game,
+        'offensive_efficiency': off_efficiency,
+        'defensive_efficiency': def_efficiency,
+        'Net_efficiency': net_efficiency,
+        'field_goals_against': field_goals_against,
+        'field_goals_percentage_against': field_goal_against_percentage,
+        'three_points_against': three_pointers_against,
+        'three_points_percentage_against': three_point_against_percentage,
+        'offensive_rebounds_per_game_against': off_rebounds_per_game_against,
+        'defensive_rebounds_per_game_against': def_rebounds_per_game_against,
+        'total_rebounds_per_game_against': total_rebounds_per_game_against,
+        'assists_per_game_against': assists_per_game_against,
+        'turnovers_per_game_against': turnovers_per_game_against,
+        'steals_per_game_against': steals_per_game_against,
+        'blocks_per_game_against': blocks_per_game_against,
+        'team_fouls_per_game_against': fouls_per_game_against,
+        'points_per_game_against': points_per_game_against
+        }
+    
+    
+    #create dictionary that maps university sports team to respective conference
+    team_conference = {
+    'Acadia': 'AUS',
+    'Alberta': 'CW',
+    'Algoma': 'OUA West',
+    'Bishop\'s': 'RSEQ',
+    'Brandon': 'CW',
+    'Brock': 'OUA Central',
+    'Calgary': 'CW',
+    'Cape Breton': 'AUS',
+    'Carleton': 'OUA East',
+    'Concordia': 'RSEQ',
+    'Dalhousie': 'AUS',
+    'Guelph': 'OUA West',
+    'Lakehead': 'OUA Central',
+    'Laurentian': 'OUA East',
+    'Laurier': 'OUA West',
+    'Laval': 'RSEQ',
+    'Lethbridge': 'CW',
+    'MacEwan': 'CW',
+    'Manitoba': 'CW',
+    'McGill': 'RSEQ',
+    'McMaster': 'OUA Central',
+    'Memorial': 'AUS',
+    'Mount Royal': 'CW',
+    'Nipissing': 'OUA East',
+    'Ontario Tech': 'OUA East',
+    'Ottawa': 'OUA East',
+    'Queen\'s': 'OUA East',
+    'Regina': 'CW',
+    'Saint Mary\'s': 'AUS',
+    'Saskatchewan': 'CW',
+    'StFX': 'AUS',
+    'Thompson Rivers': 'CW',
+    'Toronto': 'OUA Central',
+    'Toronto Metropolitan': 'OUA Central',
+    'Trinity Western': 'CW',
+    'UBC': 'CW',
+    'UBC Okanagan': 'CW',
+    'UFV': 'CW',
+    'UNB': 'AUS',
+    'UNBC': 'CW',
+    'UPEI': 'AUS',
+    'UQAM': 'RSEQ',
+    'Victoria': 'CW',
+    'Waterloo': 'OUA West',
+    'Western': 'OUA West',
+    'Windsor': 'OUA West',
+    'Winnipeg': 'CW',
+    'York': 'OUA Central'
+    }
+
+    #Create a DataFrame
+    df = pd.DataFrame(data_collected)
+
+    #remove rows with null vlaues
+    df = df[df['games_played'] != '-']
+
+    # Add a new column based on the dictionary
+    df['conference'] = df['team_name'].map(team_conference).astype('category')
+
+    #make new columns for fieldgoal_made and fieldgoal taken
+    df[['field_goal_made', 'field_goal_attempted']] = df['field_goals'].str.split('-', expand=True).astype(int)
+    df[['three_pointers_made', 'three_pointers_attempted']] = df['three_points'].str.split('-', expand=True).astype(int)
+    df[['free_throws_made', 'free_throws_attempted']] = df['free_throws'].str.split('-', expand=True).astype(int)
+    df[['field_goal_made_against', 'field_goal_attempted_against']] = df['field_goals_against'].str.split('-', expand=True).astype(int)
+    df[['three_pointers_made_against', 'three_pointers_attempted_against']] = df['three_points_against'].str.split('-', expand=True).astype(int)
+    #delete original field_goal and three point columns
+    df.drop(columns=['field_goals','three_points','free_throws','field_goals_against','three_points_against'], inplace=True)
+
+    # Convert columns to their respective data types
+    df['games_played'] = df['games_played'].astype(int)
+    df['field_goal_percentage'] = df['field_goal_percentage'].astype(float)
+    #df['three_points'] = df['three_points'].astype(str)
+    df['three_point_percentage'] = df['three_point_percentage'].astype(float)
+    #df['free_throws'] = df['free_throws'].astype(str)
+    df['free_throw_percentage'] = df['free_throw_percentage'].astype(float)
+    df['offensive_rebounds_per_game'] = df['offensive_rebounds_per_game'].astype(float)
+    df['defensive_rebounds_per_game'] = df['defensive_rebounds_per_game'].astype(float)
+    df['total_rebounds_per_game'] = df['total_rebounds_per_game'].astype(float)
+    df['assists_per_game'] = df['assists_per_game'].astype(float)
+    df['turnovers_per_game'] = df['turnovers_per_game'].astype(float)
+    df['steals_per_game'] = df['steals_per_game'].astype(float)
+    df['blocks_per_game'] = df['blocks_per_game'].astype(float)
+    df['team_fouls_per_game'] = df['team_fouls_per_game'].astype(float)
+    df['points_per_game'] = df['points_per_game'].astype(float)
+    #df['field_goals_against'] = df['field_goals_against'].astype(str)
+    df['field_goals_percentage_against'] = df['field_goals_percentage_against'].astype(float)
+    #df['three_points_against'] = df['three_points_against'].astype(str)
+    df['three_points_percentage_against'] = df['three_points_percentage_against'].astype(float)
+    df['offensive_rebounds_per_game_against'] = df['offensive_rebounds_per_game_against'].astype(float)
+    df['defensive_rebounds_per_game_against'] = df['defensive_rebounds_per_game_against'].astype(float)
+    df['total_rebounds_per_game_against'] = df['total_rebounds_per_game_against'].astype(float)
+    df['assists_per_game_against'] = df['assists_per_game_against'].astype(float)
+    df['turnovers_per_game_against'] = df['turnovers_per_game_against'].astype(float)
+    df['steals_per_game_against'] = df['steals_per_game_against'].astype(float)
+    df['blocks_per_game_against'] = df['blocks_per_game_against'].astype(float)
+    df['team_fouls_per_game_against'] = df['team_fouls_per_game_against'].astype(float)
+    df['points_per_game_against'] = df['points_per_game_against'].astype(float)
+    try:
+        df['offensive_efficiency'] = df['offensive_efficiency'].astype(float)
+        df['defensive_efficiency'] = df['defensive_efficiency'].astype(float)
+        df['Net_efficiency'] = df['Net_efficiency'].astype(float)
+    except:
+        print(f"Some team's_efficiency was not recorded")
+
+    #page from second url
+    page = requests.get(standings_url)
+   
+    if(page.status_code != 200):
+        print("USport's Server did not respond with HTTP request")
+
+    #parse html document
+    soup = BeautifulSoup(page.content, 'html.parser')
+
+    #initialize list to stroe data
+    team_names = []
+    total_wins = []
+    total_losses = []
+    win_percentage = []
+    last_ten_games = []
+    streak = []
+    league_points_for = []
+    league_points_against = []
+    league_points = []
+
+    # Find all <tr> blocks within <table> elements with class="stats-table"
+    tr_blocks = soup.select('table.stats-table tr')
+
+    # Iterate through each <tr> block
+    for block in tr_blocks:
+        # Check if the <tr> block contains a team name (i.e., <a> element)
+        team_name_element = block.select_one('td.stats-team a')
+        if team_name_element:
+            # Extract team name
+            team_names.append(team_name_element.text.strip())
+
+            #Extraact other stats
+            stats_elements = block.select('td')
+            total_wins.append(int(stats_elements[2].text.strip()))
+            total_losses.append(int(stats_elements[3].text.strip()))
+            win_percentage.append(float(stats_elements[4].text.strip()))
+            last_ten_games.append(stats_elements[5].text.strip())
+            streak.append(stats_elements[6].text.strip())
+            league_points_for.append(int(stats_elements[7].text.strip()))
+            league_points_against.append(int(stats_elements[8].text.strip()))
+            league_points.append(int(stats_elements[9].text.strip()))
+    
+    # Assuming last_ten_games contains a list of strings like "Won 3" or "Lost 2"
+    modified_streak = []
+
+    for game_result in streak:
+        if "Won" in game_result:
+            modified_streak.append("W" + game_result[3:])
+        elif "Lost" in game_result:
+            modified_streak.append("L" + game_result[4:])
+
+    data_collected = {
+    'team_name': team_names,
+    'total_wins': total_wins,
+    'total_losses': total_losses,
+    'win_percentage': win_percentage,
+    'last_ten_games': last_ten_games,
+    'streak' : modified_streak,
+    'total_points': league_points_for,
+    'total_points_against':league_points_against
+}
+    #Create a DataFrame
+    df2 = pd.DataFrame(data_collected)
+    df = pd.merge(df,df2,on='team_name', how='inner')
+    return df
+
+
+def usports_team_stats(arg:str) -> pd.DataFrame:
+    """
+    Fetches and processes team statistics data from USports website.
+
+    Args:
+        arg (str): Gender of the teams. Should be either 'men' or 'women'.
+
+    Returns:
+        pd.DataFrame: DataFrame containing processed team statistics.
+    """
+    if(arg.lower() == 'men'):
+        team = ('https://universitysport.prestosports.com/sports/mbkb/2023-24/teams?sort=&r=0&pos=off',
+             'https://universitysport.prestosports.com/sports/mbkb/2023-24/standings-conf', 52)
+    elif(arg.lower() == 'women'):
+        team = ('https://universitysport.prestosports.com/sports/wbkb/2023-24/teams?sort=&r=0&pos=off',
+               'https://universitysport.prestosports.com/sports/wbkb/2023-24/standings-conf', 48)
+    team_stats_df = __usports_team_data(team[0], team[1], team[2])
     return team_stats_df
```

### Comparing `usports_basketball-0.0.3/usports_basketball.egg-info/PKG-INFO` & `usports_basketball-1.0.0/usports_basketball.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,108 @@
-Metadata-Version: 2.1
-Name: usports-basketball
-Version: 0.0.3
-Summary: A Python package for USports basketball stats.
-Author-email: OJ Adeyemi <ojieadeyemi@gmail.com>
-Maintainer-email: OJ Adeyemi <ojieadeyemi@gmail.com>
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: beautifulsoup4>=4.12.0
-Requires-Dist: pandas>=2.2.0
-
-# USports Basketball Statistics Package
-
-## Introduction
-
-The USports Basketball Statistics Package is a Python package designed to retrieve and analyze basketball statistics data from the USports website. This package provides functions for web scraping and processing both team and player statistics, allowing users to gather data for analysis and insights.
-
-## Installation
-
-You can install the package via pip:
-
-```bash
-pip install usports-basketball
-```
-
-## Dependencies
-
-This package relies on the following dependencies:
-- requests
-- BeautifulSoup (bs4)
-- pandas
-
-Make sure you have these dependencies installed before using the package.
-
-## Functions
-
-### `usports_team_stats`
-
-This function fetches and processes team statistics data, including standings, win-loss totals, shooting percentages, and other relevant team metrics for the current USports basketball season.
-
-#### Parameters
-
-- `league` (str): The conference for which you want to retrieve team statistics. Valid values are `'men'` and `'women'`.
-
-#### Returns
-
-- `DataFrame`: A pandas DataFrame containing the team statistics data.
-
-### `usports_player_stats`
-
-This function fetches and processes player statistics data, including total games played, points scored, shooting percentages, rebounds, assists, turnovers, steals, blocks, and other individual player metrics for the current USports basketball season.
-
-#### Parameters
-
-- `league` (str): The conference for which you want to retrieve player statistics. Valid values are `'men'` and `'women'`.
-
-#### Returns
-
-- `DataFrame`: A pandas DataFrame containing the player statistics data.
-
-## Example Usage
-
-```python
-from usports_basketball import usports_team_stats, usports_player_stats
-
-# Fetching and processing men's team statistics
-men_team_stats_df = usports_team_stats('men')
-
-# Fetching and processing men's player statistics
-men_player_stats_df = usports_player_stats('men')
-```
-
-## Note
-
-- This package is based on the current USports basketball season only. To access statistics from previous seasons, manual adjustments to the web scraping code may be required.
-
-## Author
-
-This package was developed by OJ Adeyemi.
-
-## Contributing
-
-Contributions, bug reports, and feature requests are welcome! Please feel free to open an issue or submit a pull request on [GitHub](https://github.com/ojadeyemi/usports-basketball).
-
-## License
-
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
-for details.
+Metadata-Version: 2.1
+Name: usports-basketball
+Version: 1.0.0
+Summary: A Python package for USports basketball stats.
+Author-email: OJ Adeyemi <ojieadeyemi@gmail.com>
+Maintainer-email: OJ Adeyemi <ojieadeyemi@gmail.com>
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: requests>=2.31.0
+Requires-Dist: beautifulsoup4>=4.12.0
+Requires-Dist: pandas>=2.2.0
+
+# USports Basketball Statistics Package
+
+## Introduction
+
+The USports Basketball Statistics Package is a Python package designed to retrieve and analyze basketball statistics data from the USports website. This package provides functions for web scraping and processing both team and player statistics, allowing users to gather data for analysis and insights.
+
+## Installation
+
+You can install the package via pip:
+
+```bash
+pip install usports-basketball
+```
+
+## Dependencies
+
+This package relies on the following dependencies:
+- requests
+- BeautifulSoup (bs4)
+- pandas
+
+Make sure you have these dependencies installed before using the package.
+
+## Functions
+
+### `usports_team_stats`
+
+This function fetches and processes team statistics data, including standings, win-loss totals, shooting percentages, and other relevant team metrics for the current USports basketball season.
+
+#### Parameters
+
+- `arg` (str): The conference for which you want to retrieve team statistics. Valid values are `'men'` and `'women'`.
+
+#### Returns
+
+- `DataFrame`: A pandas DataFrame containing the team statistics data.
+
+### `usports_player_stats`
+
+This function fetches and processes player statistics data, including total games played, points scored, shooting percentages, rebounds, assists, turnovers, steals, blocks, and other individual player metrics for the current USports basketball season.
+
+#### Parameters
+
+- `arg` (str): The conference for which you want to retrieve player statistics. Valid values are `'men'` and `'women'`.
+
+#### Returns
+
+- `DataFrame`: A pandas DataFrame containing the player statistics data.
+
+## Example Usage
+
+```python
+from usports_basketball import usports_team_stats, usports_player_stats
+
+# Fetching and processing men's team statistics
+men_team_stats_df = usports_team_stats('men')
+
+# Fetching and processing men's player statistics
+men_player_stats_df = usports_player_stats('men')
+```
+
+You can use the `.dtype` function to retrieve the data types of all columns in the DataFrame. This can be useful for understanding the structure of the data you've fetched. Here's how you can use it:
+
+```python
+# Assuming `usports_player_stats` returns a DataFrame named `men_player_stats_df`
+# Fetching and processing men's player statistics
+men_player_stats_df = usports_player_stats('men')
+
+# Get the data types of all columns with their column names
+column_dtypes = men_player_stats_df.dtypes
+
+# Print the column names and their corresponding data types
+print(column_dtypes)
+```
+
+## Note
+
+- This package is based on the current USports basketball season only. To access statistics from previous seasons, manual adjustments to the web scraping code may be required.
+
+## Author
+
+This package was developed by OJ Adeyemi.
+
+## Contributing
+
+Contributions, bug reports, and feature requests are welcome! Please feel free to open an issue or submit a pull request on [GitHub](https://github.com/ojadeyemi/usports-basketball).
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
+for details.
```

