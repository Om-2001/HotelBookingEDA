# HotelBookingEDA

# Exploratory Data Analysis (EDA) on Hotel Bookings Dataset

## Summary of Steps Performed:

1. **Data Loading:**
   - Loaded the dataset from a CSV file using Pandas.

2. **Initial Exploration:**
   - Checked the first few rows of the dataset to understand its structure.
   - Explored column names, shape, and basic information about the dataset.
   - Checked for missing values in each column.

3. **Column Analysis:**
   - Explored unique values and characteristics of specific columns (e.g., 'hotel', 'is_canceled', 'country', 'meal', etc.).
   - Identified anomalies, outliers, and patterns in specific columns like 'adr', 'lead_time', and 'adults'.

4. **Data Wrangling:**
   - Dropped the 'agent' and 'company' columns due to limited information value and significant null data presence.
   - Eliminated rows with undefined values in 'distribution_channel' and 'market_segment'.
   - Removed rows with more than 3 required car parking spaces, lead time greater than 700, and guests equal to 0.
   - Replaced 'Undefined' values in the 'meal' column with 'BB'.
   - Filled null values in the 'country' column with 'PRT'.
   - Deleted outliers in the 'adr' column (values greater than 1000 and negative values).
   - Filled mean values in the 'adr' column where it was zero.
   - Changed data types to optimize memory usage (int16 and category).

5. **Exploratory Data Analysis (EDA):**
   - Conducted univariate analysis for various columns, including hotel types, arrival years and months, meals, countries, market segments, etc.
   - Explored numeric types and categorical types separately, visualizing trends and distributions.
   - Investigated lead time, average daily rate (ADR), and other numerical features.
   - Explored bivariate relationships between variables, such as hotel vs. market segment, hotel vs. customer type, lead time vs. ADR, etc.
   - Utilized multivariate analysis to examine relationships involving multiple variables, such as correlation matrices, ADR by hotel and customer type, and ADR by deposit type.

## Conclusions:

1. **Hotel Preference:**
   - City hotels are more preferred than resort hotels, constituting approximately 66.45% of the dataset.

2. **Temporal Trends:**
   - There is a rise in bookings in 2016, followed by a slight decrease in 2017.

3. **Meal Preferences:**
   - Breakfast (BB) is the most preferred meal type, contributing to 78% of the dataset.

4. **Country Insights:**
   - The top three countries contributing to hotel bookings are identified.

5. **Market Segments:**
   - The top five market segments are explored, providing insights into booking patterns.

6. **Customer Type Analysis:**
   - Transient customers are the most common, constituting approximately 97% of the dataset.

7. **Lead Time and ADR Analysis:**
   - The average lead time for bookings is approximately 104 days.

8. **Cancellation Patterns:**
   - Transient customers have the highest cancellation percentage, emphasizing the need for targeted strategies.

9. **Correlation Analysis:**
   - Correlation matrix highlights relationships between numeric features.

10. **ADR Patterns:**
    - ADR patterns are analyzed across different scenarios, providing insights into pricing strategies.
