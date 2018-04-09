Hariharan Thiyagarajan

CS725 - Spring 2018


**Introduction**

The topic I chose for visualization is to show the overview of teams performance and the supporting factor in **Indian Premier League(IPL)** cricket. I selected this topic because, cricket is like religion in India. 
By starting IPL, cricket fever has reached the pinnacle as IPL has introduced style and entertainment at the grounds, fans hear loud music, 
see fireworks everytime batsman hits a boundary or when bowler takes a wicket. Added to that, the name of every team is based on a state. This makes the citizen of that place 
to encourage and support them. Being an ardent of cricket, I wanted to find interesting factors about the teams performance and how it supports in winning a match. At the end,
I decided to check number of wins by each team over the years which further urge me to check teamwise winning record against all the other teams. Since winning is not only about 
the performance of players in a team there is an another underlying and important factor which is toss. I also decided to check if the toss is impacting the outcome of the match.


**Data**


I got the data from **kaggle.com** where the **matches.csv** dataset contains the details of all the mathces that was played from 2008 to 2017. There were totally 636 rows of data
where each had the following details.

* Season number
* City where it was played
* Date of match
* Team1
* Team2
* Toss winner
* Toss decision
* DL applied
* Winner of the match
* Win by runs
* Win by wickets
* Player of the match
* Venue
* Umpires

Since I decided to visualize performance of the team and to find the relation between match outcome and toss outcome, I had to do some data transformations. I created a new excel 
**data.tsv** based on the matches.csv dataset where I created 4 columns: **Team**, **TW**(Tosses won), **MW**(Matches won based on toss), **Count**(Total number of wins irrespective of the toss).
After filtering the matches.csv, I got all the necessary data in data.tsv. I also created one more excel named **TeamwiseInformation.tsv** where I created fourteen colums. First two
colums were **roll** and **state**(representing each team), remaining 12 colums had 12 distinct team names. This dataset contains information about number of wins by each team against
all the other teams in IPL. Using TeamwiseInformation.tsv I will be able to visualize the teamwise record for all the teams. Using data.tsv, I will be able to visualize teams performance over the years 
and I can also find if there is a correlation between matches won and tosses won.

Link -  https://www.kaggle.com/manasgarg/ipl/data
