# Chess Games Data Analysis (Lichess EDA)

An Exploratory Data Analysis (EDA) project investigating over 20,000 chess games played on Lichess. This project explores player ratings (ELO), opening popularity, and the different ways matches conclude to better understand chess trends.

## Project Overview
This project processes a Lichess dataset containing 20,058 games. The primary goal is to visualize the distribution of player skill levels and identify the most common outcomes of competitive matches.

### Key Features analyzed:
- **Player ELO Ratings:** Distribution of white vs. black player ratings.
- **Victory Status:** How games end (Resignation, Mate, Flagging, etc.).
- **Opening Trends:** Identification of the most popular openings (e.g., Van't Kruijs Opening).
- **Time Controls:** Frequency of different game formats (Rapid vs. Blitz).

## Libraries Used
The following Python libraries were used for data manipulation and visualization:
- **Pandas:** Data cleaning and aggregation.
- **NumPy:** Numerical operations.
- **Matplotlib:** Core plotting and figures.
- **Seaborn:** Statistical data visualization.

## Key Insights from the Analysis
- **ELO Distribution:** The majority of players fall within the 1200–1800 rating range, with the frequency decreasing as ratings approach master levels (2400+).
- **Game Outcomes:**
  - **Resignation:** The most common end to a match, accounting for **55.5%** of games (8,969 games).
  - **Checkmate:** Occurred in **31.9%** of games (5,146 games).
  - **Flagging (Out of Time):** Accounted for **8.4%** of outcomes (1,359 games).
  - **Draws:** The rarest outcome at **4.2%** (681 games).
- **Most Popular Opening:** The **Van't Kruijs Opening** was the most frequently played opening in the dataset.
- **Time Control:** **10+0 (Rapid)** was the most popular format with 6,817 plays.

## How to Run
1. Ensure you have the dataset `games.csv` in your directory.
   (download it from kaggle https://www.kaggle.com/datasets/datasnaek/chess
3. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   
