# PyBer_Analysis

## **<h1 align="center"> School District Analysis**




  ## Overview of the school district analysis: 
<p align="justify">Reviewing the previous analysis, school board has identified something anomaly in source file, students_complete.csv. Authority noticed an evidence of academic dishonesty. Specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Now new analysis has been furnished by replacing the math and reading scores for Thomas High School with NaNs and keeping the rest of the data intact. <p>

<p align="justify">This new analysis consists of two technical analysis.<p>

  - Replace ninth-grade reading and math scores
  - Repeat the school district analysis

 
  School district analysis PyCitySchools_Challenge.ipynb file link -  [ School district analysis](https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb)  

  
- Resources :
  - Data source : schools_complete.csv, students_complete.csv
  - Software : Pandas library, Jupyter Notebook


  
  
 ## School district analysis Results: 
  
<p align="justify"> The following metrics are recreated to repeat the school district analysis : 


  - The district summary
  - The school summary
  - The top 5 and bottom 5 performing schools, based on the overall passing rate
  - The average math score for each grade level from each school
  - The average reading score for each grade level from each school
  - The scores by school spending per student, by school size, and by school type
 <p>
  
<p align="justify">
  i) The district summary has been changed after replacing the 9th grade students of Thomas High School. At present Overall passing rate is 64.9, whereas Previously was 65.2. It can be visualized by following snapshot. <p>
  
  
  Present :   
<p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/Resources/2.%20Dct_summary_without%209th%20grade.png
</p>
  
  Previous : 
<p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/Resources/1.%20Dct_summary_with%209th%20grade.png
</p>
  
The command to select all the reading scores from the 9th grade at Thomas High School and replaced them with NaN: 
 
```ruby
    
    student_data_df.loc[(student_data_df["school_name"]=="Thomas High School") & (student_data_df["grade"]=="9th"),"reading_score"]=np.nan

```
  

  The command to replace the overall passing percentage for Thomas High School in the per_school_summary_df: 
 
```ruby
    
    per_school_summary_df.loc["Thomas High School", "% Overall Passing"] = passing_math_reading_percentage_THS

```
 
  
  
  <p align="justify"> ii)	The school summary of Thomas High school has been changed after replacing the 9th grade students of Thomas High School. At present, Overall passing rate is 90.63 (approx), whereas Previously was 65.07 (approx). It can be visualized by following snapshot. <p>
  
  Present :   
<p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/Resources/4.%20School_summary_without%209th%20grade.png
</p>
  
  Previous : 
<p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/Resources/3.%20School_summary_with%209th%20grade.png        
</p>
   
  
  
 

  
iii) Among the 15 schools the overall performance of Thomas High School’s position is 2nd, earlier which was 13th.
  Present performance of Thomas High school relative to the other schools :
  
  <p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/Resources/6.%20Top_School_without%209th%20grade.png       
</p>
  
  Previous performance of Thomas High school relative to the other schools :

  <p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/Resources/5.%20Top_School_with%209th%20grade.png       
</p>
  
  
<p align="justify"> iv)	Since the ninth-grade scores of Thomas High school was replaced, in dataframe of each grade level Series for average math scores showing NaN. That means, 9th grade of Thomas school has no performance both on reading and math. It also impacted in spending range while creating spending_summary on Scores by school, size_summary on Scores by school size and type_summary on Scores by school type. </p>



  

     
    
    
    
## School district analysis Summary:
<p align="justify">Finally, school district analysis have been updated after replacing the reading and math scores for the ninth grade at Thomas High School with NaNs. </p>

<p align="justify">Overall changes was visualized on the district summary, the school summary, performance of Thomas High school based on the overall passing rate,  the scores by school spending per student, by school size, and by school type.</p>



