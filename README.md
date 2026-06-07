# IPL Cricket Analysis Dashboard (2008–2024)

Interactive Power BI dashboard analyzing 17 seasons of IPL cricket — 1,095 matches and 2,60,920 ball-by-ball deliveries.

---

## Dashboard Preview

### Home — KPI Overview
![Dashboard Home](/dashboard.png)

### IPL Title Winners (2008–2024)
![Title Winners](/title_winners.png)

### Top 10 Run Scorers
![Top Batsmen](screenshots/top_10_batsmen.png)

### Toss Analysis
![Toss Analysis](screenshots/toss_analysis.png)

### Top 10 Bowlers — Wickets vs Economy
![Bowler Analysis](screenshots/bowler_analysis.png)

---

## Dataset

| File | Description |
|------|-------------|
| `matches.csv` | 1,095 matches — teams, venue, toss, result, season |
| `deliveries.csv` | 2,60,920 ball-by-ball records — batter, bowler, runs, wickets |

**Source:** [IPL Complete Dataset (2008–2024) on Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)

---

## Dashboard Pages

| Page | Description |
|------|-------------|
| Home | KPI cards — Total Matches, Venues, Seasons, Runs, Wickets, Sixes. Season & Team slicers. Navigation buttons. |
| IPL Title Winners | Bar chart of title wins by franchise (filtered to finals only) |
| Top Batsmen | Top 10 all-time run scorers with total runs |
| Toss Analysis | Does winning the toss help? Donut + stacked bar by toss decision |
| Top Bowlers | Scatter plot — Total Wickets vs Economy Rate for top bowlers |

---

## Key Findings

- **CSK and MI dominate** — 5 IPL titles each across 17 seasons
- **Toss advantage is minimal** — winning the toss results in a match win only 50.59% of the time
- **Fielding first works better** — teams that chose to field after winning the toss won significantly more matches than those who batted
- **Virat Kohli leads all-time runs** — 8,000+ runs, well ahead of Dhawan (6.8K) and Rohit (6.6K)
- **SP Narine has the best career economy** among top wicket-takers

---

## Tools & Techniques

- **Power BI Desktop** — report building, page navigation, slicers
- **Power Query** — data loading, bowler summary table via Group By
- **DAX** — calculated columns (`Toss_Match_Winner`), measures (`Total Sixes`)
- **Data Modelling** — matches ↔ deliveries relationship via match_id

---

## Files

| File | Description |
|------|-------------|
| `IPL_Dashboard.pbix` | Power BI report file |
| `matches.csv` | Match-level data |
| `deliveries.csv` | Ball-by-ball data |
| `screenshots/` | Dashboard page screenshots |
