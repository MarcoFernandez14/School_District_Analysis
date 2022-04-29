# School_District_Analysis

## Purpose of the Analysis
A City School distric requested to analyze standarized test data and funding data to understand performance trends and patterns. These insights are used for discussion and strategic decisions at school and district level. The analysis assits the School Borad and Superintendent in making decisions regarding school budget allotments.
However, after the analysis was performed, the school board notified that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have asked to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once the data is replaced, the school district analysis the school distric analysis has to be repeted.

## Evironment
* Python 3.7.3
* Anaconda 1.9.0
* Conda 4.12.0
* Jupyter notebook 6.1.12
* Pandas 1.3.4

## Results 
The testing data of 461 9th grade students at Thomas High School was replaced by NaN with the below impacts. 
### How is the district summary affected?
Original Data  
![dristrict_summary_original](https://github.com/MarcoFernandez14/School_District_Analysis/blob/main/Resources/District%20Summary%20Original.png)
Adjusted Data  
![dristrict_summary_adjusted](https://github.com/MarcoFernandez14/School_District_Analysis/blob/main/Resources/District%20Summary%20Adjusted.png)
The changes are in the decimal numbers of ***Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, % Overall Passing***.

### How is the school summary affected?
Original Data  
![school_summary_original](https://github.com/MarcoFernandez14/School_District_Analysis/blob/main/Resources/School%20Summary%20Original.png)
Adjusted Data  
![school_summary_adjusted](https://github.com/MarcoFernandez14/School_District_Analysis/blob/main/Resources/School%20Summary%20Adjusted.png)
Note that there is a drop in the ***%Passing Math*** and the ***%Passing Reading*** and therefore the ***%Overall Passing*** decerased from 90.95% to 65.08%.
However, this is mainly because we are using the total Thomas Hight School students population to calculate the passing percentages. Once we calculate the passing percentages excluding 9th grade students' test results and students count (including only 10th to 12th grade), we obtain an ***%Overall Passing*** of 90.63%.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
#### Scores by school spending
#### Scores by school size
#### Scores by school type

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
