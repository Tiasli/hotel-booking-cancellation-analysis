# Hotel Booking Cancellation Analysis

An exploratory data analysis (EDA) and statistical testing project investigating cancellation behaviors using real world reservation data from two hotels in Portugal (resort in Algarve and city hotel in Lisbon, 2015–2017).

📄 **[Read the Full Project Report (PDF)](./Hotel_Booking_Cancellation.pdf)**

---

## Overview

Hotel cancellations create operational challenges and direct revenue losses. This study analyzes over 100,000 reservation records to identify patterns behind customer churn, testing whether cancellations occur randomly or follow measurable behavioral and seasonal drivers.

Developed as a course project for *Statistics and Data Analysis* at Galatasaray University.

## Key Findings

- **Seasonality & Volume Correlation:** Monthly booking volume shows a strong positive correlation with cancellation rates ($r = 0.742$). One-way ANOVA followed by Tukey's test confirmed significant differences across months ($p < 0.001$), with summer peak periods experiencing higher cancellation ratios.
- **Family Status Feature Engineering:** Grouped bookings into family and non-family segments based on children/babies counts. Independent two-sample t-tests revealed that family bookings had a significantly lower cancellation rate ($t = -4.48$, $p < 0.0001$) despite paying higher Average Daily Rates (ADR), representing a low-risk, high-value customer profile.
- **Lead Time:** Longer lead times (days between reservation and check-in) consistently correlated with higher cancellation rates across both hotel types.
- **Special Requests & Parking:** The presence of special requests and required parking spaces strongly decreased cancellation likelihood, indicating higher commitment to the reservation.

## Methodology & Tools

- **Data Cleaning & Handling:** Handled missing values, removed extreme outliers (top 0.01% on ADR), and filtered synthetic features.
- **Statistical Tests:** One-way ANOVA, Tukey's HSD post-hoc test, Two-sample independent T-tests, Pearson correlation.
- **Tech Stack:** Python (`pandas`, `scipy`, `seaborn`, `matplotlib`).

## File Structure

- Formatted IEEE-style project paper covering statistical methodology, visualizations, and findings.
- Jupyter notebook containing the full data cleaning, testing pipeline, and plotting code.
