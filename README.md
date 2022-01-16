# School District Analysis: PyCitySchools

## Overview of the PyCitySchools District Analysis: 
Explain the purpose of this analysis.

## Results: 
Using bulleted lists and images of DataFrames as support, address the following questions.

### District Summary Analysis:
  - A few of the metrics were not impacted by replacing Thomas High School ninth grade scores for math and reading with NaNs. **Metrics that weren't impacted** include: 
    - **Total Schools**
    - **Total Students**
    - **Total Budget**
  - As anticipated, replacing the scores of the 461 ninth graders at Thomas High School with **NaNs** impacted some of the metrics as outlined below: 
    - **Average Math Score:** This score decreased slightly from 79.0 to 78.9. 
      - We utilized the pandas.DataFrame.mean function() to calculate this score. Because the "skipna" parameter is "True" by default and we didn't specify otherwise, the NaN values are excluded both from the numerator (sum of math scores) as well as the denominator (count of scores) when computing the result.     
    - **Average Reading Score:** This score remained the same.
    - **% Passing Math:** The percentage of students passing math decreased slightly from 75.0% to 74.8%.
    - **% Passing Reading:** The percentage of students passing reading decreased slightly from 85.8% to 85.7%. 
    - **% Overall Passing:** The perdentage of students passing both math and reading decreased from 65.2% to 64.9%. 


![PyCitySchools_Original_District_Summary.png](Resources/PyCitySchools_Original_District_Summary.png)


![PyCitySchools_Updated_District_Summary.png](Resources/PyCitySchools_Updated_District_Summary.png)

### School Summary Analysis:
- **How is the school summary affected?**
  - **Average Math Score:** Thomas High School's score decreased slightly.  
  - **Average Reading Score:** Thomas High School's score increased slightly. 
  - **% Passing Math:** Thomas High School's % of students passing math decreased slightly. 
  - **% Passing Reading:** Thomas High School's % of students passing reading decreased slightly.
  - **% Overall Passing:** Thomas High School's % of students passing both math and reading decreased slightly.
- **How does replacing the ninth graders’ math and reading scores with NaN affect Thomas High School’s performance relative to the other schools?**
  - Despite a decrease in a majority of Thomas High School's metrics after excluding 9th graders' scores, **Thomas High School's ranking based on performance holds steady at #2.**
  - As a result of the update, there is a narrower margin between Thomas High School and the #3 School: Griffin High School.  

![PyCitySchools_Top_Schools_Original.png](Resources/PyCitySchools_Top_Schools_Original.png)

![PyCitySchools_Top_Schools_Updated.png](Resources/PyCitySchools_Top_Schools_Updated.png)

- **How does replacing the ninth-grade scores affect the following:**
  - Math and reading scores by grade
  - Scores by school spending
  - Scores by school size
  - Scores by school type

## Summary: 
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
