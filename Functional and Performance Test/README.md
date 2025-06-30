# smartbridge-housing-project

## Model Performance Test

### 1. Data Rendered
The dataset used contains housing sales data with fields such as Sale Price, Number of Bedrooms, Bathrooms, Flat Area, Lot Area, Basement Area, House Age, Condition, Renovation Status, Zipcode Group, and others. The data was provided in .csv format and includes derived and transformed columns suitable for advanced analytics and visualizations in Tableau.

### 2. Data Preprocessing
Before importing the data into Tableau, preprocessing was done using Python (Pandas). The following steps were performed:
- Removed null or missing values.
- Renamed columns for clarity (e.g., “No of Bedrooms” → “Bedrooms”).
- Created calculated fields like “TotalAreaSqft” (sum of flat, lot, and basement areas).
- Generated dummy variables for house conditions and renovation status.
- Transformed categorical fields to improve Tableau usability.
The final cleaned dataset was stored and imported into Tableau for visualization.

### 3. Utilization of Filters
Multiple filters were implemented in Tableau to improve interactivity and user exploration. These include:
- Number of Bedrooms
- Number of Bathrooms
- House Condition
- Renovation Status (Yes/No)
- Zipcode Group
- Sale Price Bins

### 4. Calculated Fields Used
Several calculated fields were created in Tableau to enhance analysis and interactivity:
- TotalAreaSqft → [FlatAreaSqft] + [LotAreaSqft] + [BasementAreaSqft]
- SalePriceBin → Binning Sale Price into ₹100,000 intervals
- Condition_Excellent, Condition_Good, etc. → Dummy fields (0/1)
- Ever_Renovated_Yes → Dummy field to identify renovated homes
- AvgPrice → AVG([SalePrice]) for grouped insights
- HouseAge → Difference between year built and sale date if available (or derived field if pre-calculated)

### 5. Dashboard
Tableau dashboards were created integrating charts, filters, and KPIs for an interactive user experience.

### 6. Story Design
A Tableau story was developed to guide users step by step through the housing data insights and trends.
