# Comparing `tmp/usports_basketball-1.0.0.tar.gz` & `tmp/usports_basketball-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usports_basketball-1.0.0.tar", last modified: Thu May  2 22:05:04 2024, max compression
+gzip compressed data, was "usports_basketball-1.0.1.tar", last modified: Fri May  3 19:21:45 2024, max compression
```

## Comparing `usports_basketball-1.0.0.tar` & `usports_basketball-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.125507 usports_basketball-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.125507 usports_basketball-1.0.0/usports_basketball/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/usports_basketball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/usports_basketball/player_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14902 2024-05-02 22:04:52.000000 usports_basketball-1.0.0/usports_basketball/team_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:05:04.129507 usports_basketball-1.0.0/usports_basketball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 22:05:04.000000 usports_basketball-1.0.0/usports_basketball.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:45.058806 usports_basketball-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-03 19:21:45.058806 usports_basketball-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:21:45.058806 usports_basketball-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:45.058806 usports_basketball-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:45.058806 usports_basketball-1.0.1/usports_basketball/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/usports_basketball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/usports_basketball/player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-05-03 19:21:40.000000 usports_basketball-1.0.1/usports_basketball/team_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:45.058806 usports_basketball-1.0.1/usports_basketball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-03 19:21:45.000000 usports_basketball-1.0.1/usports_basketball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-03 19:21:45.000000 usports_basketball-1.0.1/usports_basketball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:21:45.000000 usports_basketball-1.0.1/usports_basketball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 19:21:45.000000 usports_basketball-1.0.1/usports_basketball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 19:21:45.000000 usports_basketball-1.0.1/usports_basketball.egg-info/top_level.txt
```

### Comparing `usports_basketball-1.0.0/pyproject.toml` & `usports_basketball-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "usports-basketball"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python package for USports basketball stats."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "OJ Adeyemi", email = "ojieadeyemi@gmail.com"}]
 maintainers = [{name = "OJ Adeyemi", email = "ojieadeyemi@gmail.com"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `usports_basketball-1.0.0/test/test.py` & `usports_basketball-1.0.1/test/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,46 @@
-import pytest
-
+""" BASIC TESTS"""
 import pandas as pd
 
 from usports_basketball import usports_team_stats, usports_player_stats
 
 def test_usports_team_stats_returns_dataframe():
+    """Test if usports_team_stats function returns a pandas DataFrame."""
     team_stats_df = usports_team_stats('men')
     assert isinstance(team_stats_df, pd.DataFrame)
 
 def test_usports_player_stats_returns_dataframe():
+    """Test if usports_player_stats function returns a pandas DataFrame."""
     player_stats_df = usports_player_stats('women')
     assert isinstance(player_stats_df, pd.DataFrame)
 
 def test_usports_team_stats_non_empty():
+    """Test if usports_team_stats function returns a non-empty DataFrame."""
     team_stats_df = usports_team_stats('women')
     assert not team_stats_df.empty, "Team statistics DataFrame is empty"
 
 def test_usports_player_stats_non_empty():
+    """Test if usports_player_stats function returns a non-empty DataFrame."""
     player_stats_df = usports_player_stats('men')
     assert not player_stats_df.empty, "Player statistics DataFrame is empty"
 
 def test_usports_team_stats_columns():
+    """Test if usports_team_stats function returns the expected columns."""
     team_stats_df = usports_team_stats('men')
     expected_columns = [
         'team_name',
         'games_played',
         # Add more expected columns as needed
     ]
     assert all(column in team_stats_df.columns for column in expected_columns), "Missing columns in team statistics DataFrame"
 
 def test_usports_player_stats_columns():
+    """Test if usports_player_stats function returns the expected columns."""
     player_stats_df = usports_player_stats('men')
     expected_columns = [
         'lastname_initials',
         'first_name',
         # Add more expected columns as needed
     ]
-    assert all(column in player_stats_df.columns for column in expected_columns), "Missing columns in player statistics DataFrame"
-
+    actual_columns = player_stats_df.columns.tolist()
+    for column in expected_columns:
+        assert column in actual_columns, f"Expected column '{column}' not found in player_stats_df"
```

### Comparing `usports_basketball-1.0.0/usports_basketball/__init__.py` & `usports_basketball-1.0.1/usports_basketball/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 
 """
 USports Basketball Statistics Web Scraping and Processing Package
 
-This package provides functions for web scraping and processing basketball statistics data from the USports website. It encompasses functionality for retrieving both team and player statistics.
+This package provides functions for web scraping and processing basketball statistics data from the USports website.
+ It encompasses functionality for retrieving both team and player statistics.
 
 Dependencies:
     - requests
     - BeautifulSoup (bs4)
     - pandas
     
 Functions:
-- usports_team_stats: Fetches and processes team statistics data, including standings, win-loss totals, and other relevant team metrics.
-- usports_player_stats: Fetches and processes player statistics data, including total games played, total points scored, field goal percentage, and other individual player metrics.
+- usports_team_stats:  Retrieves and handles team statistics such as standings, win-loss records, and key team metrics.
+- usports_player_stats:  Retrieves and processes player statistics like points scored, field goal percentage, and other individual player metrics.
 
 These functions return pandas DataFrames containing the respective statistics data.
-Note: This is based on current season only, to get stats from previous season you'll need to manually make changes in both team and players webscraping files
+Note: This is based on current season only.
+For previous season's stats, adjustment to both team and player scraping files are needed.
 
 # Example:
 >>> from usportsbballstats import usports_team_stats, usports_player_stats
 #Fetching and processing men's team and players statistics 
 >>> men_team_stats_df = usports_team_stats('men')
 # Fetching and processing player statistics data for men's players
 >>> men_player_stats_df = usports_player_stats('men') \n
@@ -27,8 +29,7 @@
     OJ Adeyemi
 
 Date Created:
     March 1, 2024
 """
 from .team_stats import usports_team_stats
 from .player_stats import usports_player_stats
-
```

### Comparing `usports_basketball-1.0.0/usports_basketball/player_stats.py` & `usports_basketball-1.0.1/usports_basketball/player_stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,47 @@
+"""
+Module for fetching and processing player statistics data from the current U Sports basketball league season.
+
+This module provides functions to retrieve player statistics, including both offense and defense data,
+from the current U Sports basketball league season for both men's and women's leagues. 
+It utilizes web scraping techniques to extract data from the U Sports website 
+and processes it into pandas DataFrames for further analysis.
+
+Functions:
+- __usports_player_offense_data(offense_url:str) -> pd.DataFrame:
+    Fetches and processes player offense statistics data from the given URL.
+
+- __usports_player_defense_data(defense_url:str) -> pd.DataFrame:
+    Fetches and processes player defense statistics data from the given URL.
+
+- usports_player_stats(arg:str) -> pd.DataFrame:
+    Fetches and processes player statistics data from the U Sports website based on the specified gender.
+Author:
+    OJ Adeyemi
+
+Date Created:
+    March 1, 2024
+"""
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 
 def __usports_player_offense_data(offense_url:str) -> pd.DataFrame:
     """
     Fetches and processes player offense statistics data from the given URL.
 
     Args:
         offense_url (str): URL of the player offense statistics data.
 
     Returns:
         pd.DataFrame: DataFrame containing processed player offense statistics.
     """ 
-    offense_page = requests.get(offense_url)
+    offense_page = requests.get(offense_url, timeout=10)
 
     # Parse the HTML using BeautifulSoup
-   
     offense_soup = BeautifulSoup(offense_page.content, 'html.parser')
 
     offense_rows = offense_soup.find_all('tr')
 
     # Initialize lists to store data
     data = {
         'lastname_initials': [],
@@ -37,16 +59,18 @@
         'free_throws_percentage': [],
         'total_points': [],
     }
     # Iterate through each row
     for row in offense_rows:
         cols = row.find_all('td')  # Find all <td> tags with class 'text'
         if len(cols) > 0:
-            player_lastname_initials = cols[1].get_text(strip=True).split()[0]  # Assuming lastname initials are the first letter of the second <td> content
-            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  # Assuming firstname is the rest of the content after lastname initials
+            # Assuming lastname initials are the first letter of the second <td> content
+            player_lastname_initials = cols[1].get_text(strip=True).split()[0] 
+            # Assuming firstname is the rest of the content after lastname initials
+            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  
             school = cols[2].get_text(strip=True)
             minutes_played = cols[5].get_text(strip=True)
             field_goals_made, field_goals_attempted = cols[6].get_text(strip=True).split('-')
             field_goal_percentage = cols[7].get_text(strip=True)
             three_points_made,three_points_attempted = cols[8].get_text(strip=True).split('-')
             three_points_percentage = cols[9].get_text(strip=True)
             free_throws_made,free_throws_attempted = cols[10].get_text(strip=True).split('-')
@@ -80,18 +104,17 @@
 
     Args:
         defense_url (str): URL of the player defense statistics data.
 
     Returns:
         pd.DataFrame: DataFrame containing processed player defense statistics.
     """ 
-    defense_page = requests.get(defense_url)
+    defense_page = requests.get(defense_url, timeout=10)
 
     # Parse the HTML using BeautifulSoup
-   
     defense_soup = BeautifulSoup(defense_page.content, 'html.parser')
 
     # Initialize lists to store data
     data = {
         'lastname_initials': [],
         'first_name': [],
         'school': [],
@@ -113,16 +136,18 @@
     # Find all <tr> tags
     defense_rows = defense_soup.find_all('tr')
 
     # Iterate through each row
     for row in defense_rows:
         cols = row.find_all('td')  # Find all <td> tags with class 'text'
         if len(cols) > 0:
-            player_lastname_initials = cols[1].get_text(strip=True).split()[0]  # Assuming lastname initials are the first letter of the second <td> content
-            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:])  # Assuming firstname is the rest of the content after lastname initials
+            # Assuming lastname initials are the first letter of the second <td> content
+            player_lastname_initials = cols[1].get_text(strip=True).split()[0]
+            # Assuming firstname is the rest of the content after lastname initials  
+            firstname = ' '.join(cols[1].get_text(strip=True).split()[1:]) 
             school = cols[2].get_text(strip=True)
             games_played = cols[3].get_text(strip=True)
             games_started = cols[4].get_text(strip=True)
             minutes_played = cols[5].get_text(strip=True)
             off_reb = cols[6].get_text(strip=True)
             def_reb = cols[7].get_text(strip=True)
             total_reb = cols[8].get_text(strip=True)
@@ -166,23 +191,25 @@
 
     Args:
         arg (str): Gender of the players. Should be either 'men' or 'women'.
 
     Returns:
         pd.DataFrame: DataFrame containing processed player statistics.
     """
-    if(arg == 'men'):
-            players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=st&r=0')
-            players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=bt&r=0')
-    elif (arg == 'women'):
+    if arg == 'men':
+        players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=st&r=0')
+        players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/mbkb/2023-24/players?view=&pos=bt&r=0')
+    elif arg == 'women':
         players_off_stats_df = __usports_player_offense_data('https://universitysport.prestosports.com/sports/wbkb/2023-24/players?view=&pos=st&r=0')
         players_def_stats_df = __usports_player_defense_data('https://universitysport.prestosports.com/sports/wbkb/2023-24/players?view=&pos=bt&r=0')
+    else:
+        raise ValueError("In correct argument . options are: \'men\' or \'women\'")
 
-    players_stats_df = pd.merge(players_def_stats_df, players_off_stats_df, on=['lastname_initials','first_name','school', 'minutes_played'], how='inner')
-    
+    players_stats_df = pd.merge(players_def_stats_df, players_off_stats_df, 
+                        on=['lastname_initials','first_name','school', 'minutes_played'], how='inner')
     players_stats_df['games_played'] = pd.to_numeric(players_stats_df['games_played'], errors='coerce').fillna(0).astype(int)
     players_stats_df['games_started'] = pd.to_numeric(players_stats_df['games_started'], errors='coerce').fillna(0).astype(int)
     players_stats_df['minutes_played'] = pd.to_numeric(players_stats_df['minutes_played'], errors='coerce').fillna(0).astype(int)
     players_stats_df['offensive_rebounds'] = pd.to_numeric(players_stats_df['offensive_rebounds'], errors='coerce').fillna(0).astype(int)
     players_stats_df['defensive_rebounds'] = pd.to_numeric(players_stats_df['defensive_rebounds'], errors='coerce').fillna(0).astype(int)
     players_stats_df['total_rebounds'] = pd.to_numeric(players_stats_df['total_rebounds'], errors='coerce').fillna(0).astype(int)
     players_stats_df['personal_fouls'] = pd.to_numeric(players_stats_df['personal_fouls'], errors='coerce').fillna(0).astype(int)
@@ -199,8 +226,8 @@
     players_stats_df['three_pointers_attempted'] = pd.to_numeric(players_stats_df['three_pointers_attempted'], errors='coerce').fillna(0).astype(int)
     players_stats_df['three_pointers_percentage'] = pd.to_numeric(players_stats_df['three_pointers_percentage'], errors='coerce').fillna(0).astype(float)
     players_stats_df['free_throws_made'] = pd.to_numeric(players_stats_df['free_throws_made'], errors='coerce').fillna(0).astype(int)
     players_stats_df['free_throws_attempted'] = pd.to_numeric(players_stats_df['free_throws_attempted'], errors='coerce').fillna(0).astype(int)
     players_stats_df['free_throws_percentage'] = pd.to_numeric(players_stats_df['free_throws_percentage'], errors='coerce').fillna(0).astype(float)
     players_stats_df['total_points'] = pd.to_numeric(players_stats_df['total_points'], errors='coerce').fillna(0).astype(int)
 
-    return players_stats_df
+    return players_stats_df
```

### Comparing `usports_basketball-1.0.0/usports_basketball/team_stats.py` & `usports_basketball-1.0.1/usports_basketball/team_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-#importing libraries
+"""
+Module for fetching and processing team statistics data from the current U Sports basketball league season.
+
+This module provides functions to retrieve team statistics from the current U Sports basketball league season for both men's and women's leagues.
+ It utilizes web scraping techniques to extract data from the U Sports website and processes it into pandas DataFrames for further analysis.
+
+Functions:
+- __usports_team_data(stats_url: str, standings_url: str, no_of_teams: int) -> pd.DataFrame:
+    Fetches and processes team statistics data from the given URLs and the specified number of teams.
+
+- usports_team_stats(arg:str) -> pd.DataFrame:
+    Fetches and processes team statistics data from the U Sports website based on the specified gender.
+"""
+
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 
 def __usports_team_data(stats_url: str, standings_url: str, no_of_teams: int) -> pd.DataFrame:
     '''
     This function takes the URL of the USport's team stats and the number of teams and returns a
@@ -13,17 +26,17 @@
         standings_url (str): URL of the standings page.
         no_of_teams (int): Number of teams.
 
     Returns:
         pd.DataFrame: DataFrame containing processed team statistics.
     '''
     #perfrom GET request to the URL and returns the server response to the HTTP request
-    page = requests.get(stats_url)
+    page = requests.get(stats_url, timeout=10)
    
-    if(page.status_code != 200):
+    if page.status_code != 200:
         print("USport's Server did not respond with HTTP request")
 
     #parse html document
     soup = BeautifulSoup(page.content, 'html.parser')
 
     #Find the table containing stats
     rows = soup.find_all('tr')
@@ -93,16 +106,15 @@
         blocks_per_game.append(columns[13].text.strip())
         fouls_per_game.append(columns[14].text.strip())
         points_per_game.append(columns[15].text.strip())
         off_efficiency.append(columns[16].text.strip())
         net_efficiency.append(columns[17].text.strip())
 
     #Loop through defensive stats row (skip first row(header) and second row which contains game played)
-    for index, row in enumerate(rows[no_of_teams+2:]):
-        
+    for index, row in enumerate(rows[no_of_teams+2:]):        
         #exit loop when we reached end of table
         if index >= no_of_teams:
             break
 
         #Extract data from other columns
         columns = row.find_all('td', align = 'center')
         field_goals_against.append(columns[1].text.strip())
@@ -152,15 +164,14 @@
         'turnovers_per_game_against': turnovers_per_game_against,
         'steals_per_game_against': steals_per_game_against,
         'blocks_per_game_against': blocks_per_game_against,
         'team_fouls_per_game_against': fouls_per_game_against,
         'points_per_game_against': points_per_game_against
         }
     
-    
     #create dictionary that maps university sports team to respective conference
     team_conference = {
     'Acadia': 'AUS',
     'Alberta': 'CW',
     'Algoma': 'OUA West',
     'Bishop\'s': 'RSEQ',
     'Brandon': 'CW',
@@ -253,24 +264,25 @@
     df['assists_per_game_against'] = df['assists_per_game_against'].astype(float)
     df['turnovers_per_game_against'] = df['turnovers_per_game_against'].astype(float)
     df['steals_per_game_against'] = df['steals_per_game_against'].astype(float)
     df['blocks_per_game_against'] = df['blocks_per_game_against'].astype(float)
     df['team_fouls_per_game_against'] = df['team_fouls_per_game_against'].astype(float)
     df['points_per_game_against'] = df['points_per_game_against'].astype(float)
     try:
-        df['offensive_efficiency'] = df['offensive_efficiency'].astype(float)
-        df['defensive_efficiency'] = df['defensive_efficiency'].astype(float)
-        df['Net_efficiency'] = df['Net_efficiency'].astype(float)
-    except:
-        print(f"Some team's_efficiency was not recorded")
+        df['offensive_efficiency'] = pd.to_numeric(df['offensive_efficiency'], errors='coerce')
+        df['defensive_efficiency'] = pd.to_numeric(df['defensive_efficiency'], errors='coerce')
+        df['Net_efficiency'] = pd.to_numeric(df['Net_efficiency'], errors='coerce')
+    except ValueError:
+        print("Some team's_efficiency was not recorded")
+
 
     #page from second url
-    page = requests.get(standings_url)
+    page = requests.get(standings_url, timeout=10)
    
-    if(page.status_code != 200):
+    if page.status_code != 200:
         print("USport's Server did not respond with HTTP request")
 
     #parse html document
     soup = BeautifulSoup(page.content, 'html.parser')
 
     #initialize list to stroe data
     team_names = []
@@ -336,15 +348,17 @@
 
     Args:
         arg (str): Gender of the teams. Should be either 'men' or 'women'.
 
     Returns:
         pd.DataFrame: DataFrame containing processed team statistics.
     """
-    if(arg.lower() == 'men'):
+    if arg.lower() == 'men':
         team = ('https://universitysport.prestosports.com/sports/mbkb/2023-24/teams?sort=&r=0&pos=off',
              'https://universitysport.prestosports.com/sports/mbkb/2023-24/standings-conf', 52)
-    elif(arg.lower() == 'women'):
+    elif arg.lower() == 'women' :
         team = ('https://universitysport.prestosports.com/sports/wbkb/2023-24/teams?sort=&r=0&pos=off',
                'https://universitysport.prestosports.com/sports/wbkb/2023-24/standings-conf', 48)
+    else:
+        raise ValueError("In correct argument . options are: \'men\' or \'women\'")
     team_stats_df = __usports_team_data(team[0], team[1], team[2])
-    return team_stats_df
+    return team_stats_df
```

