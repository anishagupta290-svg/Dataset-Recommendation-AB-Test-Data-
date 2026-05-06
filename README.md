### 1. **Hypothesis Formulation**
The code begins by defining the statistical objectives. It sets a **Null Hypothesis (H_0)** stating that the new design has no positive effect on conversion rates, and an **Alternative Hypothesis (H_1)** asserting that the new design is significantly better.
### 2. **Data Processing and Summary**
The script loads e-commerce data to compare a **Control** group (the original design) against a **Treatment** group (the new design).
 * **Control**: 10,000 visitors with a 7.5% conversion rate.
 * **Treatment**: 10,000 visitors with a 9.0% conversion rate.
### 3. **Statistical Testing (The Core)**
The code utilizes several statistical methods to validate the results:
 * **Two-Proportion Z-Test**: This is used to determine if the 1.5% difference in conversion rates is statistically significant. With a resulting p-value of 0.000001, the code concludes that the null hypothesis should be rejected.
 * **Chi-Square Test**: This is applied to categorical relationships, such as checking if different device types (mobile vs. desktop) influenced the conversion results.
 * **T-Test**: Used for continuous metrics, specifically to see if the session duration (time spent on site) changed between the two groups.
### 4. **Experimental Design and Power Analysis**
To ensure the test was designed correctly, the code includes a **Power Analysis**. It calculates the required sample size (393 per group) needed to detect a specific effect size while maintaining an 80\% power level. This ensures the test is neither underpowered nor unnecessarily long.
### 5. **Visualization and Business Insight**
 * **Confidence Intervals**: The code generates a plot showing 95\% confidence intervals. Since the intervals for the Control and Treatment groups do not overlap, it visually confirms statistical significance.
 * **Financial Impact**: The code translates these technical findings into business terms, estimating an annual revenue impact of +\$180,000 based on the conversion lift.
### 6. **Assumption Checks**
Finally, the workflow includes "Pro Tips" to validate the underlying assumptions of the tests, such as the **Shapiro-Wilk test** for normality and the **Levene’s test** for equal variance.
