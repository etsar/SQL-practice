# Case Study #8 - Fresh Segments
<div>
<img src="https://user-images.githubusercontent.com/94500188/221339169-00f29d9c-04c6-41e3-83e0-576e587086f2.png" width="500"/>
</div>
Danny created Fresh Segments, a digital marketing agency that helps other businesses analyse trends in online ad click behaviour for their unique customer base. 
He has asked for your assistance to analyse aggregated metrics for an example client and provide some high level insights about the customer list and their interests.

## Case Study Questions
<br>**1. Data Exploration and Cleansing**
1. Update the `fresh_segments.interest_metrics` table by modifying the `month_year` column to be a date data type with the start of the month
1. What is count of records in the `fresh_segments.interest_metrics` for each `month_year` value sorted in chronological order (earliest to latest) with the null values appearing first?
1. What do you think we should do with these null values in the `fresh_segments.interest_metrics`
1. How many `interest_id` values exist in the `fresh_segments.interest_metrics` table but not in the `fresh_segments.interest_map` table? What about the other way around?
1. Summarise the `id` values in the `fresh_segments.interest_map` by its total record count in this table
1. What sort of table join should we perform for our analysis and why? Check your logic by checking the rows where `interest_id` = 21246 in your joined output and include all columns from `fresh_segments.interest_metrics` and all columns from `fresh_segments.interest_map` except from the `id` column.
1. Are there any records in your joined table where the `month_year` value is before the `created_at` value from the `fresh_segments.interest_map` table? Do you think these values are valid and why?

**2. Interest Analysis**
1. Which interests have been present in all `month_year` dates in our dataset?
1. Using this same `total_months` measure - calculate the cumulative percentage of all records starting at 14 months - which `total_months` value passes the 90% cumulative percentage value?
1. If we were to remove all `interest_id` values which are lower than the `total_months` value we found in the previous question - how many total data points would we be removing?
1. Does this decision make sense to remove these data points from a business perspective? Use an example where there are all 14 months present to a removed interest example for your arguments - think about what it means to have less months present from a segment perspective.
1. After removing these interests - how many unique interests are there for each month?

**3. Segment Analysis**
1. Using our filtered dataset by removing the interests with less than 6 months worth of data, which are the top 10 and bottom 10 interests which have the largest composition values in any `month_year`? Only use the maximum composition value for each interest but you must keep the corresponding `month_year`
1. Which 5 interests had the lowest average `ranking` value?
1. Which 5 interests had the largest standard deviation in their `percentile_ranking` value?
1. For the 5 interests found in the previous question - what was minimum and maximum `percentile_ranking` values for each interest and its corresponding `year_month` value? Can you describe what is happening for these 5 interests?
1. How would you describe our customers in this segment based off their `composition` and `ranking` values? What sort of products or services should we show to these customers and what should we avoid?

**4. Index Analysis**
<br>The `index_value` is a measure which can be used to reverse calculate the average composition for Fresh Segments’ clients.

Average composition can be calculated by dividing the `composition` column by the `index_value` column rounded to 2 decimal places.

1. What is the top 10 interests by the average composition for each month?
1. For all of these top 10 interests - which interest appears the most often?
1. What is the average of the average composition for the top 10 interests for each month?
1. What is the 3 month rolling average of the max average composition value from September 2018 to August 2019 and include the previous top ranking interests in the same output shown below.
1. Provide a possible reason why the max average composition might change from month to month? Could it signal something is not quite right with the overall business model for Fresh Segments?
