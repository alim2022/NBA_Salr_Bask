# NBA Performance & Salary
This is the final coding project for Joshua Koh, Edward Yang,
Edward Fujiwara, and Aaron Lim. The objective of this project is to analyze multiple data points from NBA players, and seeing if players’ salaries and their performance have any correlation(i.e. seeing if salaries are higher for 'better' players). Through this project we hoped to discover more of this in detail.

### Project Management

Our project was mostly managed on Trello, and a shared Google Doc which we used to discuss and write a rough draft of this page. We assigned each member to certain tasks, which were roughly divided into Coding, the Readme document, and working on the Joshua Score Index(JSI)(the New Score Index(NSI) was added later).

### CSV Files and Statistics

For our NBA statistics, we found CSV files about players’ salaries and their performance (FG, AST, STL, BLK, etc.) on GitHub. We downloaded these files and merged them on Pandas to make a file to see how the salaries affect a player's performance. The years we used for our data are 2015 to 2016, and we synthesized this to get a more rounded data score, opposed to only one game.
Not every column was useful for us, so we deleted them. The only data columns we used were the player, Field Goal Percentage, average assists, average steals, average blocks, average turnovers, and we added the JSI and NSI, our own score index we used to measure performance. This will be explained in detail next.

### JSI (Joshua Score Index)
The JSI formula is a formula created to assess a player’s performance based on their number of turnovers, steals, blocks, assists, and field goals. The formula takes the average turnovers and multiplies it by 1.2, and adds the average number of steals and blocks to this product. Next, the average assists is multiplied by 0.8. The reason why the assists are multiplied by 0.8, and not 1.2 is because we thought that assists weren’t as important and showed less of a performance than the other three. With the total of all of these numbers, the formula multiplies this with the square root of the product of the average field goal percentage and 10. The reason why the average field goal percentage is square rooted after being multiplied by 10 is to decrease the ratio when comparing two or more players to make the comparison more accurate. The reason why we multiply the average field goal percentage by 10 before square rooting it is because since all of the percentages are less than 1, when it is square rooted the product becomes high. The multiplying by 10 allows the field goal percentage to be more equal.
When comparing different players’ JSI’s, the higher score equals a higher performance.

### NSI (New Score Index)

Although the JSI was a good way to calculate the players' skill, there were still a few factors that were less than accurate, as some ratios were not calculated correctly and some factor were incorporated. Created by Edward Yang, Joshua Koh and Aaron Lim, the New Score Index was created to bring the best of the JSI and solve its shortcomings to create a simple but accurate index on which to rate the players. In the NSI, a total of 7 factors are used, which are the 2-point goal percentage, 3-point goal percentage, average turnovers, average personal fouls, assists, steals and blocks. To calculate the actual score index, we first added both the 2-point goal percentage with the 3-point goal percentage, then multiplied by 100 to scale the data. Then we subtracted the turnover value plus the average personal fouls, which was halved, as  fouls are more common and we chose to minimize its negative effect. Next to that, we calculated 0.65 times the average number of assists plus 0.8 times the sum of the average steals and blocks. All ratios were calculated on how important one was. For example, we did not think the number of assists were as important as the steals and blocks, and so we multiplied it by a smaller ratio. Here, as is in the JSI, higher score equals higher performance.

### Plotting
We decided to use a scatter plot to show our data's correlation. A scatter plot is used when you need to show a correlation between two items, but only when there is no specific time relation. We used we used the individual salary of the players and the overall JSI as the y-axis. We believe that the scatter plot is the most effective method to show our data.


### Contributors
* Joshua Koh
* Edward Yang
* Edward Fujiwara
* Aaron Lim
