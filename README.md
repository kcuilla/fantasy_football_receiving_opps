# Fantasy Football Receiving Stats & Opportunities

Link:  https://rpubs.com/kcuilla/fantasy_receiving_opps_table

Interactive table displaying the top 100 WR & TE fantasy scorers in the NFL and their average opportunity and performance metrics per game as well as an option to drilldown and see that player's week by week stats by clicking on their row or dropdown arrow.

Note: This version is currently updated through week 7 of the NFL season, however, the code to make this update continuously throughout the season is included in the Rmd file.

The interactive table was made using the `reactable` package and the data is sourced from the `nflfastR` package.

## Explanation and Usage

In fantasy football, volume and opportunities are the most important factors a player needs in order to score points. A player who receives 50% of his team's targets per game is much more likely to score more fantasy points than a player who only receives 5% of his team's target share. 

This interactive tool can be used to help your fantasy football decision-making by shedding light on which WR & TE's in the NFL are receiving the most opportunities in the games they play and whether they are underperforming/overperforming based on their share of opportunities. 

For example, if you are having difficulty deciding which WR to start in a given week, you can look at each player's WOPR, which is their Weighted Opportunity Rating developed by Josh Hermsmeyer from FiveThirtyEight. WOPR is the weighted average of a player's team target share and team air yards share. If one of your players has an 'A' WOPR rating and the other has a 'D' WOPR rating, you should consider starting the player with the 'A' WOPR rating since that player has a larger target share and air yards share compared to the other player, and therefore, should have more opportunities to score more fantasy points.

Another way you could use this tool to your advantage is to look at which players are buy-low or sell-high candidates. For example, if a player has a 'D' WOPR rating but they are averaging more fantasy points per game relative to the Top 100, this player is over-performing where they should be based on their opportunities and it might be a good idea to sell-high on this player and trade for a player who has a higher share of opportunities.

### Column Definitions

- WOPR = Weighted Opportunity Rating. The weighted average of a player's team target share and team air yards share, created by Josh Hermsmeyer from FiveThirtyEight. If a player has an 'A' WOPR, this means they are in the upper 25% of the metric, while 'D' means they are in the lower 25%
- TGT SHARE = % of team's targets in games player played
- AIR SHARE = % of team's air yards in games player played
- AIR = the average number of yards thrown toward a receiver when he is targeted
- PTS = average fantasy points scored based on standard scoring rules (0 points per reception, 1 point per 10 yards receiving, 6 points per TD reception, -2 points per fumble lost; does not include points gained from rushing)
- AVG PTS vs TOP 100 = average fantasy points scored relative to top 100 average fantasy points scored

## Interactive Demo:
![](fantasyoppsinteractive.gif)
