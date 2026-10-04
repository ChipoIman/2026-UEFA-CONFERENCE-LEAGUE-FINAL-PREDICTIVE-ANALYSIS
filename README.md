# 2026-UEFA-CONFERENCE-LEAGUE-FINAL-PREDICTIVE-ANALYSIS
This is a predictive analysis of Crystal Palace F.C's win probability against Rayo Vallecano in the 2026 Uefa conference league final  using 6 datasets from 3 leagues(The English Premier League, La Liga and the UEFA conference league), cleaned data  and built a combined simplified dataset using six CSV files, that was created a week before the Uefa Conference league final. 

**Objective**: 
Use team performance data to estimate Palace's win probability and help guide Oliver Glasner's tactical planning for the final.


Problem Overview: 
Problem: 
- What is the realistic probability of Crystal Palace to Win the UEFA Conference league final? 

Accurately prediction is important to  helping Oliver Glasner make the right tactical planning, squad rotation necessary to maximise palace's chances of winning the trophy.

Decision Maker:  Oliver Glasner(Coach) 

Why the problem matters: Crystal Palace are in there first ever European final , having won their first 2 trophies last season with the FA cup and the Community Shield, there looking to add another trophy and continue their upwards trajectory.

DATA
**Sources** 
Web-scraped through excel power query from:
- Soccerway
- Flashscore
- LiveSport
League Data Included:
- EPL 24/25 &25/26
- La Liga 24/25 &25/26
- UEFA Conference league 24/25 & 25/26
Most of the available data online that could be web-scraped without license is betting orientated, so cleaning was necessary to remove irrelevant fields and reduce noise.

Data Cleaning & Transformation
- Removed missing values
- standardized column names
- Simplified the data(to make it easier to understand)
- Combined all 6 csv files into one dataframe
- built team profiles using average goals scored and conceded.

MACHINE LEARNING
I tested four models against the data to determine what the match outcome probability would be for a crystal palace win.
Model                                   Test Accuracy 
Logistic Regression                      68.8%
Decision Tree                            59.9%
Random Forest                            59.1%
Gradient Boosting                        57.3%
The Logistic regression model performed the best and avoided over fitting, so It became the final model.

FINAL PREDICTION(Win Probability)
Crystal Palace:37.8%
Rayo Vallecano win/draw probability: 62.2%

Recommendations:
1. High press, high possession football to try to disrupt Rayo Vallecanos defense
2. Rest players for the Final and take advantage of the underdog tag in the final.
3. Since our data is mostly goal data, Palace must implement a better defensive strategy to keep Rayo Vallecano under control (quiet).

Measure of Success:
Win the trophy!

Project Limitations:
- only used two seasons of data for each of the leagues, ideally five seasons or more for each league would be better.
- did not include player or coaching metrics
- goal based data approach oversimplified real football dynamics
- Model accuracy limited by dataset depth.

Future Improvements
- add player stats, coaching profiles
- include high-pressure match history
- update data continuously
- Add team strength metrics( squad value, power index etc.)
- Try other ML techniques to build a self update model.
- Try Monte carlo simulation for predictive analysis

  Tools:
  Language - PYTHON
  Data Manipulation - PANDAS, NumPY
  Machine Learning - Scikit learn
  Data Visualization - Matplotlib, Seaborn
  Project Tracking - Weights & Bases (W & B)
  Web-Scraping - Excel Power Query
  Environment - Google Colab

Project Structure:
2026-UEFA-CONFERENCE-LEAGUE-FINAL-PREDICTIVE-ANALYSIS/
│
├── data/
│   ├── EPL-24-25.csv
│   ├── EPL-25-26.csv
│   ├── La-Liga-24-25.csv
│   ├── La-Liga-25-26.csv
│   ├── Conference-League-24-25.csv
│   ├── Conference-League-25-26.csv
│
├── notebooks/
│   └── Crystal_Palace_Prediction.ipynb
│
├── presentation/
│   ├── final Project.pptx
│
├── reports/
│   ├── Weights-and-Biases-results.pdf
│ 
└──README.md

How to run:
Download the Crystal_Palace_Prediction.ipynb file from the repo and open it in jupyter notebook, google colab or VS code, The notebook is already pre-trained, so you can run it as it is or tweak it as you see fit. 

Wandb.login information removed from jupyter notebook for security reasons. 
