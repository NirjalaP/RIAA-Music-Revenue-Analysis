# U.S. Recorded Music Revenue Analysis (1973–2024)

### Exploring the Economics Behind Music Revenue Recovery

An independent analysis of U.S. recorded music industry revenue using data from the Recording Industry Association of America (RIAA). This project explores 52 years of industry performance, the transition from physical to digital music, and the economic role of paid streaming subscriptions.

**[Explore the Interactive Tableau Dashboard](https://public.tableau.com/app/profile/nirjala.prajapati1612/viz/EconomicsBehindMusicRevenueRecovery/RIAADashboard)**

## Dashboard Preview

![RIAA Dashboard Overview](images/dashboard-overview.png)

![Subscription Analysis](images/subscription-analysis.png)

## Project Objectives

- Examine long-term changes in U.S. recorded music revenue from 1973 to 2024
- Compare nominal and inflation-adjusted revenue to distinguish reported growth from real growth
- Identify which music formats contributed to the industry's recovery
- Investigate paid subscription growth and revenue per reported subscription
- Explore potential challenges to future industry revenue growth

## Dataset Overview

The analysis uses **3,484 records covering 52 years (1973–2024)** from the RIAA's U.S. Recorded Music Revenue dataset.

| Attribute | Description |
|---|---|
| Data source | Recording Industry Association of America (RIAA) |
| Records | 3,484 |
| Time period | 1973–2024 |
| Data structure | Historical, annual, format-level industry data |
| Measures | Revenue, unit shipments, and subscription counts |
| Revenue types | Nominal and inflation-adjusted |
| Music formats | CDs, vinyl, downloads, streaming subscriptions, and other formats |
| Analysis tool | Tableau |

The dataset contains different types of measurements, making metric validation particularly important. Revenue values, physical units, and subscription counts cannot be aggregated interchangeably.

## Data Preparation and Validation

Before building the dashboard, I explored the dataset structure, reviewed metric definitions, and checked calculated totals against published industry figures.

### Key Validation Issue

My initial aggregation produced a 2024 revenue total approximately **$100 million higher** than the RIAA's published total.

After investigating the underlying records, I found that **Paid Subscription** represented revenue, while **Paid Subscriptions** represented the annual-average number of subscriptions.

Separating these metrics corrected the aggregation and reconciled the 2024 revenue total to approximately **$17.675 billion**.

This highlighted the importance of understanding metric definitions and measurement units before interpreting results.

### Analytical Preparation

- Distinguished revenue values from physical unit shipments and subscription counts
- Validated annual revenue totals against RIAA's published figures
- Used inflation-adjusted revenue for historical comparisons
- Compared revenue changes across formats and time periods
- Calculated annual subscriber growth and revenue per reported subscription
- Created Tableau calculated fields and interactive visualizations to investigate patterns

## Key Findings

### 1. The Industry Has Not Fully Recovered in Real Terms

U.S. recorded music revenue reached approximately **$17.7 billion in 2024**.

However, after accounting for inflation, revenue remained approximately **35.6% below its 1999 peak of $27.5 billion**.

This reveals a different picture from nominal revenue growth alone.

### 2. Paid Subscriptions Drove the Recovery

Inflation-adjusted recorded music revenue increased from approximately **$8.9 billion in 2014** to **$17.7 billion in 2024**, representing a net recovery of **$8.8 billion**.

During the same period, paid subscription revenue increased by approximately **$9.7 billion**.

Paid subscriptions therefore contributed more than the net industry recovery, offsetting declines in CDs, downloads, and other formats.

### 3. Subscriber Growth Is Maturing

Annual-average paid subscriptions increased substantially over the past decade, reaching approximately **100 million in 2024**.

However, year-over-year subscriber growth slowed to approximately **3.3% in 2024**, suggesting a more mature subscription market.

This raises an important question: how can the industry sustain revenue growth as subscriber acquisition slows?

### 4. Inflation Changes the Interpretation of Subscription Economics

A closer comparison of nominal and inflation-adjusted revenue per reported subscription revealed an important distinction:

| Metric | 2014 | 2024 |
|---|---:|---:|
| Nominal revenue per reported subscription | ~$100 | ~$107 |
| Inflation-adjusted revenue per reported subscription | ~$132 | ~$107 |

Nominal revenue per subscription increased slightly, while inflation-adjusted revenue per subscription declined.

This indicates that inflation was a major driver of the decline in real revenue per subscription over this period, rather than a decline in nominal revenue per subscription.

## Tableau Dashboard

The interactive Tableau dashboard explores:

- Historical nominal and inflation-adjusted revenue trends
- Changes in revenue contribution across music formats
- The growth of paid streaming subscriptions
- Subscriber growth and subscription revenue trends
- Industry recovery and long-term market dynamics

**[Open the Interactive Tableau Dashboard](https://public.tableau.com/app/profile/nirjala.prajapati1612/viz/EconomicsBehindMusicRevenueRecovery/RIAADashboard)**

The packaged Tableau workbook is also available in this repository: [RIAA-Analysis.twbx](RIAA-Analysis.twbx).

## Limitations and Future Research

The RIAA dataset provides valuable industry-level information, but it does not fully explain the underlying causes of changes in subscription economics.

Important factors not directly captured include:

- Individual, student, and family subscription plan mix
- Promotional pricing and bundled subscription offers
- Subscriber retention and churn
- Consumer willingness to pay
- Platform-level costs and profitability

Revenue per reported subscription is an aggregate industry measure, not necessarily revenue per individual customer.

Future research could combine industry data with consumer surveys and platform-level information to investigate pricing sensitivity, subscription preferences, and opportunities for sustainable growth.

## Skills Demonstrated

- **Data Validation:** Reconciled reported totals and identified inconsistent measurement units
- **Exploratory Data Analysis:** Investigated multi-decade trends and changes in revenue composition
- **Tableau:** Developed interactive visualizations, calculated fields, and analytical dashboards
- **Business Analysis:** Connected quantitative findings to broader industry questions
- **Analytical Communication:** Translated historical data into clear, evidence-based insights

## Data Source

**Recording Industry Association of America (RIAA)** — U.S. Recorded Music Revenue Data.

This is an independent portfolio project created for analytical research and visualization purposes.
