# Crowdfunding Analysis with Excel

## Project Overview

Crowdfunding platforms such as Kickstarter and Indiegogo have gained immense popularity since the late 2000s. These platforms have become crucial tools for launching new products, generating buzz, and gaining support from backers worldwide. However, not all crowdfunding campaigns succeed. The goal of this project is to analyze a dataset of 1,000 crowdfunding projects to uncover hidden trends and patterns that may lead to successful campaigns.

## Objective

The primary objective of this project is to use Excel to analyze and visualize key trends in crowdfunding campaigns, including success rates, funding percentages, and other metrics. We aim to draw meaningful conclusions that could help identify factors contributing to the success or failure of a crowdfunding campaign.

## Dataset

The dataset contains information on 1,000 crowdfunding projects, including:
- Project category and subcategory
- Funding goal
- Amount raised
- Number of backers
- Campaign outcome (successful, failed, canceled, live)
- Launch and end dates

## Analysis and Methodology

1. **Conditional Formatting**:  
   Applied to the outcome and percentage funded columns to visualize the success, failure, or status of each campaign using color coding.

2. **Column Creation**:
   - **Percent Funded**: A formula that calculates how much funding each campaign received relative to its funding goal.
   - **Average Donation**: A formula that calculates the average contribution per backer.
   - **Parent Category and Sub-Category**: Separated the "Category and Sub-Category" column into two distinct columns using a formula.
   - **Date Created Conversion**: Converted Unix timestamps from the launch date to Excel’s date format.
   - **Date Ended Conversion**: Converted Unix timestamps from the end date to Excel’s date format.

3. **Pivot Tables and Charts**:
   - **Category Stats**: Created a pivot table to count how many campaigns were successful, failed, canceled, or are live per category, followed by a stacked column pivot chart filtered by country.
   - **Subcategory Stats**: Created a pivot table to analyze campaign outcomes per subcategory, with a corresponding pivot chart that filters by country and parent category.
   - **Outcomes Based on Launch Date**: Created a pivot table and a line chart visualizing the campaign outcome trends by launch date, filtered by parent category and year.

4. **Crowdfunding Goal Analysis**: 
   - Created new goal ranges and computed the success, failure, and cancellation percentages for projects within each goal range.
   - Visualized the relationship between the goal amount and the likelihood of success, failure, or cancellation through a line chart.

5. **Bonus Statistical Analysis**:
   - Created summary statistics for the number of backers of successful and unsuccessful campaigns, evaluating the mean, median, minimum, maximum, variance, and standard deviation for each outcome.

## Crowdfunding Analysis Conclusions

### Key Insights:
1. **Theatre and Plays Lead in Successful Campaigns**:
   - The category "Theatre" and the sub-category "Plays" have the highest count of successful campaigns, with 187 successful projects each.
   - The highest number of successful campaigns occurred in July.

2. **Dataset Limitations**:
   - The dataset primarily focuses on the count of outcomes. For instance, Theatre has both the highest number of successful and failed campaigns, which can be misleading when drawing comparisons across categories.
   - To avoid skewed analysis, focusing on percentages instead of raw counts may provide a clearer picture of the factors contributing to campaign outcomes.

3. **Suggestions for Improved Analysis**:
   - Additional columns could be added to the dataset to calculate percentages for canceled, failed, live, and successful outcomes. These percentages can be computed by dividing the count of each outcome by the total number of outcomes in that category.
   - Pivot tables and visualizations based on these percentages would offer more insights into the trends, including:
     - Category vs. Percentage of Outcome
     - Sub-category vs. Percentage of Outcome
     - Date Created vs. Percentage of Outcome

### Statistical Analysis:
1. **Mean vs. Median**:
   - The means in this dataset are considerably larger than the medians, indicating the presence of extreme values or outliers, which are skewing the mean upwards. Therefore, the median is a better measure of central tendency in this case.

2. **Variability in Successful vs. Unsuccessful Campaigns**:
   - The data shows that successful campaigns exhibit higher variability. This is expected because successful campaigns typically have a wider range of funding goals, leading to more variability in the number of backers. On the other hand, failed campaigns are more consistent, likely reflecting their inability to attract significant support, regardless of the goal size.

## Setup and Installation

1. Download the project files from the provided link.
2. Open the Excel workbook to view and modify the datasets.
3. Review the pivot tables and charts for key insights.
4. Generate your report based on the analysis.

## Author

Kristina Abramoff
