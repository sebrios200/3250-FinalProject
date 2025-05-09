# Data Wrangling Project: Soccer Salary and Performance Analysis

This project analyzes the relationship between player salaries and performance in the English Premier League 2021–2022 season.

## Folder Structure

| Folder         | Description                        |
|----------------|------------------------------------|
| `raw data`     | Contains original/raw dataset files |
| `clean data`   | Cleaned or transformed datasets     |
| `Jupytor`      | Jupyter Notebooks for exploration and analysis |
| `docs`         | Documentation like data dictionaries |

## Table of Contents

- [`README.md`](./README.md): Project overview and instructions  
- [`raw data`](./data/raw): Raw dataset files  
- [`Jupytor/`](./notebooks): Jupyter notebooks used in the project  
- [`docs/DATA_DICTIONARY.md`](./docs/DATA_DICTIONARY.md): Dataset variable descriptions  
- [Official Premier League Table – 2021/22 Season](https://www.premierleague.com/tables?co=1&se=418&ha=-1)

## Data Source

The data in this project is partially derived from the official Premier League standings and team statistics:  
[https://www.premierleague.com/tables?co=1&se=418&ha=-1](https://www.premierleague.com/tables?co=1&se=418&ha=-1)

Additional data on individual player statistics and salaries was compiled from public sports databases and media sources.

## Key Questions

- Do higher-paid players perform better?
- Are certain positions overpaid or underpaid?
- How do total team wages relate to team performance (e.g., points or league position)?
- Are there players offering strong value for money?

## Data Dictionary

The data dictionary below describes all variables used in the dataset:


| Column            | Type    | Source          | Description                                                            |
|:------------------|:--------|:----------------|:-----------------------------------------------------------------------|
| Player            | Text    | PL21-22         | Name of the player.                                                    |
| Weekly Salary     | Float   | Testing         | Player's weekly salary (£).                                            |
| Annual Salary     | Float   | Testing         | Player's annual salary (£).                                            |
| Team              | Text    | PL21-22/PRTable | Club or team the player belongs to.                                    |
| Nation            | Text    | PL21-22         | Player's nationality.                                                  |
| Pos               | Text    | PL21-22         | Specific playing position (e.g., FW, MF).                              |
| Age               | Integer | PL21-22         | Player's age.                                                          |
| MP                | Integer | PL21-22         | Matches played.                                                        |
| Starts            | Integer | PL21-22         | Matches started (as part of starting lineup).                          |
| Min               | Integer | PL21-22         | Total minutes played.                                                  |
| 90s               | Float   | PL21-22         | Number of full 90-minute games played (Min ÷ 90).                      |
| Gls               | Integer | PL21-22         | Goals scored.                                                          |
| Ast               | Integer | PL21-22         | Assists made.                                                          |
| G-PK              | Integer | PL21-22         | Goals excluding penalties.                                             |
| PK                | Integer | PL21-22         | Penalty goals scored.                                                  |
| PKatt             | Integer | PL21-22         | Penalty attempts (both scored and missed).                             |
| CrdY              | Integer | PL21-22         | Yellow cards received.                                                 |
| CrdR              | Integer | PL21-22         | Red cards received.                                                    |
| Gls.1             | Float   | PL21-22         | Goals per 90 minutes.                                                  |
| Ast.1             | Float   | PL21-22         | Assists per 90 minutes.                                                |
| G+A               | Float   | PL21-22         | Combined goals and assists.                                            |
| G-PK.1            | Float   | PL21-22         | Non-penalty goals per 90 minutes.                                      |
| G+A-PK            | Float   | PL21-22         | Combined non-penalty goals and assists.                                |
| xG                | Float   | PL21-22         | Expected goals (xG) — model-estimated quality of chances.              |
| npxG              | Float   | PL21-22         | Expected goals excluding penalties (non-penalty xG).                   |
| xA                | Float   | PL21-22         | Expected assists (xA).                                                 |
| npxG+xA           | Float   | PL21-22         | Sum of non-penalty expected goals and expected assists.                |
| xG.1              | Float   | PL21-22         | Expected goals per 90 minutes.                                         |
| xA.1              | Float   | PL21-22         | Expected assists per 90 minutes.                                       |
| xG+xA             | Float   | PL21-22         | Sum of xG and xA per 90 minutes.                                       |
| npxG.1            | Float   | PL21-22         | Non-penalty expected goals per 90 minutes.                             |
| npxG+xA.1         | Float   | PL21-22         | Sum of non-penalty expected goals and expected assists per 90 minutes. |
| Played            | Integer | PRTable         | Number of matches the team played.                                     |
| Won               | Integer | PRTable         | Number of matches won by the team.                                     |
| Drawn             | Integer | PRTable         | Number of matches drawn by the team.                                   |
| Lost              | Integer | PRTable         | Number of matches lost by the team.                                    |
| Goals For         | Integer | PRTable         | Total goals scored by the team.                                        |
| Goals Against     | Integer | PRTable         | Total goals conceded by the team.                                      |
| Goal Difference   | Integer | PRTable         | Goal differential (Goals For - Goals Against).                         |
| Points            | Integer | PRTable         | Total points earned by the team.                                       |
| Performance Score | Float   | Custom Metric   | Custom overall player/team performance metric.                         |
| Goals_per_1k      | Float   | Custom Metric   | Goals scored per £1k earned.                                           |
| xG_per_1k         | Float   | Custom Metric   | Expected Goals per £1k earned.                                         |
| Assists_per_1k    | Float   | Custom Metric   | Assists made per £1k earned.                                           |
| G+A_per_1k        | Float   | Custom Metric   | Combined goals and assists per £1k earned.                             |