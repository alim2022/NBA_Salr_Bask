# NBA Performance & Salary
This is the final coding project for Joshua Koh, Edward Yang,
Edward Fujiwara, and Aaron Lim. The objective of this project is to analyze multiple data points from NBA players, and seeing if players’ salaries and their performance have any correlation(i.e. seeing if salaries are higher for 'better' players). Through this project we hoped to discover more of this in detail.

### Project Management

Our project was mostly managed on Trello, and a shared Google Doc which we used to discuss and write a rough draft of this page. We assigned each member to certain tasks, which were roughly divided into Coding, the Readme document, and working on the Joshua Score Index(JSI).

### CSV Files and Statistics

For our NBA statistics, we found CSV files about players’ salaries and their performance (FG, AST, STL, BLK, etc.) on GitHub. We downloaded these files and merged them on Pandas to make a file to see how the salaries affect a player's performance. The years we used for our data are #############, and we synthesized this to get a more rounded data score, opposed to only one season.
Not every column was useful for us, so we deleted them. The only data columns we used were the player, Field Goal Percentage, average assists, average steals, average blocks, average turnovers, and we added the JSI, our own score index we used to measure performance. This will be explained in detail next.

### JSI (Joshua Score Index)
The JSI formula is a formula created to assess a player’s performance based on their number of turnovers, steals, blocks, assists, and field goals. The formula takes the average turnovers, steals, and blocks of a player and multiplies them by 1.2, and takes the average assists and multiplies them by 0.8. The reason why the assists are multiplied by 0.8, and not 1.2 is because we thought that assists weren’t as important and showed less of a performance than the other three. With the factor of all of these numbers multiplied, the formula multiplies this factor with the square root of the average field goal. The reason why the field goal is square rooted is to decrease the difference when comparing two or more players to make the comparison more accurate.

### Contributors
* Joshua Koh
* Edward Yang
* Edward Fujiwara
* Aaron Lim
