###  Task 2 — Exploratory Data Analysis on Restaurant Tips

> "I never thought a dataset about restaurant tips could tell such an interesting story. The patterns were genuinely surprising."


|  Dataset | Restaurant Tips Data (244 records) |
|  Kaggle | [Download Dataset](https://www.kaggle.com/datasets/jsphyg/tipping) |

#### What I Did

This task was about exploring the data — not cleaning it, just understanding it. The tips dataset records information about restaurant customers: how much they spent, how much they tipped, whether they smoked, what day they came in, and more. My job was to dig in and find patterns.

Started with the basics. Computed all the descriptive stats — mean, median, standard deviation, quartiles. The average tip was around $3, but the spread was wide.

Then I made six visualizations, each answering a different question:

 **VIZ 1 — Histograms with KDE:** How are bill amounts, tips, and party sizes distributed? (Spoiler: most people dine in groups of 2, and most tips cluster between $1–$4)

 **VIZ 2 — Correlation Heatmap:** Which numbers are related to each other? Total bill and tip had the strongest correlation (r = 0.68) — the bigger the bill, the bigger the tip, mostly.

 **VIZ 3 — Box Plots:** How do tips vary by day and gender? By time and smoking status? Box plots made the spread and outliers immediately visible.

 **VIZ 4 — Scatter Plot with Trend Line:** Plotted total bill vs tip with a red trend line. The upward slope confirmed the positive relationship clearly.

 **VIZ 5 — Group-By Bar Charts:** Averaged tips by day of the week and by smoker/gender combo. Sunday came out on top.

 **VIZ 6 — Violin Plot:** Created a `tip_pct` feature (tip as a % of total bill) and plotted it by day and meal time. Dinner on Sundays had the most interesting shape.

#### What I Found — 3 Key Insights

 **Insight 1:** There's a strong correlation (r = 0.68) between total bill and tip amount. The more people spend, the more they tip. This means upselling — drinks, desserts, appetizers — is the most reliable way for servers to increase their tip income.

 **Insight 2:** Sunday evenings generate the highest average tips. Weekend diners are in a more relaxed, generous mood. Restaurants should schedule their most experienced servers on Sunday dinner shifts.

 **Insight 3:** Non-smokers tip slightly more than smokers on average. It's a small difference, but consistent across the dataset.
