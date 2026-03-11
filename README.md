# Rider Cancellation Analysis

This project performs exploratory data analysis (EDA) on operational ride data to understand patterns and factors influencing rider cancellations. The analysis focuses on identifying behavioral and operational features that correlate with cancellation events.

## Dataset

- Total records: ~450,000 ride sessions
- Target variable: `cancelled`
  - 0 → Ride completed
  - 1 → Ride cancelled

The dataset contains operational ride information such as session time, reassignment status, and ride distance.

## Objective

Ride cancellations impact both platform efficiency and customer experience.  
The goal of this analysis is to:

- Explore cancellation patterns
- Identify operational factors related to cancellations
- Understand temporal trends in rider behavior

## Analysis Workflow

The project follows a structured EDA pipeline:

1. **Data Understanding**
   - Inspected dataset structure and variable types
   - Identified target variable distribution

2. **Class Imbalance Analysis**
   - Observed strong class imbalance  
   - ~52K cancelled rides vs majority non-cancelled rides

3. **Feature Analysis**

   Examined operational variables including:

   - Session time
   - Reassignment status
   - Acceptance delay  
     *(accept time – allotted time)*

4. **Feature Engineering**

   Created additional features:

   - **Total trip distance**  
     *(first mile distance + last mile distance)*

   - **Acceptance delay**

5. **Temporal Analysis**

   Investigated ride cancellation patterns across:

   - Hour of the day
   - Day of the week

6. **Visualization**

   Used statistical plots to explore trends and relationships.

## Key Insights

- Dataset exhibits **significant class imbalance**, indicating cancellations are relatively rare events.
- Operational features such as **session time and acceptance delay** show correlation with cancellation behavior.
- Temporal patterns suggest certain **hours of the day experience higher cancellation activity**.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Future Improvements

- Build predictive models for cancellation detection
- Apply feature importance analysis


