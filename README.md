# final-programming-and-data-analysis-2024

> Final: Programming and Data Analysis 2024.

- Define functions or classes in `asgmt.py` given their names, templates, and docstrings.
- Use file name as a relative path rather than using an absolute path when you import data.
- Run `test-runner.py` to validate your functions or classes.
- Upload `asgmt.py` to [NTU COOL](https://cool.ntu.edu.tw).

## 01. Define a class `ManipulateArgs` which instantiates objects with three methods `sort_asc()`, `sort_desc()` and `reverse()`.

```python
class ManipulateArgs:
    """
    >>> manipulate_args = ManipulateArgs(3, 2, 7, 5, 11)
    >>> manipulate_args.sort_asc()
    [2, 3, 5, 7, 11]
    >>> manipulate_args.sort_desc()
    [11, 7, 5, 3, 2]
    >>> manipulate_args.reverse()
    [11, 5, 7, 2, 3]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a class `SequenceGenerator` which instantiates objects with two methods `get_evens()` and `get_odds()` that return a `list` with the first `n` evens or odds.

```python
class SequenceGenerator:
    """
    >>> sequence_generator = SequenceGenerator(5)
    >>> sequence_generator.get_evens()
    [0, 2, 4, 6, 8]
    >>> sequence_generator.get_odds()
    [1, 3, 5, 7, 9]
    >>> sequence_generator = SequenceGenerator(7)
    >>> sequence_generator.get_evens()
    [0, 2, 4, 6, 8, 10, 12]
    >>> sequence_generator.get_odds()
    [1, 3, 5, 7, 9, 11, 13]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a function `get_primes()` which returns a `list` with the first `n` primes.

Source: <https://en.wikipedia.org/wiki/Prime_number>

```python
def get_primes(n: int) -> list:
    """
    >>> get_primes(3)
    [2, 3, 5]
    >>> get_primes(5)
    [2, 3, 5, 7, 11]
    >>> get_primes(7)
    [2, 3, 5, 7, 11, 13, 17]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a function `get_fibonacci()` which returns a `list` with the first `n` Fibonacci integers (given `n >= 2`).

Source: <https://en.wikipedia.org/wiki/Fibonacci_sequence>

```python
def get_fibonacci(n: int) -> list:
    """
    >>> get_fibonacci(3)
    [0, 1, 1]
    >>> get_fibonacci(5)
    [0, 1, 1, 2, 3]
    >>> get_fibonacci(7)
    [0, 1, 1, 2, 3, 5, 8]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```


## 05. Based on previous three questions, define a class `AdvancedSequenceGenerator` which instantiates objects with four methods `get_evens()`, `get_odds()`, `get_primes()`, and `get_fibonacci()` that return a `list` with the first `n` evens, odds, primes or integers of a Fibonacci sequence (given `n >= 2`).

- Source: <https://en.wikipedia.org/wiki/Prime_number>
- Source: <https://en.wikipedia.org/wiki/Fibonacci_sequence>

```python
class AdvancedSequenceGenerator:
    """
    >>> advanced_sequence_generator = AdvancedSequenceGenerator(5)
    >>> advanced_sequence_generator.get_evens()
    [0, 2, 4, 6, 8]
    >>> advanced_sequence_generator.get_odds()
    [1, 3, 5, 7, 9]
    >>> advanced_sequence_generator.get_primes()
    [2, 3, 5, 7, 11]
    >>> advanced_sequence_generator.get_fibonacci()
    [0, 1, 1, 2, 3]
    >>> advanced_sequence_generator = AdvancedSequenceGenerator(7)
    >>> advanced_sequence_generator.get_evens()
    [0, 2, 4, 6, 8, 10, 12]
    >>> advanced_sequence_generator.get_odds()
    [1, 3, 5, 7, 9, 11, 13]
    >>> advanced_sequence_generator.get_primes()
    [2, 3, 5, 7, 11, 13, 17]
    >>> advanced_sequence_generator.get_fibonacci()
    [0, 1, 1, 2, 3, 5, 8]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a class `KeyValueMethods` which instantiates objects takes `**kwargs` with 3 methods `reverse()`, `to_upper()`, and `to_lower()`.

```python
class KeyValueMethods:
    """
    >>> key_value_methods = KeyValueMethods(twn="Taiwan")
    >>> key_value_methods.reverse()
    {'Taiwan': 'twn'}
    >>> key_value_methods.to_upper()
    {'TWN': 'TAIWAN'}
    >>> key_value_methods.to_lower()
    {'twn': 'taiwan'}
    >>> key_value_methods = KeyValueMethods(twn="Taiwan", jpn="Japan")
    >>> key_value_methods.reverse()
    {'Taiwan': 'twn', 'Japan': 'jpn'}
    >>> key_value_methods.to_upper()
    {'TWN': 'TAIWAN', 'JPN': 'JAPAN'}
    >>> key_value_methods.to_lower()
    {'twn': 'taiwan', 'jpn': 'japan'}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a function `rotate_character()` which rotates a character with the 13th letter after it.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
def rotate_character(x: str) -> str:
    """
    >>> rotate_character("A")
    'N'
    >>> rotate_character("B")
    'O'
    >>> rotate_character("L")
    'Y'
    >>> rotate_character("M")
    'Z'
    >>> rotate_character("a")
    'n'
    >>> rotate_character("b")
    'o'
    >>> rotate_character("l")
    'y'
    >>> rotate_character("m")
    'z'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `rotate_sentence()` which rotates a sentence with ROT13.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
def rotate_sentence(x: str) -> str:
    """
    >>> rotate_sentence("Abj vf orggre guna arire.")
    'Now is better than never.'
    >>> rotate_sentence("Now is better than never.")
    'Abj vf orggre guna arire.'
    >>> rotate_sentence("Rkcyvpvg vf orggre guna vzcyvpvg.")
    'Explicit is better than implicit.'
    >>> rotate_sentence("Explicit is better than implicit.")
    'Rkcyvpvg vf orggre guna vzcyvpvg.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION 
```

## 09. Based on previous two questions, define a class `Rot13` which instantiates objects with 2 methods `rotate_character()` and `rotate_sentence()`.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
class Rot13:
    """
    >>> rot13 = Rot13()
    >>> rot13.rotate_character("A")
    'N'
    >>> rot13.rotate_character("B")
    'O'
    >>> rot13.rotate_character("L")
    'Y'
    >>> rot13.rotate_character("M")
    'Z'
    >>> rot13.rotate_character("a")
    'n'
    >>> rot13.rotate_character("b")
    'o'
    >>> rot13.rotate_character("l")
    'y'
    >>> rot13.rotate_character("m")
    'z'
    >>> rot13.rotate_sentence("Abj vf orggre guna arire.")
    'Now is better than never.'
    >>> rot13.rotate_sentence("Now is better than never.")
    'Abj vf orggre guna arire.'
    >>> rot13.rotate_sentence("Rkcyvpvg vf orggre guna vzcyvpvg.")
    'Explicit is better than implicit.'
    >>> rot13.rotate_sentence("Explicit is better than implicit.")
    'Rkcyvpvg vf orggre guna vzcyvpvg.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Given a plain text file `friends.txt` in working directory, define a class `Friends` with 2 methods `get_actor()` and `get_character()`.

```python
class Friends:
    """
    >>> friends = Friends()
    >>> friends.get_actor("Rachel Green")
    'Jennifer Aniston'
    >>> friends.get_actor("Monica Geller")
    'Courteney Cox'
    >>> friends.get_actor("Phoebe Buffay")
    'Lisa Kudrow'
    >>> friends.get_character("Jennifer Aniston")
    'Rachel Green'
    >>> friends.get_character("Courteney Cox")
    'Monica Geller'
    >>> friends.get_character("Lisa Kudrow")
    'Phoebe Buffay'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 11. Define a function `import_mlb_teams_json()` which imports `mlb_teams.json` in working directory.

```python
def import_mlb_teams_json() -> list:
    """
    >>> mlb_teams_json = import_mlb_teams_json()
    >>> type(mlb_teams_json)
    list
    >>> len(mlb_teams_json)
    30
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 12. Define a function `find_location_with_name()` which returns a MLB team's location name (`locationName`) given team's full name (`name`) based on `mlb_teams.json` in working directory.

```python
def find_location_with_name(name: str) -> str:
    """
    >>> find_location_with_name("New York Yankees")
    'Bronx'
    >>> find_location_with_name("New York Mets")
    'Flushing'
    >>> find_location_with_name("Los Angeles Dodgers")
    'Los Angeles'
    >>> find_location_with_name("Los Angeles Angels")
    'Anaheim'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 13. Define a function `find_names_with_franchise()` which returns MLB team names (`name`) given team's franchise name (`franchiseName`) based on `mlb_teams.json` in working directory. If there are multiple teams in the same franchise, return as a `tuple`, otherwise return as a `str`.

```python
def find_names_with_franchise(franchise: str):
    """
    >>> find_names_with_franchise("Los Angeles")
    ('Los Angeles Angels', 'Los Angeles Dodgers')
    >>> find_names_with_franchise("New York")
    ('New York Yankees', 'New York Mets')
    >>> find_names_with_franchise("Boston")
    'Boston Red Sox'
    >>> find_names_with_franchise("San Francisco")
    'San Francisco Giants'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 14. Define a function `import_imdb_files()` which imports 3 CSV files `movies.csv`, `movies_directors.csv`, and `directors.csv` in working directory.

```python
def import_imdb_files() -> tuple:
    """
    >>> movies, movies_directors, directors = import_imdb_files()
    >>> type(movies)
    pandas.core.frame.DataFrame
    >>> type(movies_directors)
    pandas.core.frame.DataFrame
    >>> type(directors)
    pandas.core.frame.DataFrame
    >>> movies.shape
    (250, 5)
    >>> movies_directors.shape
    (284, 4)
    >>> directors.shape
    (179, 3)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 15. Define a function `merge_dataframes()` which merges(or joins) 3 dataframes based on the following join-keys `movies.id`, `movies_directors.movie_id`, `movies_directors.director_id`, and `directors.id`. Select specified columns showing movie's title, director's name and their directing order given `movies.csv`, `movies_directors.csv`, and `directors.csv` in working directory.

```
                        title              director  ord
0    The Shawshank Redemption        Frank Darabont    1
1              The Green Mile        Frank Darabont    1
2               The Godfather  Francis Ford Coppola    1
3       The Godfather Part II  Francis Ford Coppola    1
4              Apocalypse Now  Francis Ford Coppola    1
..                        ...                   ...  ...
279             The 400 Blows     François Truffaut    1
280                  The Help           Tate Taylor    1
281                   Aladdin          Ron Clements    1
282                   Aladdin           John Musker    2
283                  Drishyam       Nishikant Kamat    1

[284 rows x 3 columns]
```

```python
def merge_dataframes() -> pd.core.frame.DataFrame:
    """
    >>> merged_dataframe = merge_dataframes()
    >>> type(merged_dataframe)
    pandas.core.frame.DataFrame
    >>> merged_dataframe.shape
    (284, 3)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 16. Define a function `find_movies_directed_by_nolan_spielberg()` which finds out movies directed by Christopher Nolan and Steven Spielberg. Select specified columns showing movie's title and director's name given `movies.csv`, `movies_directors.csv`, and `directors.csv` in working directory.

```
             director                               title
0   Christopher Nolan                     The Dark Knight
1   Christopher Nolan                           Inception
2   Christopher Nolan                         Oppenheimer
3   Christopher Nolan                        Interstellar
4   Christopher Nolan                        The Prestige
5   Christopher Nolan                             Memento
6   Christopher Nolan               The Dark Knight Rises
7   Christopher Nolan                       Batman Begins
8    Steven Spielberg                    Schindler's List
9    Steven Spielberg                 Saving Private Ryan
10   Steven Spielberg             Raiders of the Lost Ark
11   Steven Spielberg  Indiana Jones and the Last Crusade
12   Steven Spielberg                       Jurassic Park
13   Steven Spielberg                 Catch Me If You Can
14   Steven Spielberg                                Jaws
```

```python
def find_movies_directed_by_nolan_spielberg() -> pd.core.frame.DataFrame:
    """
    >>> movies_directed_by_nolan_spielberg = find_movies_directed_by_nolan_spielberg()
    >>> type(movies_directed_by_nolan_spielberg)
    pandas.core.frame.DataFrame
    >>> movies_directed_by_nolan_spielberg.shape
    (15, 2)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 17. Define a function `find_movies_with_multiple_directors()` which finds out movies directed by multiple directors. Select specified columns showing movie's title, director's name and their directing order given `movies.csv`, `movies_directors.csv`, and `directors.csv` in working directory.

```
                                  title               director  ord
0                               Aladdin           Ron Clements    1
1                               Aladdin            John Musker    2
2                     Avengers: Endgame          Anthony Russo    1
3                     Avengers: Endgame              Joe Russo    2
4                Avengers: Infinity War          Anthony Russo    1
5                Avengers: Infinity War              Joe Russo    2
..                                  ...                    ...  ...
55                     The Wizard of Oz          Norman Taurog    4
56                     The Wizard of Oz         Richard Thorpe    5
57                     The Wizard of Oz             King Vidor    6
58                                   Up            Pete Docter    1
59                                   Up           Bob Peterson    2

[60 rows x 3 columns]
```

```python
def find_movies_with_multiple_directors() -> pd.core.frame.DataFrame:
    """
    >>> movies_with_multiple_directors = find_movies_with_multiple_directors()
    >>> type(movies_with_multiple_directors)
    pandas.core.frame.DataFrame
    >>> movies_with_multiple_directors.shape
    (60, 3)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 18. Define a function `import_premier12_files()` which imports 2 CSV files `stats_batting.csv` and `stats_pitching.csv` in working directory.

```python
def import_premier12_files() -> tuple:
    """
    >>> stats_batting, stats_pitching = import_premier12_files()
    >>> type(stats_batting)
    pandas.core.frame.DataFrame
    >>> type(stats_pitching)
    pandas.core.frame.DataFrame
    >>> stats_batting.shape
    (164, 18)
    >>> stats_pitching.shape
    (166, 28)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 19. Define a function `find_batting_leaders()` which calculates batting average `AVG` for batters from `stats_batting.csv` in working directory and finds out the batting leaders whose `AVG` is above `.500`. The formula for finding `AVG` is dividing a player's hits(`H`) by his total at-bats(`AB`).

Source: <https://en.wikipedia.org/wiki/Batting_average_(baseball)>

$$
AVG = \frac{H}{AB}
$$

```
              Player Team       AVG   H  AB
0  CHEN, Chieh-Hsien  TPE  0.625000  15  24
1       HANSON, Alen  DOM  0.545455   6  11
2      PÉREZ, Hernán  VEN  0.533333   8  15
3     GAITAN, Alonso  MEX  0.526316  10  19
```

```python
def find_batting_leaders() -> pd.core.frame.DataFrame:
    """
    >>> batting_leaders = find_batting_leaders()
    >>> type(batting_leaders)
    pandas.core.frame.DataFrame
    >>> batting_leaders.shape
    (4, 5)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 20. Define a function `find_pitching_leaders()` which calculates earned run average `ERA` for pitchers from `stats_pitching.csv` in working directory and finds out the pitching leaders whose `ERA` is `0.00`. The formula for finding `ERA` is: 9 x earned runs(`ER`) / innings pitched(`IP`).

Source: <https://en.wikipedia.org/wiki/Earned_run_average>

$$
ERA = 9 \times \frac{ER}{IP}
$$

```
                Player Team  ERA    IP
0           HILL, Rich  USA  0.0  10.1
1            CHANG, Yi  TPE  0.0   8.0
2      FUJIHIRA, Shoma  JPN  0.0   6.0
3        CHEN, Kuan-Yu  TPE  0.0   5.2
4     KILOMÉ, Franklyn  DOM  0.0   5.0
5        HUANG, En-Sih  TPE  0.0   4.2
6   BALDONADO, Alberto  PAN  0.0   4.2
7       BENITEZ, Jorge  PUR  0.0   4.1
8          OTA, Taisei  JPN  0.0   4.0
9     SHIMIZU, Tatsuya  JPN  0.0   4.0
10       KIM, Seohyeon  KOR  0.0   4.0
11          GWAK, Been  KOR  0.0   4.0
12     PARK, Yeonghyun  KOR  0.0   3.2
13         CRUZ, Jesus  MEX  0.0   3.2
14      MIRANDA, Kevin  PAN  0.0   3.1
15    MENDEZ, Yohander  VEN  0.0   3.1
16     FUENTES, Steven  PAN  0.0   3.1
17        ALANIZ, R.J.  MEX  0.0   3.0
18        KENNEDY, Jon  AUS  0.0   3.0
19  RODRÍGUEZ, Ricardo  VEN  0.0   2.2
20     BURGOS, Enrique  PAN  0.0   2.1
21      REYES, Gerardo  MEX  0.0   2.1
22     MCGRATH, Daniel  AUS  0.0   2.0
23       WILKINS, Luke  AUS  0.0   2.0
24       SUZUKI, Shota  JPN  0.0   1.2
25    HUNTINGTON, Ryan  NED  0.0   1.2
26    RODRÍGUEZ, Joely  DOM  0.0   1.1
27  ESTANISTA, Jaydenn  NED  0.0   1.0
28       CINTRON, Luis  PUR  0.0   1.0
29       GOMEZ, Miguel  PAN  0.0   1.0
30    MARTINEZ, Raidel  CUB  0.0   1.0
31        SUZUKI, Sora  JPN  0.0   1.0
32        IBARRA, Jeff  MEX  0.0   0.2
```

```python
def find_pitching_leaders() -> pd.core.frame.DataFrame:
    """
    >>> pitching_leaders = find_pitching_leaders()
    >>> type(pitching_leaders)
    pandas.core.frame.DataFrame
    >>> pitching_leaders.shape
    (33, 4)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```