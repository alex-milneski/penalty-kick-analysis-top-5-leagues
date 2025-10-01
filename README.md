# Penalty kick analysis in the top 5 European football leagues 

*Note: Commonly know as 'penalties', FBref refers to these shots as Penalty Kicks (PKs) - so will I.*

### Data Source
[FBref's API - Team Season Statistics](https://fbrapi.com/documentation#team-season-stats) - FBref's data that I scraped was originally collected by Opta Sports.

---

### Exploring the Data ⚽
The goal of this project is to look at penalty kicks from the top 5 leagues (English Premier League, Serie A, Bundesliga, La Liga, Ligue 1) over the last 5 years and compare the conversion ratio of these shots against the determined probability of one of these shots being successful.

xG (Expected Goals) is a metric that has become increasingly popular in ⚽ to calculate the probability of a team scoring from a single shot. The probability is determined by several factors including where the shot was taken from (distance and angle from goal), how the shot was taken (stronger foot, weaker foot, head, bouncing ball, etc.), and other factors [xG Explained](https://fbref.com/en/expected-goals-model-explained/).

Penalty kicks are a unique type of shot, since they are always taken from the same spot and under similar conditions. Opta has determined the probability of a penalty kick scoring a goal at 0.79 or **pxG (Penalty xG) = 0.79**.

### Research Questions
**Is pxG being underestimated/overestimated in some instances?**
Are there teams or leagues that massively overperform/underperform at penalty kicks?

---

### Results

In total, from the 2020-2021 season to the 2024-2025 season, there have been 2312 PK goals from 2910 PK attempts **resulting in a 0.79 conversion rate**. However, looking at leagues individually shows us that from the 'Big 5' leagues, the French Ligue 1 and the English Premier League overperform xpG with 83% and 82% conversion rates respectively while the Spanish La Liga underperforms xpG with a 76% conversion rate.
 
![alt text](https://github.com/alex-milneski/penalty-kick-analysis-top-5-leagues/blob/main/la_liga.png)

<br>

La Liga has a lot of underperforming teams well below a 0.79 conversion rate, 5 of the worst performing teams are from the Spanish league, and them that has the most attempts in La Liga has a conversion rate of 0.7. 
Interestingly, from the 'Big 5' league, Espanyol is the team with the most PKs without any missed attempts (15/15). This is contrasted by Real Madrid, 5th in terms of total PKs but the worst performing team out of the top 12 teams with the most PK attempts (at least 40 PKs).

Both Lyon and Paris St. Germain, 2 teams from the French Ligue 1, have also taken some of the most PKs but have been overperforming the xpG - 1st and 3rd respectively from all teams who have taken at least 40 PKs in a top 5 league. This could also help explain how that league has been overperforming the 0.79 xpG.    

 Note: when looking at conversion rates in the context of a league, or for 'best/worst performers' a filter was applied to remove teams that had 5 attempts or less.

 <br>


| team |            pk attempts  |pk made | conversion rate |                 league    |                                                                     
| ------------- |-------------:| -----:| -------------:| ---------------:|             
|Lyon             |         41  |     37        |     0.90      |    French Ligue 1
|Roma              |        47   |    40         |    0.85       |  Italian Serie A
|Paris S            |       44    |   37          |   0.84        |  French Ligue 1
|Inter              |      48      | 40     |        0.83   |      Italian Serie A
|Valencia             |    41    |   34       |      0.83     |    Spanish La Liga
|Manchester City      |   42   |    33         |    0.79   | English Premier League
|Villarreal            |    40   |    31      |       0.78   |      Spanish La Liga
|Monaco               |  44     |  34       |      0.77     |     French Ligue 1
|Napoli                | 47      | 35        |     0.74      |   Italian Serie A
|Fiorentina             |   40    |   29        |     0.72       |  Italian Serie A
|Milan                  |   49     |  35      |       0.71    |     Italian Serie A
|**Real Madrid**           |   **46**    |  **32**    |        **0.70**   |      **Spanish La Liga**
