# Uber-Supply-Demand-Gap-Analysis
EDA of Uber ride data to analyze supply–demand gaps and unfulfilled trips.


**Project Overview :-**
    This project conducts an in-depth Exploratory Data Analysis (EDA) on Uber's ride request data to identify and analyze the critical supply-demand gaps, particularly for trips connecting the City and the Airport. The core challenge is the significant imbalance between rider demand and driver availability, which results in a high volume of unfulfilled requests.


**Objective:** To pinpoint the exact time slots and pickup locations where service failures are most severe and to determine the underlying causes—whether structural (lack of cars) or behavioral (driver cancellations)—to provide data-driven solutions for operational efficiency and revenue optimization.


**Key Findings: The 58% Service Failure**
    The analysis of 6,745 ride requests revealed a low overall trip completion rate of only 42%, with 58% of requests resulting in a service failure (Cancelled or No Cars Available). The service failures are concentrated in two distinct temporal and spatial gaps:

| Time Slot | Pickup Point | Primary Issue | Root Cause | Failure Rate |
| --- | --- | --- | --- | --- |
| **Evening Rush** (5 PM – 10 PM) | **Airport** | **No Cars Available** | Massive shortage of driver supply at the airport to meet high arrival demand. | ~66.5% |
| **Early Morning** (5 AM – 10 AM) | **City** | **Driver Cancellations** | Drivers avoid airport trips from the city, likely due to the fear of a lack of return fares. | High |


**Actionable Recommendations :-**

Based on the root causes identified, the following targeted interventions are recommended to bridge the supply-demand gap:

**1. Addressing the Evening Airport Gap (No Cars Available)**

- **Dynamic Incentives:** Implement targeted surge pricing and financial incentives to encourage drivers to move towards the Airport during peak arrival hours (5 PM - 10 PM).

- **Designated Staging:** Create a dedicated, incentivized waiting area for drivers at the Airport to ensure a consistent supply pool.

**2. Addressing the Morning City Gap (Driver Cancellations)**

- **Cancellation Penalties:** Introduce stricter penalties for drivers who cancel during the peak morning hours (5 AM - 10 AM) for airport-bound trips.

- **Return Trip Guarantee:** Offer a guaranteed minimum fare or a preferential match for a return trip from the Airport back to the City to reduce driver hesitancy.


**Methodology and Tools :-**

The analysis followed a structured Exploratory Data Analysis (EDA) approach, including:

**1. Data Wrangling:** Standardizing mixed timestamp formats and performing feature engineering to create key variables such as Request Hour, Request Day, Time Slot and a binary Gap Status.

**2. Exploratory Analysis (UBM Rule):** Conducting Univariate, Bivariate and Multivariate analysis to understand the distribution of requests, the relationship between pickup points and status and the hourly demand vs. supply curves.

**3. Visualization:** Utilizing Python libraries to create clear visualizations that highlight the temporal and spatial nature of the supply-demand imbalance.


**Tools Used:**

- **Python:** Pandas, NumPy, Matplotlib
- **Jupyter Notebook:** For data processing and visualization logic.
- **Excel:** For initial data cleaning and creating an interactive dashboard for stakeholders.


**Conclusion :-**
    The analysis highlights that Uber’s operational challenges are primarily due to predictable supply shortages rather than random demand. By leveraging these insights, Uber can significantly increase trip completion rates, revenue and customer satisfaction.
