# Cricket-torunament-simulation

This Python script simulates a cricket match between two teams, India and Pakistan. The simulation includes random player statistics and field conditions to determine the match outcome. The script uses classes to represent players, teams, the field, umpires, and commentators to manage the match simulation.

## How to Run

To execute the script, simply run the Python file "cricket_match_simulation.py". The script will generate random player statistics for both teams and simulate the match with 20 overs. The match simulation will display various match events, ball outcomes, and the final result of the match.

```bash
python cricket_match_simulation.py
```

Please note that the player statistics and field conditions are random, so the match outcomes may vary each time you run the script.

## Classes

### Player

Represents a player in a cricket team.

Attributes:

- `name` (str): The name of the player.
- `bowling` (float): The bowling skill of the player.
- `batting` (float): The batting skill of the player.
- `fielding` (float): The fielding skill of the player.
- `running` (float): The running skill of the player.
- `experience` (float): The experience level of the player.

### Team

Represents a cricket team.

Attributes:

- `name` (str): The name of the team.
- `players` (list): The list of Player objects representing the team's players.
- `captain` (Player): The Player object representing the team's captain.
- `batting_order` (list): The list of Player objects representing the batting order.
- `bowlers` (list): The list of Player objects representing the team's bowlers.

### Field

Represents the field conditions in a cricket match.

Attributes:

- `size` (str): The size of the field.
- `fan_ratio` (float): The fan ratio of the field.
- `pitch_conditions` (float): The pitch conditions of the field.
- `home_advantage` (float): The home advantage of the field.

### Umpire

Manages the match updates and predicts ball outcomes.

Attributes:

- `field` (Field): The Field object representing the field conditions.
- `scores` (int): The current score of the match.
- `wickets` (int): The number of wickets taken.
- `overs` (int): The number of overs bowled.

### Commentator

Generates descriptions of the match events and provides match information.

Attributes:

- `umpire` (Umpire): The Umpire object providing match information.

### Match

Represents a cricket match between two teams.

Attributes:

- `team1` (Team): The Team object representing the first team.
- `team2` (Team): The Team object representing the second team.
- `field` (Field): The Field object representing the field conditions.
- `total_overs` (int): The total number of overs in the match.

## Dependencies

This script does not have any external dependencies. It only requires Python 3.x to run.

## Note

The player statistics and field conditions are randomly generated, so the match outcomes may not reflect real-world scenarios. The script provides a basic simulation for cricket matches and can be further enhanced with more realistic player statistics, team strategies, and additional features for a more comprehensive cricket match simulation.
