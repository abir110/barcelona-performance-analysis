<<<<<<< HEAD
# ⚽ FC Barcelona: La Liga Performance Analysis (2021/22 – 2025/26)

> Exploratory analysis of FC Barcelona's league performance across five seasons: results, home advantage, toughest opponents, finishing efficiency, second-half resilience, and how they compare with La Liga's other leading clubs.
=======
# FC Barcelona — La Liga Performance Analysis (2021–2025)

> End-to-end exploratory data analysis of FC Barcelona's La Liga performance across 5 seasons (1,810 matches), uncovering scoring trends, tactical efficiency, rival comparisons, and resilience patterns using Python.
>>>>>>> 8d02ab283ff3a71b407e3cc03ebab8422e5f68d3

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8%2B-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13%2B-4C72B0)
<<<<<<< HEAD

**Data:** 1,790 La Liga matches from Football-Data.co.uk, of which **179 involve Barcelona**. Four complete seasons plus 2025/26 up to 9 March 2026.

---

## 📌 Key findings

| # | Question | Answer |
|---|---|---|
| 1 | How consistent has Barcelona been? | **1st** in 2022/23 and 2024/25, **2nd** in 2021/22 and 2023/24, and **leading 2025/26** after 27 matches. Points per game rose from **1.92 → 2.48**. |
| 2 | How big is the home advantage? | **77.5%** win rate at home vs **62.2%** away (2.40 vs 2.08 points per game). Higher at home in four of five seasons. |
| 3 | Who is the toughest opponent? | **Real Madrid**: 4 wins, 5 losses in 9 league meetings (1.33 points per game). |
| 4 | How efficient is the attack? | 16.2 shots per game, **37.0%** on target, **37.5%** of shots on target converted. |
| 5 | Do they turn games around? | Improved their half-time result in **58** matches, lost ground in only **14**. Trailing at half-time 34 times, they still won 11. |
| 6 | How do they compare with rivals? | The **most goals per game** of the leading clubs (2.18), but Real Madrid edged them on points per game (**2.27 vs 2.24**). |

---

## 📊 Charts

**Season by season.** Points per game climbed after a weaker 2021/22.

![Season performance](fig1_season_performance.png)

**Home vs away.** Home win rate was higher in four of five seasons (level in 2024/25), and Barcelona have won every home league match of 2025/26 so far.

![Home vs away](fig2_home_away.png)

**Head-to-head.** Win rates against every opponent faced at least 3 times.

![Head to head](fig3_head_to_head.png)

**Shooting efficiency.** Shots, accuracy and conversion by season.

![Shot efficiency](fig4_shot_efficiency.png)

**Half-time resilience.** How half-time positions turned into full-time results.

![Half-time resilience](fig5_halftime_resilience.png)

**Rivals comparison.** Barcelona vs La Liga's other leading clubs.

![Rivals comparison](fig6_rivals_comparison.png)

---

## 🗂️ Repository structure

```
barcelona-performance-analysis/
├── barcelona_analysis.ipynb      # full analysis
├── SP1_21.csv                    # La Liga 2021/22
├── SP1_22.csv                    # La Liga 2022/23
├── SP1_23.csv                    # La Liga 2023/24
├── SP1_24.csv                    # La Liga 2024/25
├── SP1_25.csv                    # La Liga 2025/26 (to 9 March 2026)
├── fig1_season_performance.png … fig6_rivals_comparison.png
├── requirements.txt
└── README.md
```

File names follow the year each season **starts**: `SP1_21.csv` holds the 2021/22 season (first match 13 August 2021).

## ▶️ How to run

```bash
git clone https://github.com/abir110/barcelona-performance-analysis.git
cd barcelona-performance-analysis
pip install -r requirements.txt
jupyter lab barcelona_analysis.ipynb
```

## 🛠️ Tools

Python · pandas · NumPy · Matplotlib · Seaborn · Jupyter

## 📚 Data source

