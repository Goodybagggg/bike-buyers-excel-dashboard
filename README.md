# Bike Buyers Analysis: Excel Dashboard

An Excel project that explores what kind of customers buy a bike, using pivot tables, charts and a one-page dashboard.

## Project Overview
The dataset describes 1,000 customers (marital status, gender, income, children, education, occupation, home ownership, cars, commute distance, region, age) and whether each one purchased a bike. I cleaned the data, grouped customers into age brackets, and used pivot tables and charts to see which characteristics go with buying a bike.

## Objectives
- Prepare the raw data for analysis (checks, age brackets).
- Compare bike purchases across age, income, commute distance and other customer traits.
- Present the results on a single, readable dashboard.

## Tools Used
Microsoft Excel: formulas (`IF`), pivot tables, pivot charts, dashboard layout.

## Methodology
1. **Inspect** the 1,000-row `bike_buyers` sheet (no missing values and no duplicate IDs found).
2. **Prepare** a `Working Sheet` copy and add an **Age Brackets** column with a nested `IF`:
   - Over 54 = Old, 31 to 54 = Middle Age, under 31 = Adolescent
3. **Analyse** with pivot tables in the `Pivot Table` sheet:
   - Average income by gender and purchase status
   - Purchases by commute distance
   - Purchases by age bracket
   - Purchases by individual age
4. **Visualise** with three charts, assembled in the `Dashboard` sheet: *Average Income Per Purchase*, *Customer Commute*, *Customer Age Brackets*.

## Key Findings
> Calculated from the full 1,000-row dataset.

- **48.1%** of customers bought a bike (481 of 1,000).
- **Age:** Middle Age customers (31 to 54) were the most likely to buy, at about **55%**, compared with about 36% for under-31s and 31% for over-54s.
- **Commute distance:** Customers commuting **2 to 5 miles** bought most often (about 59%). Those commuting **10+ miles** bought least (about 30%).
- **Region:** Pacific (about 59%) was ahead of Europe (about 49%) and North America (about 43%).
- **Income:** Buyers had a slightly higher average income (about 57,963) than non-buyers (about 54,875).
- **Gender:** Purchase rates were very similar (female about 49%, male about 47%).
- **Marital status:** Single customers bought more often (about 54%) than married customers (about 43%).

## Recommendations
- Focus marketing on customers aged roughly 31 to 54 and on shorter commutes (up to 5 miles).
- Look at what is working in the Pacific region and test it in North America.
- Treat income and gender as weak signals, since the differences are small.

## Limitations
- The pivot tables saved in the workbook show only 18 customers (they appear to be filtered), so the figures above were recalculated from all 1,000 rows. Refresh or clear the filters in the pivots if you want them to match.
- The figures show association, not cause.

## Repository Structure
```
bike-buyers-excel-dashboard/
├── README.md
├── data/Bike_Buyers_Excel_Project.xlsx   # raw data, working sheet, pivots, dashboard
└── screenshots/                          # dashboard images
```

## Dashboard Preview
![Dashboard](screenshots/dashboard.png)

## Author
**Olumide Goodness**
