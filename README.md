Hariharan Thiyagarajan

CS725 - Spring 2018


**INTRODUCTION**

The topic I chose for visualization is to show the overview of teams performance and the supporting factor in **Indian Premier League(IPL)** cricket. I selected this topic because, cricket is like religion in India. 
By starting IPL, cricket fever has reached the pinnacle as IPL has introduced style and entertainment at the grounds, fans hear loud music, 
see fireworks everytime batsman hits a boundary or when bowler takes a wicket. Added to that, the name of every team is based on a state. This makes the citizen of that place 
to encourage and support them. Being an ardent of cricket, I wanted to find interesting factors about the teams performance and how it supports in winning a match. At the end,
I decided to check number of wins by each team over the years which further urge me to check teamwise winning record against all the other teams. Since winning is not only about 
the performance of players in a team there is an another underlying and important factor which is toss. I also decided to check if the toss is impacting the outcome of the match.

<br>

**DATA**


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

<br>


**VISUALIZATION**

For visualization, I used three charts. Two bar chart and one scatterplot. First bar chart shows the number of wins by each and every team from highest to lowest number of wins over
the years in the history of IPL. Since I used bar chart for this, the exact number will not be known by looking at the chart alone. By **hovering** every single rectangle bar, we will
get to know the number of wins by each team. Second bar chart shows the teamwise record. Since there are 12 different teams, I decided to make it **interactive** by placing a **dropdown**
**selector** where the dropdown will have 12 teams from which we can select any team of our choice to know the stats. Barchart will be updated everytime when different team is selected. For
example: if Chennai Super Kings is **selected**, bar chart will be display multiple bars which represents the number of wins by Chennai Super Kings(CSK) aganist every other team in IPL. 
Hovering the each bar will give exact number of wins against that particular team. Even the teams in the dropdown selector are palced from highest to lowest number of wins.The third and final scatterplot shows the supporting factor for the previous two charts. If we look at the first and second 
bar chart, Mumbai Indians(MI) looks like a most dominating team over the years. I plotted matches and tosses won in the scatterplot. Each **dot** in the scatterplot has **different colors**
and hovering them will provide team name, number of tosses and mathces won by them. I also placed a **color legend** to know the teams name. Once after this, I found that there is a strong 
positive correlation between the toss and match outcome. When the number of tosses won by each team increases, number of mathces won by them also increases. It is clearly evident
from the scatterplot that toss plays a crucial role in teams overall performance as well as the outcome of the match.