# School_District_Analysis

## Overview of the school district analysis: 
Explain the purpose of this analysis.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

- How is the **district summary** affected?
  - A few of the metrics were not impacted by replacing Thomas High School ninth grade scores for math and reading with NaNs. **Metrics that weren't impacted** include: 
    - Total Schools
    - Total Students
    - Total Budget
  - As anticipated, replacing the scores of the 461 ninth graders at Thomas High School with NaNs impacted the metrics that utilized math and reading scores for mathematical calculation: 
    - Average Math Score: With the Thomas High School ninth grade scores excluded, the average math score decreased slightly from 79.0 to 78.9. We utilized the pandas.DataFrame.mean function() to calculate this score. Because the "skipna" parameter is "True" by default, the NaN values are excluded both from the numerator (sum of math scores) as well as the denominator (count of scores) when computing the result.     
    - Average Reading Score: This score remained the same.
    - % Passing Math: The percentage of students passing math decreased slightly from 75.0% to 74.8%.
    - % Passing Reading: The percentage of students passing reading decreased slightly from 85.8% to 85.7%. 
    - % Overall Passing: The perdentage of students passing both math and reading decreased from 65.2% to 64.9%.  
- How is the school summary affected?
- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- How does replacing the ninth-grade scores affect the following:
  - Math and reading scores by grade
  - Scores by school spending
  - Scores by school size
  - Scores by school type

## Summary: 
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
