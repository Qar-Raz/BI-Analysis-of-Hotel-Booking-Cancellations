# BI Analysis: Hotel Booking Cancellations

## Project Overview

This project presents an end-to-end Business Intelligence analysis of a hotel booking dataset to uncover the primary drivers of cancellations. The goal is to translate raw data into actionable insights that can help a hotel optimize its booking policies, reduce revenue loss, and improve operational efficiency. The analysis utilizes the **Design Thinking framework** to ensure the final solution is targeted, relevant, and addresses real-world business problems.

The project encompasses a full data lifecycle, from initial data cleaning and exploratory analysis in Python to the creation of a dynamic, multi-faceted dashboard in Power BI.

**Dataset:** [Hotel Booking Demand on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

---

## Methodology: The Design Thinking Framework

This project was structured using the five stages of the Design Thinking framework to ensure a user-centric and problem-focused approach:

1.  **Empathize:** The process began by gathering qualitative insights through an interview with a hotel marketing professional to understand the real-world context of booking cancellations. This helped build an empathy map and frame the problem from an industry perspective.

2.  **Define:** Based on the initial research, the core problem was defined: "Cancellations are significantly affecting our revenue, and we need to check which hotel policies are affecting cancellations. It's not just the number of cancellations, but when they happen and who is cancelling."

3.  **Ideate:** This stage involved brainstorming key business questions and analytical paths. Queries were formulated to investigate high-value cancellations, the impact of lead time and seasonality, and the risk profiles of different market segments and distribution channels.

4.  **Prototype:** An interactive, multi-page dashboard was designed and built in Power BI to serve as the prototype. This dashboard was created to visualize the complex relationships between variables and tell a clear data story.

5.  **Test:** The final dashboard allows for interactive exploration, enabling users (e.g., hotel managers) to filter data, test hypotheses, and derive their own insights, effectively testing the solution's ability to answer critical business questions.

---

## Repository Files

This repository contains the core components of the analysis:

*   `Hotel_Booking_Analysis.ipynb`: A **Jupyter Notebook** containing all the Python code for the project. This includes:
    *   **Data Wrangling:** Loading the dataset, cleaning inconsistent data (e.g., "NULL" strings), standardizing data types, and handling missing values with appropriate imputation strategies (mode for country, 0 for agent/company IDs).
    *   **Feature Engineering:** Creating a unified `arrival_date` column from its constituent parts.
    *   **Exploratory Data Analysis (EDA):** Univariate and bivariate analysis to understand data distributions and initial relationships using libraries like Pandas and Matplotlib.
    *   **Statistical Testing:** Performing ANOVA and Chi-squared tests to validate correlations between variables (e.g., `lead_time` and `is_canceled`).
    *   **Outlier Analysis:** Using the IQR method to identify and understand outliers in `adr` and `lead_time`.

*   `Hotel_Cancellations_Dashboard.pbix`: The final **Power BI** file. This interactive dashboard visualizes the findings from the Python notebook and serves as the primary tool for data storytelling. It includes dedicated pages for analyzing:
    *   Time and Seasonality Impact
    *   High-Value Cancellations (by revenue and special requests)
    *   Deposit Type Effectiveness
    *   Market Segment Performance
    *   Advanced visualizations like a decomposition tree and a Sankey chart to illustrate complex cancellation flows.

*   `Background_Research.xlsx`: An **Excel** file documenting the initial background knowledge gathered during the "Empathize" phase, including notes from the industry interview and the initial empathy map draft.

---

## Key Insights from the Analysis

The analysis uncovered several key insights that challenge conventional wisdom:

*   **Deposit Policy:** Bookings with a "No Deposit" policy had a lower cancellation rate than those with "Non-Refund" or "Refundable" deposits, likely due to data imbalance but a critical finding nonetheless.
*   **Customer History:** Customers with a prior history of cancellations were more likely to cancel again.
*   **Market Segments:** Bookings from "Online TA" (Travel Agents) had the highest cancellation rate, while "Groups" had the lowest.
*   **Revenue Impact:** Room type "A" and stays of "4-7 nights" contributed the most to lost revenue from cancellations.
*   **Agent Performance:** A single agent ID (Agent 9) was associated with nearly half of all cancellations, warranting further investigation.

---

## Tools and Libraries Used

*   **Programming Language:**
    *   Python 3.x
*   **Python Libraries:**
    *   Pandas (for data manipulation and analysis)
    *   Matplotlib (for data visualization during EDA)
*   **Business Intelligence Tool:**
    *   Microsoft Power BI
