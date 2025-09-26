# Penalty kick analysis in the top 5 European football leagues 

*Note: Commonly know as 'penalties', FBref refers to these shots as Penalty Kicks - so will I.*

### Data Source
[FBref's API - Team Season Statistics](https://fbrapi.com/documentation#team-season-stats) - FBref's data that I scraped was originally collected by Opta Sports.

---

### Goals ⚽
The goal of this project is to look at penalty kicks from the top 5 European leagues of ⚽ (English Premier League, Bundesliga, Serie A, Ligue 1 and La Liga) over the last 5 years and compare the conversion ratio of these shots against the determined probability of one of these shots being successful.

xG (Expected Goals) is a metric that has become increasingly popular in ⚽ to calculate the probability of a team scoring from a single shot. The probability is determined by several factors including where the shot was taken from (distance and angle from goal), how the shot was taken (stronger foot, weaker foot, head, bouncing ball, etc.), and other factors [xG Explained](https://fbref.com/en/expected-goals-model-explained/).

Penalty kicks are a unique type of shot since they are always taken from the same spot and under similar conditions. Opta has determined the probability of a penalty kick scoring a goal at 0.79 or
**pxG (Penalty xG) = 0.79**.


---

**Is pxG being underestimated/overestimated in some instances?**
Are there teams or leagues that massively overperform/underperform at penalty kicks?
