# MathE Learning Intelligence

Analytics dashboard built from the MathE higher-education mathematics dataset (9,546 student answers, 372 students, 8 countries, 14 topics).

## Files

- `mathe_dashboard.html` — self-contained interactive dashboard. Open it directly in any browser (double-click, or drag into a browser window). No server or internet connection needed; all data is embedded in the file.
- `MathE_dataset__4_.csv` — original source data (uploaded).

## What's in the dashboard

- **Overview stats** — total answers, overall accuracy, student count, country count.
- **Accuracy by topic** — sorted by number of answers, so rare topics don't get overweighted.
- **Accuracy by country** — with sample size (`n`) shown alongside each bar.
- **Difficulty matrix** — basic vs. advanced accuracy per topic, with the gap between them flagged (green/amber/red).
- **Hardest / easiest questions** — ranked by empirical accuracy (minimum 5 attempts, to avoid noise from low-sample questions).
- **Student profile lookup** — type or pick a Student ID to see their overall accuracy, basic vs. advanced split, and strongest/weakest topics.

## Data notes

- Accuracy = share of answers marked correct (`Type of Answer` = 1).
- "Difficulty" here is empirical (observed accuracy), not assumed from the question's labeled level.
- The dataset contains individual answers, not full exam sessions — so this measures assessment performance, not long-term learning growth.

## Not yet built

From the original project brainstorm, these are still open if wanted:
- ML model predicting correct/incorrect + feature importance (logistic regression / random forest / XGBoost)
- Student clustering into learning-profile groups (generalists, basic-strong/advanced-weak, specialists, struggling)
- Geographic map view
