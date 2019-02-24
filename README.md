# NBA Performance & Salary
This is the final coding project for Joshua Koh, Edward Yang,
Edward Fujiwara, and Aaron Lim. The objective of this project is to analyze multiple data points from NBA players, and seeing if players’ salaries and their performance have any correlation(i.e. seeing if salaries are higher for 'better' players). Through this project we hoped to discover more of this in detail.

### Project Management

Our project was mostly managed on Trello, and a shared Google Doc which we used to discuss and write a rough draft of this page. We assigned each member to certain tasks, which were roughly divided into Coding, the Readme document, and working on the Joshua Score Index(JSI), New Score Index (NSI), New Score Index 2.0 (NSI 2.0), and Player Score Index (PSI).

### CSV Files and Statistics

For our NBA statistics, we found CSV files about players’ salaries and their performance (FG, AST, STL, BLK, etc.), which were mostly available on GitHub. We downloaded these files and merged them on Pandas to make a file to see how the salaries affect a player's performance. The years we used for our data are 2015 to 2016, and we synthesized this to get a more rounded data score, opposed to only one game.
Not every column was useful for us, so we deleted them. The only data columns we used were the player, Field Goal Percentage, average assists, average steals, average blocks, average turnovers, and we added the JSI and NSI, our own score index we used to measure performance. This will be explained in detail next.

### JSI (Joshua Score Index)
The JSI formula is a formula created to assess a player’s performance based on their number of turnovers, steals, blocks, assists, and field goals. The formula takes the average turnovers and multiplies it by 1.2, and adds the average number of steals and blocks to this product. Next, the average assists is multiplied by 0.8. The reason why the assists are multiplied by 0.8, and not 1.2 is because we thought that assists weren’t as important and showed less of a performance than the other three. With the total of all of these numbers, the formula multiplies this with the square root of the product of the average field goal percentage and 10. The reason why the average field goal percentage is square rooted after being multiplied by 10 is to decrease the ratio when comparing two or more players to make the comparison more accurate. The reason why we multiply the average field goal percentage by 10 before square rooting it is because since all of the percentages are less than 1, when it is square rooted the product becomes high. The multiplying by 10 allows the field goal percentage to be more equal.
When comparing different players’ JSI’s, the higher score equals a higher performance.

### NSI (New Score Index)

Although the JSI was a good way to calculate the players' skill, there were still a few factors that were less than accurate, as some ratios were not calculated correctly and some factor were incorporated. Created by Edward Yang, Joshua Koh and Aaron Lim, the New Score Index was created to bring the best of the JSI and solve its shortcomings to create a simple but accurate index on which to rate the players. In the NSI, a total of 7 factors are used, which are the 2-point goal percentage, 3-point goal percentage, average turnovers, average personal fouls, assists, steals and blocks. To calculate the actual score index, we first added both the 2-point goal percentage with the 3-point goal percentage, then multiplied by 100 to scale the data. Then we subtracted the turnover value plus the average personal fouls, which was halved, as  fouls are more common and we chose to minimize its negative effect. Next to that, we calculated 0.65 times the average number of assists plus 0.8 times the sum of the average steals and blocks. All ratios were calculated on how important one was. For example, we did not think the number of assists were as important as the steals and blocks, and so we multiplied it by a smaller ratio. Here, as is in the JSI, higher score equals higher performance.

### Player Score Index(PSI)

After the New Score Index proved to be defective, and did not show the player correlations as accurately as even the JSI, we decided to make a final score index that would most closely match the NBA's official score ranking. This score index was intended to be simple, and also was to be the most accurate index. First, we evaluated the previous outcomes of the JSI and NSI, and tried to understand why we had not succeeded in making an accurate representation of the scores. The Player score index was first created with equalizing all aspects of a player's performance, including some such as points made and steals. However, when we had first done this and tried to make every point completely equal, it showed as if it were not accurate. This was shown very clearly in a specific case: Anthony Davis. As per the NBA's official ranking, Davis' overall performance score is not the highest, yet with our unedited PSI, Davis showed up as one of the best players. We knew that something must be changed, yet we did not know which. We started by looking at the specific parts of which Davis was good at. Davis was found out to be the best at blocks and rebounds, being many points ahead of any other player. This is how we found out that the blocks and both offensive and defensive rebounds of a player was being emphasized too much. After finding this out, we were able to adjust our scores into the final equation, which is PSI = 1.2* Points + 0.9 * Field Goal - 0.3*field goals attempted - Free throws missed + 0.4*ORB + 0.2*DRB + Steals + 0.6*assists + 0.2* Block - 0.4*fouls - 1.2*turn overs, where points are calculated by 3* (3 points made) + 2* (2 points made) + Free throws.


### Plotting
We decided to use a scatter plot to show our data's correlation. A scatter plot is used when you need to show a correlation between two items, but only when there is no specific time relation. We used we used the individual salary of the players and the overall JSI as the y-axis. We believe that the scatter plot is the most effective method to show our data.

### Conclusion

In conclusion, from our project, we were able to deduce that NBA players’ salaries do not necessarily correlate with their performance, though players with higher salaries did indeed do better generally. We created our own score index to measure player efficiency by compiling significant statistics. Then, we compared our PSI to the official Game Score Index (GS) used in the NBA and found out that we had twelve overlaps from the top fifteen players. This means that the first fifteen players in our PSI had twelve players that were also in the top fifteen of the official GS. This showed how accurate our player score index is. When comparing the top fifteen salaries of the 2015-2016 NBA season to our top fifteen players in the PSI, there were only five overlaps, which was relatively small. This means that there were “worse” players that had higher salaries, and vise versa("better" players with lower salaries). This lets us conclude that salary mostly does not affect players’ performance in the NBA. One explanation for this is that of the role a certain player has in their team. For example, Kobe Bryant had the highest salary in the 2015-2016 season, but wasn’t even ranked in the top 40. This is due to his importance to his team, the Los Angeles Lakers, who probably paid him a high salary for him to remain on that team, also becuase Kobe Bryant was a shooting guard and a small forward, and perhaps less likely to do other things a player with another position might.


### Contributors
* Joshua Koh
* Edward Yang
* Edward Fujiwara
* Aaron Lim
