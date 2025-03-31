# Sprint 4 Project – Revenue Comparison of Megaline Prepaid Plans

As a data analyst for **Megaline**, a telecom operator, I was tasked with identifying which of their two prepaid mobile plans — **Surf** or **Ultimate** — brought in more revenue. The insights from this project were aimed at guiding their advertising budget decisions for future marketing campaigns.

### Surf vs. Ultimate: Which Plan Pays Off?

Using behavioral data from 500 customers in 2018, I explored their usage patterns across calls, messages, and internet consumption. The goal was to calculate monthly revenue per user and determine which plan was more profitable on average.

#### The Data

The analysis combined five separate CSV files:

- **`megaline_users.csv`** – user info and their subscribed plan
- **`megaline_calls.csv`** – call durations per user per day
- **`megaline_messages.csv`** – number of text messages sent
- **`megaline_internet.csv`** – amount of data consumed
- **`megaline_plans.csv`** – plan details including pricing and monthly limits

#### The Process

1. **Data Cleaning & Merging**  
   - Converted dates to datetime format, removed duplicates, and handled missing values.
   - Merged all datasets into a single user-level monthly dataset.

2. **Feature Engineering**  
   - Rounded call durations to the nearest minute, calculated total minutes, MBs, and messages per user per month.
   - Calculated monthly charges by simulating overage fees based on the Surf and Ultimate plan structures.

3. **Revenue Analysis**  
   - Computed average monthly revenue per user for each plan.
   - Conducted statistical tests (t-test) to check if revenue differences were statistically significant.

### Results & Takeaways

The analysis showed a **clear difference in average monthly revenue** between the Surf and Ultimate plans. One of the plans consistently outperformed the other in revenue generation, providing solid evidence for re-allocating advertising resources.

This project helped sharpen my ability to join multiple datasets, engineer realistic business metrics (like overage charges), and support decisions with data-driven insights.
