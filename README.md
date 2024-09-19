# Crowdfunding Campaign Success Analysis

## Project Overview

This project analyzes a dataset of 1,000 crowdfunding campaigns from platforms like Kickstarter and Indiegogo. By leveraging the power of Microsoft Excel for data manipulation, pivot tables, and visualizations, we explore trends related to the success and failure of crowdfunding campaigns. The aim is to uncover hidden insights that could help predict a campaign’s likelihood of success based on various factors such as the amount funded, the average donation, and campaign backers.

## Table of Contents

- Project Background

- Technologies Used

- Data Preparation and Analysis
  - Conditional Formatting
  - Calculated Fields
  - Pivot Tables and Charts
  - Crowdfunding Goal Analysis
  - Statistical Analysis
- Key Findings
- Conclusion
- Visualizations
- Repository Structure
- How to Run

## Project Background

Crowdfunding platforms have become an essential tool for creators to raise funds for projects. However, not all projects reach their goals. In this analysis, we work with data from 1,000 sample projects to investigate trends and factors contributing to success or failure. The goal is to identify patterns that may help predict campaign outcomes.

---

## Technologies Used

- **Microsoft Excel**
  - Conditional Formatting
  - Pivot Tables & Charts
  - COUNTIFS, AVERAGE, MEDIAN, MIN, MAX, VAR.P, STDEV.P functions
- **Microsoft Word** : For generating the final project report.

---

## Data Preparation and Analysis

### Conditional Formatting

- Applied conditional formatting to the **Outcome** column to visually differentiate between successful, failed, canceled, and live campaigns.
- In the **Percent Funded** column, a three-color scale was applied:
  - Red for 0% funding.
  - Green for 100% funding.
  - Blue for 200% funding and beyond.

### Calculated Fields

- **Percent Funded** : Calculated as the amount raised relative to the funding goal.
- **Average Donation** : Found by dividing the total amount raised by the number of backers.
- **Parent Category** and **Sub-Category** : Split the existing Category column into two separate columns.
- **Date Created Conversion** and **Date Ended Conversion** : Used formulas to convert Unix timestamps into Excel-readable date formats.

### Pivot Tables and Charts

- Created pivot tables to summarize campaign outcomes based on categories and sub-categories.
- Filtered stacked-column pivot charts by country to visualize the distribution of successful, failed, and canceled projects.
- Developed a pivot table that tracks campaign outcomes over time, filtered by parent category and year.
- Generated a line chart from this pivot table to show trends in campaign outcomes over time.

### Crowdfunding Goal Analysis

- Created a new table with columns for different funding goal ranges (e.g., Less than 1000, 1000 to 4999, etc.).
- Used **COUNTIFS** formulas to calculate the number of successful, failed, and canceled campaigns for each goal range.
- Calculated the total number of projects per range and the percentage of success, failure, or cancellation.
- Graphed the relationship between campaign goals and outcomes (success, failure, cancellation) using a line chart.

### Statistical Analysis

- Created a summary statistics table comparing successful and unsuccessful campaigns based on the number of backers.
- Calculated:
  - **Mean** number of backers.
  - **Median** number of backers.
  - **Minimum** and **Maximum** number of backers.
  - **Variance** and **Standard Deviation** .
- Determined which metrics (mean or median) better summarize the data and assessed the variability between successful and unsuccessful campaigns.

---

## Key Findings

1. **High-Goal Campaigns** : Campaigns with higher funding goals have a lower success rate, while campaigns with lower funding goals tend to succeed more often.
2. **Number of Backers** : The mean number of backers was higher for successful campaigns, but there is more variability in unsuccessful campaigns.
3. **Timing Trends** : Campaigns launched in earlier years had higher success rates compared to more recent campaigns, which tend to have more live or failed outcomes.

---

## Conclusion

This analysis revealed that while the number of backers is a key factor in campaign success, the funding goal plays a significant role in determining whether a campaign will succeed or fail. Additionally, certain categories of campaigns are more successful than others. The variability in backers across unsuccessful campaigns highlights the unpredictability of reaching campaign goals.
