# Will a previous-year NBA All-Star player cause the team’s performance to improve in terms of win rate?

## Purpose
Importing a new player through trades, free agency, or the draft is a crucial aspect of building and maintaining a successful NBA team. Among these, the trade of an All-Star player will generally attract the most public attention. These All-Star players normally play pivotal roles in shifting the competitiveness of teams, impacting the strategies and dynamics of teams. Acquiring an All-Star player could have a profound influence on the franchise; for example, in 2018, LeBron James left the Cavaliers and signed with the Lakers. Ever since then, LeBron James has been the franchise player for the Lakers. Fans are excited about these trades, actively following the rumors during the offseason.

From the team’s perspective, acquiring an All-Star player can serve as an immediate force on the court for the team. A famous example was the 2017-2019 Warriors. After a dominant regular season record in 2016, the team lost to the Cavaliers in the final. To everyone’s surprise, the Warriors acquired Kevin Durant, an All-Star player who had almost beaten them in the Western Conference final. Later, the Warriors won two consecutive NBA championships in 2017 and 2018 and barely lost to the Toronto Raptors in 2019 due to player injuries.

However, All-Star players are not the only factor contributing to the success of a team. Sometimes, acquiring an All-Star player could potentially break a team's chemistry, worsening the team’s performance. Specifically, we are interested in the change in the team’s performance in terms of win rate and whether acquiring a previous-year All-Star player has a positive impact on the team in general.

## Model Choice
we decided to implement causal inference because it helps identify causality between acquiring a new All-Star player and the team’s win rate. Since we calculated the difference in the win rate for each team every season and knew if a team imported a previous-year All-Star player at the beginning of the season, this is an observational study. We decided to use outcome regression. 

## Preprocessing and producure
Completed information in report

## Result

The model’s coefficient for “treat”(~6%) is larger to the result in the simple difference(~1.5%) 
For every variable, we are 95% confident that the coefficient interval does not include 0, making the result significant. 
To test the impact of randomness in the model, we also tried to use bootstrap through a frequentist's perspective. 

Even though the simple difference indicates an insignificant improvement in terms of win rate(~1.5%), our model suggests an approximate 6% improvement in win rate. Both Bayesian and Frequentist’s perspectives agree with the result. However, the magnitude of this improvement is not too big, indicating there exists many other factors that impact the win rate of a team.  

