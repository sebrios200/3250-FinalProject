# Data Dictionary

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