# A/B Test Analysis for E-Commerce Interface Optimization

### Project Description<br>
This project involved analyzing an A/B test conducted by an international online retailer to evaluate the effectiveness of a new interface featuring a recommendation system. Although the test was partially abandoned, we were provided with the data to perform a comprehensive impact assessment. The analysis covered the period from December 7, 2020, to January 1, 2021.

### Objectives<br>
   * Verify data quality and integrity: duplicates, null values, and data types.<br>
   * Assess group balance between control and test segments.<br>
   * Analyze user behavior across the conversion funnel stages.<br>
   * Compare conversion rates between the original interface and the recommendation-based interface.<br>
   * Apply a Z-test to determine whether observed differences were statistically significant.<br>

### Methodology<br>
Using Python and libraries such as pandas, NumPy, Seaborn, Plotly, SciPy, and StatsModels, I performed an exploratory analysis and evaluated the validity of the A/B test. The work included:<br>

  - Data cleaning: date conversions, detection of null and duplicate values, and removal of users appearing in both groups.<br>
  - Conversion funnel creation to visualize behavior at each stage: login, product view, cart, and purchase.<br>
  - Calculation of key metrics (conversion rates, coefficients of variation).<br>
  - Graphical comparison of Groups A and B.<br>
  - Z-test application to compare conversions between interfaces.<br>

### Key Findings<br>
   * Uneven distribution of users and events: Group A had significantly more participation in the recommendation test (14,215 events vs. 3,979 in Group B).<br>

   * Higher conversion with the traditional interface:<br>
      * In the control group, the traditional interface outperformed the recommendation interface at all key stages (up to 7.23% more purchases).<br>
      * In the test group, the traditional interface also performed better (up to 12.39% more product_page views).<br>

   * The Z-test (p = 0.099) found no statistically significant difference between groups, so the null hypothesis could not be rejected.<br>

   * Recommendation: Do not proceed with implementing the recommendation system, as it showed no improvement in conversion and may be counterproductive.<br>

### Tools & Technologies<br>
   - Python (pandas, numpy, matplotlib, seaborn, plotly, scipy, statsmodels)<br>
   - Jupyter Notebook for documenting the analysis<br>
   - Z-test for proportions for statistical validation<br>

This analysis delivered a robust evaluation of an incomplete A/B test, enabling informed decisions on product direction and website optimization strategies.