[Football-Data.co.uk, La Liga results and statistics (SP1)](https://www.football-data.co.uk/spainm.php). Free and publicly available. Includes results, half-time scores, shots, shots on target, corners, fouls, cards and betting odds.

## ⚠️ Notes and limitations

- League positions are computed from the match data (points, then goal difference). La Liga's official tie-breaker is head-to-head, but no season here was decided by a tie.
- 2025/26 is incomplete, so its figures will change as the season continues.
- "Comeback" counts any improvement from half-time to full-time (draw → win, loss → draw, loss → win).

---

**Author:** Abir Alam Srabon · MSc Data Science, Aston University · [LinkedIn](https://www.linkedin.com/in/abir-alam-srabon) · [GitHub](https://github.com/abir110) · [Portfolio](https://abir110.github.io)
=======
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)

---

## Project Overview

This project analyses **5 seasons of La Liga match data** (2020/21 – 2024/25) from Football-Data.co.uk, focusing on FC Barcelona's performance trends across 179 matches. The analysis covers attacking efficiency, home/away splits, head-to-head records, and benchmarking against La Liga's top rivals.

| Season | Matches in Dataset |
|---|---|
| 2020/21 | 380 |
| 2021/22 | 380 |
| 2022/23 | 380 |
| 2023/24 | 380 |
| 2024/25 | 270 (ongoing) |

---

## Key Questions Answered

1. How has Barcelona's win rate and points-per-game evolved across 5 seasons?
2. How does home performance compare to away performance?
3. Which opponents have been the toughest for Barcelona?
4. How efficient is Barcelona at converting shots into goals?
5. How often do Barcelona come back from half-time deficits vs collapse from leads?
6. How does Barcelona rank against La Liga's other top teams?

---

## Key Findings

- **Consistent contenders** — Barcelona averaged 2.0+ points per game across all 5 seasons
- **Home fortress** — Win rate at home consistently outperforms away, though away form remains strong
- **Shot quality over quantity** — Conversion rate and shot accuracy consistently rank among La Liga's best
- **Resilient** — More comebacks than collapses across 5 seasons, reflecting strong squad mentality
- **Top of La Liga** — Highest points per game and goals scored among La Liga's top 6 clubs

---

## Repository Structure

```
barcelona-performance-analysis/
│
├── barcelona_analysis.ipynb    # Main analysis notebook
├── README.md                   # This file
│
├── data/
│   ├── SP1_21.csv              # La Liga 2020/21
│   ├── SP1_22.csv              # La Liga 2021/22
│   ├── SP1_23.csv              # La Liga 2022/23
│   ├── SP1_24.csv              # La Liga 2023/24
│   └── SP1_25.csv              # La Liga 2024/25 (partial)
│
└── figures/                    # Auto-generated by notebook
    ├── fig1_season_performance.png
    ├── fig2_home_away.png
    ├── fig3_head_to_head.png
    ├── fig4_shot_efficiency.png
    ├── fig5_halftime_resilience.png
    └── fig6_rivals_comparison.png
```

---

## Getting Started

```bash
# Clone
git clone https://github.com/abir110/barcelona-performance-analysis.git
cd barcelona-performance-analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Run
jupyter notebook barcelona_analysis.ipynb
```

---

## Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, aggregation |
| `numpy` | Numerical calculations |
| `matplotlib` | All visualisations |
| `seaborn` | Statistical plots |

---

## Data Source

- **Football-Data.co.uk** — La Liga Results & Stats (SP1 files): https://www.football-data.co.uk/spainm.php
- Free, publicly available football statistics dataset
- Columns include: match result, goals, shots, corners, fouls, cards, and 70+ betting odds

---

## Author

**Abir Alam Srabon**  
MSc Data Science — Aston University, Birmingham  
[LinkedIn](https://linkedin.com/in/abir-alam-srabon) · [GitHub](https://github.com/abir110) · [Portfolio](https://abir110.github.io)

---

*Part of a data analytics portfolio showcasing real-world EDA, sports analytics, and Python data science skills.*
>>>>>>> 8d02ab283ff3a71b407e3cc03ebab8422e5f68d3
