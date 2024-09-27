# Project Title:
**Basketball Game Data Analysis (2004-2020)**

---

## 1. Objective/Problem Statement:
**Objective:** This project aims to analyze basketball game data from 2004 to 2020, uncover patterns, identify high-scoring games, and understand key factors contributing to game outcomes.  
**Why it Matters:** By analyzing key metrics such as points scored and win rates, this analysis provides insights into game dynamics, team performance, and strategies that lead to success.

---

## 2. Dataset Description:
- **games.csv:** Contains information for each game from 2004 to December 2020, including the two competing teams, their points, game date, and win status.
- **teams.csv:** Contains information about the teams, including team IDs, cities, and nicknames.

---

## 3. Tools and Technologies:
- **Programming Language:** Python
- **Libraries:** Pandas (for data manipulation and analysis)
- **IDE:** Jupyter Notebook
- **Version Control:** GitHub (for tracking changes and collaboration)

---

## 4. Data Preprocessing:
- **Subset Games Data:** Key columns such as game date, home/away team IDs, points scored, and win status were selected to focus the analysis on the most relevant aspects.
- **Data Cleaning:**
  - Converted `GAME_DATE` to a datetime format for consistency.
  - Standardized the data types of other relevant columns such as `GAME_STATUS_TEXT` (converted to string) to ensure proper handling during the analysis.

---

## 5. Merging Datasets:
- **Merging Games and Teams Data:** Merged the `games` dataset with the `teams` dataset on team IDs to incorporate team-specific details (city and nickname) for both home and away teams. This adds contextual team information into the game data, enriching the analysis.
- **Renaming Columns:** After merging, columns were renamed to distinguish between home and away team details (e.g., `city_home`, `nickname_home` for the home team).

---

## 6. Exploratory Data Analysis (EDA):
- **Game Outcomes:** Focused on analyzing key game outcomes such as high-scoring games and determining how often the home team won.
- **High-Scoring Games:** Analyzed games where the home team scored over 150 points to identify patterns in high-scoring matches.
- **Home Wins:** Investigated the performance of home teams and how often they won based on different scoring conditions.

---

## 7. Feature Engineering:
- **points_total Feature:** Created a new feature that sums the points scored by both the home and away teams in each game. This new metric (`points_total`) provides additional insights into the overall scoring intensity of games.

---

## 8. Data Manipulation and Sorting:
- **Sorting by Total Points:** Sorted the games by the `points_total` column to identify both the highest and lowest-scoring games.
- **Subset Selection Using iloc:** Selected subsets of data, including the first four rows and five columns of the `games` DataFrame, for further examination.

---

## 9. Indexing and Filtering:
- **Changing Index:** Set the `game_date` column as the index of the `games` DataFrame to facilitate time-based filtering and analysis of games by date.
- **Filtering by Game Date and Points:** Filtered games based on specific conditions, such as selecting games where the home team scored more than 150 points and did not win.

---

## 10. Data Visualization and Sorting:
- **Visualizing High-Scoring Games:** Used sorting and filtering to visualize and analyze high-scoring games and identify key moments where unusual or interesting results occurred.
- **Sorting and Ranking:** Ranked games by total points using methods like `nlargest` to identify the top-scoring games.

---

## 11. Data Export and Backup:
- **Exporting Transformed Data:** After all transformations and manipulations, the dataset was exported as a new CSV file (`games_transformed.csv`) for future use and sharing with stakeholders.

---

## 12. Challenges and Solutions:
- **Challenge:** Managing large datasets, performing multiple merges, and ensuring data integrity throughout the process.
- **Solution:** Systematically verified merges, renamed columns for clarity, and used data type conversions to ensure consistency throughout the analysis.

---

## 13. Future Improvements:
- **Advanced Analysis:** Plan to incorporate machine learning models to predict game outcomes based on performance statistics and historical game data.
- **Visualization:** Create visualizations, such as trends over time, to highlight patterns in team performance and game outcomes.

---

## 14. Key Learnings:
- Developed skills in cleaning and merging datasets with complex relationships, including handling large sports data.
- Learned to engineer features (e.g., `points_total`) to enhance the analysis of game outcomes.
- Gained expertise in using Pandas for exploratory data analysis, sorting, and filtering, which helped in uncovering valuable insights into basketball game dynamics.

---
