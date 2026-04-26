# Chess Games — Exploratory Data Analysis

An exploratory data analysis of over 16,000 chess games from [Lichess](https://lichess.org/), uncovering patterns in player ratings, openings, game outcomes, and time controls.

---

## Dataset

**Source:** [Chess Games Dataset (Lichess) — Kaggle](https://www.kaggle.com/datasets/datasnaek/chess)

**File:** `archive/games.csv`

The dataset contains metadata for real Lichess games, including player ratings, opening names, number of turns, time controls, victory conditions, and outcomes.

---

## Analysis Overview

### Data Cleaning & Inspection
- Loaded and inspected the dataset with `.info()` and `.isnull().sum()`
- Verified data types and checked for missing values

### Visualizations

| Chart | Description |
|---|---|
| ELO Distribution | Stacked histogram of white and black player ratings |
| Most Played Openings | Top 30 openings by frequency |
| ELO Distribution by Bracket | Player counts grouped in 200-point Elo bands |
| Opening Performance by Elo Group | Heatmap of win rates per opening across skill tiers |
| Rating Difference vs Win Probability | Sanity check: higher-rated players win more |
| Opening Depth vs Favourite's Win Rate | Do stronger players use deeper openings — and does it help? |
| Rated vs Unrated Games | Pie chart of game type breakdown |
| Top 10 Time Controls | Most commonly played time formats |
| How Matches End | Victory status breakdown (resign, checkmate, flag, draw) |
| Game Outcomes | White vs Black vs Draw proportions |
| Game Length Distribution | Histogram of number of turns per game |

---

## Key Findings

- **80.5%** of games were rated; **19.5%** were unrated
- Player ELO is concentrated in the **1450–1800** range
- Most games last between **40–60 turns**
- White wins **49.8%**, Black wins **45.7%**, Draws account for **4.5%**
- The most-played opening was the **Van't Kruijs Opening** (1.e3), likely due to its single-move simplicity
- The most common time control was **10+0** (Rapid — 6,817 games)
- **55.5%** of games ended by resignation, **31.9%** by checkmate, **8.4%** by flagging, and **4.2%** by draw

---

## Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, feature engineering |
| `numpy` | Numerical operations and binning |
| `matplotlib` | All visualizations |
| `seaborn` | Imported for styling |

---

## Getting Started

```bash
git clone https://github.com/arch-Seraph/ChessAnalysis.git
cd ChessAnalysis
pip install pandas numpy matplotlib seaborn
```

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/datasnaek/chess) and place `games.csv` inside an `archive/` folder, then open `pipeline.ipynb` in Jupyter.

---

## References

- [Matplotlib Documentation](https://matplotlib.org/stable/index.html)
- [NumPy Documentation](https://numpy.org/doc/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Chess Games Dataset — Lichess](https://www.kaggle.com/datasets/datasnaek/chess)
