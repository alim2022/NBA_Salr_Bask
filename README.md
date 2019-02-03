# NBA Performance & Salary
This is the final project for Joshua Koh, Edward Yang,
Edward Fujiwara, and Aaron Lim’s coding class. The objective of this project is to analyze data from the NBA, and seeing if players’ salaries and their performance correlate. For example, a player might have a higher salary if they perform well, and vice versa.
### Project Management
Our project was mostly managed on Trello. We assigned each member on certain tasks to do such as coding and research.

### CSV Files and Statistics

For our NBA statistics, we found CSV files about players’ salaries and their performance (FG, AST, STL, BLK, etc.) on GitHub. We downloaded these files and merged them on Pandas to make a file to see how the salaries affects performance.
Although, not every column was useful for us, so we deleted some of the columns that were no use for us. We also needed a column for the Joshua Score Index, our own score index we used to measure performance, so we added an extra column for the JSI.

### JSI (Joshua Score Index)
The JSI formula is a formula created to assess a player’s performance based on their number of turnovers, steals, blocks, assists, and field goals. The formula takes the average turnovers and multiplies it by 1.2, and adds the average number of steals and blocks to this product. Next, the average assists is multiplied by 0.8. The reason why the assists are multiplied by 0.8, and not 1.2 is because we thought that assists weren’t as important and showed less of a performance than the other three. With the total of all of these numbers, the formula multiplies this with the square root of the product of the average field goal percentage and 10. The reason why the average field goal percentage is square rooted after being multiplied by 10 is to decrease the ratio when comparing two or more players to make the comparison more accurate. The reason why we multiply the average field goal percentage by 10 before square rooting it is because since all of the percentages are less than 1, when it is square rooted the product becomes high. The multiplying by 10 allows the field goal percentage to be more equal.
When comparing different players’ JSI’s, the higher score equals a higher performance.


### Contributors
* Joshua Koh
* Edward Yang
* Edward Fujiwara
* Aaron Lim
