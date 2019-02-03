# NBA Performance & Salary
This is the final coding project for Joshua Koh, Edward Yang,
Edward Fujiwara, and Aaron Lim. The objective of this project is to analyze multiple data points from NBA players, and seeing if players’ salaries and their performance have any correlation(i.e. seeing if salaries are higher for 'better' players). Through this project we hoped to discover more of this in detail.

### Project Management

Our project was mostly managed on Trello, and a shared Google Doc which we used to discuss and write a rough draft of this page. We assigned each member to certain tasks, which were roughly divided into Coding, the Readme document, and working on the Joshua Score Index(JSI).

### CSV Files and Statistics

For our NBA statistics, we found CSV files about players’ salaries and their performance (FG, AST, STL, BLK, etc.) on GitHub. We downloaded these files and merged them on Pandas to make a file to see how the salaries affect a player's performance. The years we used for our data are #############, and we synthesized this to get a more rounded data score, opposed to only one season.
Not every column was useful for us, so we deleted them. The only data columns we used were the player, Field Goal Percentage, average assists, average steals, average blocks, average turnovers, and we added the JSI, our own score index we used to measure performance. This will be explained in detail next.

### JSI (Joshua Score Index)
The JSI formula is a formula created to assess a player’s performance based on their number of turnovers, steals, blocks, assists, and field goals. The formula takes the average turnovers and multiplies it by 1.2, and adds the average number of steals and blocks to this product. Next, the average assists is multiplied by 0.8. The reason why the assists are multiplied by 0.8, and not 1.2 is because we thought that assists weren’t as important and showed less of a performance than the other three. With the total of all of these numbers, the formula multiplies this with the square root of the product of the average field goal percentage and 10. The reason why the average field goal percentage is square rooted after being multiplied by 10 is to decrease the ratio when comparing two or more players to make the comparison more accurate. The reason why we multiply the average field goal percentage by 10 before square rooting it is because since all of the percentages are less than 1, when it is square rooted the product becomes high. The multiplying by 10 allows the field goal percentage to be more equal.
When comparing different players’ JSI’s, the higher score equals a higher performance.


### Contributors
* Joshua Koh
* Edward Yang
* Edward Fujiwara
* Aaron Lim
