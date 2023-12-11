# COMP3125-FinalProj

## Introduction
  In the era where job mobility is common among multiple STEM fields, the analysis of salary data is of upmost importance when deciding what field to work in as well as what company. This paper attempts to analyze salary data regarding data analysts by asking questions that allows people to gain insight into this specific field. This dataset covers multiple facets impacting salary, such as experience levels, job titles, employment types and the ratio that such person works remotely. This paper will show how all these factors contribute to or diminish salary by asking three questions of the dataset. First, the analysis on whether there are significant variations in salaries across different countries. Secondly, what the correlation is between the extent of remove work and salary levels or rather are employees who work remotely more often compensated differently than those who predominantly work in office. Finally, how does the choice of job title impact salary levels within the data as well as are there any trends associated with specific job titles across different experience levels. In the context of the data analytic salaries, this paper hopes to show the influences of job title, remote work dynamics, and global variations, offering insight to current and future professionals navigating the landscape of STEM career mobility.

### Methodology: 
•	Data cleaning: removing missing values, outliers, and inconsistencies if necessary.
•	Exploring the data: Using NumPy and Pandas to decipher trends and answers to my questions.
•	Global Salary Differences: Group the data by countries and analyze the distribution of salaries.
•	Remote Work Impact: What’s the correlation between remote_ratio and salary
•	Job Title Influence: What’s the relationship between job titles and salary levels as well as identifying specific patterns associated with job titles and experience levels.
•	Conclusions
•	Documentation


## Data Selection and Cleaning
Dataset: https://www.kaggle.com/datasets/piyushborhade/salary-of-data-scientists/data 

The data contains important information regarding the salary of data scientists including, salary in USD, experience level, job titles, employment types such as full-time or part-time, whether the employee is in-person or a remote worker, and employee residency. No data cleaning was required for this dataset. 

Preview of the Data: 
![image](https://github.com/danforthcATWIT/COMP3125-FinalProj/assets/90588626/762caa83-5000-44d3-aaae-38bfece24adb)

## Methods

General Tools:
- NumPy
- Pandas
- MatplotLib
- Seaborn
- SciPy for ANOVA test

### Question 1: Are there salary disparities between different countries?
  
Created a bar graph of the means of the salaries in USD of each country to visualize if there are salary disparities. Then performed statistical tests to assess whether there are significant variations in salaries across different countries.

ANOVA is meant to compare means across multiple groups to determine if there are significant differences among them. Computing the ratio of the variance between groups to the variance within groups is necessary in determining the p value of the distribution. If the p value is greater than .05 then it is determined that significant differences in the mean salaries of each country have significant differences.

### Question 2: Remote Work and Salary

Created a scatterplot to determine the correlation coefficient between the ratio of remote work that one does and how much salary they get. Then a bar plot was necessary for better viewing the average salary of each ratio of remote work. 

Then performed an ANOVA test for confirmation of results.

### Question 3: Impact Job Titles have on Salary

Created a bar plot to show the top 50 job titles in data science in order to inform people of what they should expect their average salary to be at a certain position.

## Results

### Question 1: Global Salary Variations

It was determined that globally, there are significant salary disparties between countries.

![image](https://github.com/danforthcATWIT/COMP3125-FinalProj/assets/90588626/a7b0b04f-6cb8-41b2-b978-de7e67686b9c)

In some countries, significantly: Israel, Malaysia, Puerto Rico, the United States, Canada, and China the salary for data scientists is higher than other countries. This result allows data scientists to consider options such as cost of living, economic landscapes and salary into account if they were deciding whether to apply their skills in a specific country. 

Analyzing the data with ANOVA shows that there is a significant difference in salaries between countries.


### Question 2: Remote Work and Salary

It was shown that the decision to work a remote position does generally have an impact on salary within the data science field. On average, those who work strictly in office tend to make more than those who work strictly remote, and those who work a hybrid model make significantly less than in-person and fully remote workers. This data can be valuable when deciding what company to work at when job searching within the data science field. It was determined that the correlation coefficient between salary and remote ratio is -0.06417, meaning that it has a low correlation, but this can be attributed to the fact that both fully remote and in-person workers make significantly more than hybrid workers.

![image](https://github.com/danforthcATWIT/COMP3125-FinalProj/assets/90588626/88574f11-bb80-4603-99bb-0ecf6dc77367)

![image](https://github.com/danforthcATWIT/COMP3125-FinalProj/assets/90588626/a146e93e-8f86-41a1-9c8a-b3f2fb59e539)

Performing the ANOVA test on the data suggests that significant differences exist between fully remote, hybrid and in-person working models.


### Question 3: Impact Job Titles have on Salary

Job title has a significant impact on salary, as leader roles get paid significantly more in the data science field, such as Data Science Tech Leads, Principles of Data Science and Cloud Data Architect Leads.

![image](https://github.com/danforthcATWIT/COMP3125-FinalProj/assets/90588626/011aef0a-920f-4b9f-b5fb-ffba9a2ac32f)

## Discussion

### Global Salary Disparities 

Contributing Factors of the disparities:

Several potential factors could contribute to the identified variations. Economic conditions, cost of living, and currency exchange rates are essential considerations. Additionally, differences in labor market dynamics, industry structures, and governmental policies may play pivotal roles. Understanding the specific influence of each factor requires further investigation and could serve as a basis for more targeted compensation strategies.

### Remote Work and Compensation 

Correlation vs. Causation:

The correlation analysis between remote work ratio and salary levels provides intriguing insights into potential trends. However, it is crucial to emphasize that correlation does not imply causation. While our findings suggest a weak negative correlation, additional factors, such as job responsibilities, industry norms, and individual performance, may contribute to the observed relationship.

### Job Title Impact on Salary

Implications for Talent Management:

Understanding the influence of job titles on compensation is paramount for effective talent management. Organizations can leverage these insights to refine job classification structures, ensuring that employees are fairly compensated based on their roles and responsibilities.

## Conclusion

The research provides insightful information about the intricacies of international wage systems, the dynamics of remote employment, and how job titles affect pay. The discrepancies that have been found highlight the necessity for businesses to implement context- and talent-specific remuneration plans. Research and flexibility will be essential in promoting fair and competitive compensation systems as the professional field changes.

## References

https://www.statisticssolutions.com/free-resources/directory-of-statistical-analyses/anova/
https://www.kaggle.com/datasets/piyushborhade/salary-of-data-scientists/code

