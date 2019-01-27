# NBA Performance & Salary
This is the final project for Joshua Koh, Edward Yang,
Edward Fujiwara, and Aaron Lim’s coding class. The objective of this project is to analyze data from the NBA, and seeing if players’ salaries and their performance correlate. For example, a player might have a higher salary if they perform well, and vice versa.
### Project Management
Our project was mostly managed on Trello. We assigned each member on certain tasks to do such as coding and research.

### CSV Files and Statistics

For our NBA statistics, we found CSV files about players’ salaries and their performance (FG, AST, STL, BLK, etc.) on GitHub. We downloaded these files and merged them on Pandas to make a file to see how the salaries affects performance.
Although, not every column was useful for us, so we deleted some of the columns that were no use for us. We also needed a column for the Joshua Score Index, our own score index we used to measure performance, so we added an extra column for the JSI.

### JSI (Joshua Score Index)
The JSI formula is a formula created to assess a player’s performance based on their number of turnovers, steals, blocks, assists, and field goals. The formula takes the average turnovers, steals, and blocks of a player and multiplies them by 1.2, and takes the average assists and multiplies them by 0.8. The reason why the assists are multiplied by 0.8, and not 1.2 is because we thought that assists weren’t as important and showed less of a performance than the other three. With the factor of all of these numbers multiplied, the formula multiplies this factor with the square root of the average field goal. The reason why the field goal is square rooted is to decrease the difference when comparing two or more players to make the comparison more accurate.

### Contributors
* Joshua Koh
* Edward Yang
* Edward Fujiwara
* Aaron Lim
