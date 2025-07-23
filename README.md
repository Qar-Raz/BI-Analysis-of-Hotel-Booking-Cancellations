# Business Intelligence Analysis: Hotel Booking Cancellations

### Final Dashboard
<table>
  <tr>
    <td><img src="./Dashboard%20Img%201.png" alt="Dashboard View 1"></td>
    <td><img src="./Dashboard%20Img%202.png" alt="Dashboard View 2"></td>
    <td><img src="./Dashboard%20Img%203.png" alt="Dashboard View 3"></td>
  </tr>
</table>

## Project Overview

This project presents an end-to-end Business Intelligence analysis of a hotel booking dataset to uncover the primary drivers of cancellations. The goal is to translate raw data into actionable insights that can help a hotel optimize its booking policies, reduce revenue loss, and improve operational efficiency. The analysis utilizes the **Design Thinking framework** to ensure the final solution is targeted, relevant, and addresses real-world business problems.

The project encompasses a full data lifecycle, from initial data cleaning and exploratory analysis in Python to the creation of a dynamic, multi-faceted dashboard in Power BI.

**Dataset:** [Hotel Booking Demand on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

---

## Methodology: The Design Thinking Framework

This project was structured using the five stages of the Design Thinking framework to ensure a user-centric and problem-focused approach:

1.  **Empathize:** The process began by gathering qualitative insights through an interview with a hotel marketing professional to understand the real-world context of booking cancellations.
2.  **Define:** Based on initial research, the core problem was defined around identifying not just the number of cancellations, but the policies, timing, and customer types involved.
3.  **Ideate:** This stage involved brainstorming key business questions and analytical paths to investigate high-value cancellations, seasonality, and segment risk.
4.  **Prototype:** An interactive, multi-page dashboard was designed and built in Power BI to serve as the prototype.
5.  **Test:** The final dashboard allows for interactive exploration, enabling users to filter data, test hypotheses, and derive their own insights.

---

## Repository Files

This repository contains the core components of the analysis:

*   `Hotel_Booking_Analysis.ipynb`: A **Jupyter Notebook** containing all the Python code for the project.
    *   **Data Wrangling & EDA:** Includes cleaning, feature engineering, and univariate/bivariate analysis using Pandas and Matplotlib.
    *   **Statistical Testing & Outlier Detection:** Performed ANOVA, Chi-squared, and IQR methods to validate findings.

    ### EDA Visualizations
    <table>
      <tr>
        <td><img src="./Eda%20Img%201.png" alt="EDA Chart 1"></td>
        <td><img src="./Eda%20Img%202.png" alt="EDA Chart 2"></td>
        <td><img src="./Eda%20Img%203.png" alt="EDA Chart 3"></td>
      </tr>
    </table>

*   `Hotel_Cancellations_Dashboard.pbix`: The final **Power BI** file containing the interactive dashboard.

*   `Background_Research.xlsx`: An **Excel** file documenting the initial background knowledge gathered during the "Empathize" phase.

---

## Key Insights from the Analysis

*   **Deposit Policy:** "No Deposit" bookings showed a lower cancellation rate than deposit-based bookings.
*   **Customer History:** Customers with prior cancellations were more likely to cancel again.
*   **Market Segments:** "Online TA" bookings had the highest cancellation rate.
*   **Revenue Impact:** Room type "A" and stays of "4-7 nights" contributed the most to lost revenue.
*   **Agent Performance:** A single agent ID was responsible for a disproportionately high number of cancellations.

---

## Tools and Libraries Used

*   **Programming Language:** Python 3.x
*   **Python Libraries:** Pandas, Matplotlib
*   **Business Intelligence Tool:** Microsoft Power BI
