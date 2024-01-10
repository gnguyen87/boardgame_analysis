# What makes a board game difficult? (An EDA)
By Na Nguyen, James Hernandez, Jordy Marin Urbina, and Sylvain Zong-Naba

Date: November 11, 2022

Our group seeks to investigate data on Board games created from 1950-2016 with an emphasis on their complexity with which different variables (from game types and minimum age to number of categories and maximum players)  may correlate. 

When applicable, we also try to track the changes through each decade by faceting our graphs to give a better visualization.

# Investigating Boardgame Complexity

## Playing Time

![image](https://github.com/gnguyen87/boardgame_analysis/assets/134335069/c7e50250-f423-4421-b459-e7dcd4b013fd)


Figure 1 shows the relationship between average complexicty of a game and its playing time. From the visualization of the scatter plot, there is a strong association between playing time and average complextity at first (between 15-to around 100 minutes) and then the association starts to lower as the playing time increases. Games that have a playing time between the range of 15-200 minutes have a complexity in the range of 1-5. Most of the games that are in that interval have a complexity concentrated between 1-3. Most games with a playing time of more than 200 minutes have a complexity level concentrated in the level of 2-4.5. Overall, one could stay that although there seems to be a certain relationship bewteen playing time and complexity level of a game,it seems the strength of the relationship is weak. Both games with a lower playing time and high playing time have more or less similar complexity thus, playing time does not seem to be associated with the complexity level of a game.

## Number of Categories

![image](https://github.com/gnguyen87/boardgame_analysis/assets/134335069/e92dfda9-fd3d-47bf-9c36-e566b7d3d6da)


From the observed data, we can see that the highest complexity rating concentrates in games that have 9-12 categories. The average complexity score from the collected sample steadily increases as board games have more categories. However, once they have surpassed the 9-12 categories/per game, the average complexity rating drops significantly, with a median of around 2.2 average complexity score of boardgames with 13-14 categories and below 2 average complexity score of those with 21-24 categories. Board games with 25-28 categories have a median of 2.5 average complexity rating.

## Base Games vs. Expansion Packs

Considering that expansion packs were quite literally adding new material (i.e. rules, lore, strategies, etc.), we wondered whether expansion packs were viewed as more complicated than base games, we decided to create multi-density plots as they would show the frequency of players that rated the game in a specific way for both base games and expansion packs. We filtered out all ratings of 0, as the lowest possible rating was 1. If we had kept that occurrence (0) in the data frame, the graph would imply that many players did not find these games to be complex at all when they really just did not provide a rating. We also noticed that expansion packs became prevalent in the 1970's; we decided to keep previous data to allow for a temporal analysis of before and after. 

![image](https://github.com/gnguyen87/boardgame_analysis/assets/134335069/b4768de4-04df-4cb1-94d6-fa8cf92824a3)

We saw that, in general, expansion packs were viewed as more complicated by players. In the 1950s and 1960's, board games were very skewed to the right (though much more extreme in the former), implying that they were viewed as simple and easy to play. In the 1970's and forward, ratings began to vary more, but still were viewed as less complicated than that of expansion packs regardless of the decade. The largest subset of players seem to rate base games at a complexity between 1 and 2, implying these games are not very challenging. On the contrary, the largest subset of expansion pack players provided a rating that peaked at roughly 2 and 3. However, while all the density plots for original board games were largely right skewed, expansion packs were still skewed to the right, but only slightly (i.e. 1970's and 1990's); there is a much more even distribution. It is interesting to see though how prior to the rise of  expansion packs, board games were considered much simpler. It would be interesting to see what factors caused this, and what factors maybe influence expansion packs being more complex. 

## Number of Categories ~ Game Type


When examining original board games (excluding their expansion versions), we can observe that in the most 2 recent decades, these original board games started to have more categories within a game. Furthermore, the median average complexity score for an original board game with more categories (around 2-3 for games with 9-12 and 13-16 categories), starting from the 1990s, is higher than those with less categories (around 1.8-1.9 for those with less than 9 categories). There is not much data on original games with more than 21 categories, however.

![image](https://github.com/gnguyen87/boardgame_analysis/assets/134335069/8c308705-5295-4587-a22a-09c114c62b4d)

The group sought to look at how the complexity of expanded games compares to the amount of categories through a temporal lens. Figure 4.2 shows a reinforcement that expanded games only really came to prevalence in the 1970's. These expansion packs were mostly between 1-8 categories, with the occurrence of 9-12 categories growing in the 2000's. In general, it seems as if the graph shows a decline in perceptions of complexity for these games over time in expansion packs with either 1-4 or 5-8 categories, with greater median complexity alternating throughout the different decades. However, those expansion packs with 9-12 categories clearly had a greater median and average perceived complexity, although this was more clear in the 2000's than the 2010's (median 3.5 complexity in the 2000’s, but median 3 in the 2010’s). 

## Card & Maximun Players

Throughout our data-wrangling process, we only considered games with 25 maximum players or fewer since the higher concentration was in the low numbers of players. From figure 6 we can observe the distribution of the average complexity scores of the games faceted by subgroups of the maximum number of players. From the scores, 1 is the lowest level of average complexity score and 5 is the highest. Within the group of 1-5 maximum number of players, there is a relatively uniform distribution of the average complexity between 1 and 4, having its highest peak at approximately 2. Correspondingly, within the group of 6-10 maximum players, the distribution is right-skewed, having the highest concentration around the lower average complexity scores and with two peaks close to 1 and 2. Additionally, the category of 11-15 maximum players has the highest concentration of around 1-3 average complexity and its peak is between 1-2. However, we can see that there is also some concentration around 3 to 5 average complexity. Lastly, the last two groups of 16-20 and 21-25 maximum players have a similar distribution, having the highest concentration and a peak between 1 to 2. Also, these groups have another concentration around 2.5 to 4 and both peaking at 3. Overall, there seems to be a tendency across all the groups for the maximum number of players and low level of complexity scores.

![image](https://github.com/gnguyen87/boardgame_analysis/assets/134335069/bc337011-31c0-4756-87ce-eda82910db90)

# Conclusion

For Figure 1, The game playing times does not seem to be associated with their complexity level. Some further research that could be done would be to look at the relationship between the complexity level of games and User rating as it would be interesting to see if there is a trend between how a game complexity is and how many users rates it. 

For Figure 2, it is observable that the number of categories, to an extent, does correlate with a higher median average complexity score. However, the median for average complexity score seems to decrease once a board game has more than 12 categories.

For Figure 3, regardless of the decade, original board games were not perceived to be very complicated at all, they were very right skewed. On the other hand, there were no expansion packs until the 1970’s. For the following decades after, there was a more complex perception of the games. Still, while they were more complex, there was slightly more even distributions.      

For Figure 4, drawing from both visualizations 4.1 and 4.2, we can see that although the number of categories does correlate with a higher median average complexity score after the 1990s, the median average complexity score of expansion packs are relatively higher than that of original base games.

From figure 5.1, we can see that Science Fiction games were rated as the most complex across decades from 1980 to 2010 in proportion to Card Games. By looking closely at Figure 5.2 we found that Science Fiction games seem to be rated as more complex (between the 4 and 5 scores).

For Figure 6, we observed that across all five intervals for maximum players, there seems to be a high concentration of the games being rated as 1 and 3 on the score level.

All in all, there are a lot of variables that can fluctuate a board game's average complexity score. However, there are some that do not significantly correlate with how difficult a game can be. Our project aimed to look at what may or may not influence these results. Yet, there are myriad ways to investigate this topic further that are beyond the scope of the given data. 


