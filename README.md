# swot-analysis-dataset
Data set used to develop http://www.swot.cricpredictor.com; a SWOT Analysis system of Cricket Players.

Data set prepared for Online Analytics System for SWOT Analysis of Cricket Players, hosted at http://swot.cricpredictor.com/

## About Data set
Data set contains 5 CSV files separated by "|"
keywords.csv, players.csv, odi_balls.csv, t20_balls.csv, cluster_data_bat.csv

## keywords.csv
It contains all the keywords

1. id <int> unique identifier for the keyword
2. title <string> title of the keyword
3. type <string> what type of keyword is it? balls type, batting shot, batting shots how, ball line, ball length, fielding region

## players.csv
It contains brief but important information about each player

1. id <int> unique identifier for the player
2. fullname <string> full name of the player
3. Nation_team <string> Which country the player represents?
4. Bating <string> Player bats left handed or right handed?
5. Bowling <string> what is the bowling style of the player

## odi_balls.csv
It contains all the balls information for ODI, a total of 399,034 records.

1. id <int> unique identifier for each ball
2. odi_no <int> unique identifier for each ODI
3. host <string> country where the match was played
4. innings <int> whether it is innings 1 or 2
5. batting_team <string> name of batting country
6. ball <float> ball number along with the over, such as 0.1,0.2, 49.5 and so on
7. batsman <int> id of the batsman 
8. bowler <int> id of the bowler
9. bowling_team <string> name of the bowling country
10. bat_runs <int> number of runs scored by batsman off that ball
11. extra_runs <int> number of runs scored as extra of that ball
12. total_runs <int> total number of runs scored off that ball
13. wicket <int> whether it was wicket ball or not. -1 means no wicket and 1 means wicket
14. balls_type <int> keyword id of the ball type, that bowler delivered. -1 means information was not available.
15. batting_shot <int> keyword id of what shot batsman played. -1 means information was not available.
16. batting_shots_how <int> keyword id of how batsman played shot. -1 means information was not available.
17. ball_line <int> keyword id of what line was bowled by bowler. -1 means information was not available.
18. ball_length <int> keyword id of what length was bowled by bowler. -1 means information was not available.
19. fielding_region <int> keyword id of what fielding region that ball went. -1 means information was not available.

## t20_balls.csv
It contains all the balls information for T-20, a total of 84,507 records.
All attributes are same as of odi_balls.csv except:

1. t20_no <int> unique identifier for each T-20

## cluster_data_bat.csv
It contains swot values for selected attributes of the filtered batsmen.

1. 	bat_id <int> batsman id
2.	Attack_swot <float> swot of the shot, ranging from -1 to +1.
3.	Defend_swot <float> swot of the shot, ranging from -1 to +1.
4.	Leave_swot <float> swot of the shot, ranging from -1 to +1.
5.	Gentle Shot_swot <float> swot of the shot, ranging from -1 to +1.
6.	Back Foot_swot <float> swot of the shot, ranging from -1 to +1.
7.	Front Foot_swot <float> swot of the shot, ranging from -1 to +1.
8.	Wide Off Stump_swot <float> swot of the ball line, ranging from -1 to +1.
9.	Outside Off Stump_swot <float> swot of the ball line, ranging from -1 to +1.
10.	Stumps_swot <float> swot of the ball line, ranging from -1 to +1.
11.	Down Leg Stump_swot <float> swot of the ball line, ranging from -1 to +1.
12.	Wide Down Leg Stump_swot <float> swot of the ball line, ranging from -1 to +1.
13.	Yorker_swot <float> swot of the ball length, ranging from -1 to +1.
14.	Full Toss_swot <float> swot of the ball length, ranging from -1 to +1.
15.	Full Length_swot <float> swot of the ball length, ranging from -1 to +1.
16.	Good Length_swot <float> swot of the ball length, ranging from -1 to +1.
17.	Short of Length_swot <float> swot of the ball length, ranging from -1 to +1.
18.	Over Pitched_swot <float> swot of the ball length, ranging from -1 to +1.
19.	Fine Leg Region_swot <float> swot of the fielding region, ranging from -1 to +1.
20.	Square Leg Region_swot <float> swot of the fielding region, ranging from -1 to +1.
21.	Wis-Wicket Region_swot <float> swot of the fielding region, ranging from -1 to +1.
22.	Long On Region_swot <float> swot of the fielding region, ranging from -1 to +1.
23.	Long Off Region_swot <float> swot of the fielding region, ranging from -1 to +1.
24.	Cover Region_swot <float> swot of the fielding region, ranging from -1 to +1.
25.	Point Region_swot <float> swot of the fielding region, ranging from -1 to +1.
26.	Third-man Region_swot <float> swot of the fielding region, ranging from -1 to +1.
