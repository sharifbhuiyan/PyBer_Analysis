## **<h1 align="center"> PyBer_Analysis**




  ## Overview of the PyBer_Analysis: 
<p align="justify">The analysis shows how the data differs by city type and how those differences can be used by decision-makers at PyBer. A summary DataFrame of the ride-sharing data has been created by city type. This dataframe shows the weekly fare by city type.  Then, using Pandas and Matplotlib, a multiple-line graph has been created that shows the total weekly fares for each city type. <p>

<p align="justify">This analysis consists of two technical analysis.<p>

  - A ride-sharing summary DataFrame by city type
  - A multiple-line chart of total fares for each city type

 
  PyBer_Analysis PyBer_Challenge.ipynb file link -  [ PyBer Analysis](https://github.com/sharifbhuiyan/PyBer_Analysis/blob/main/PyBer_Challenge.ipynb)  

  
- Resources :
  - Data source : city_data.csv, ride_data.csv
  - Software : Pandas library, Matplotlib library. Jupyter Notebook


  
  
 ## PyBer_Analysis Results: 
  
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
  <img width="800" src=https://github.com/sharifbhuiyan/PyBer_Analysis/blob/main/analysis/pyber%20summary.png
</p>
  
  Previous : 
<p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/PyBer_Analysis/blob/main/analysis/pyber%20weekly%20fare.png
</p>
  
 # 8. Create a new DataFrame using the "resample()" function by week 'W' and get the sum of the fares for each week.
  ```ruby
    
    pyber_fare_resample_df=pyber_fare_range_df.resample("w").sum()

```
 

  
  
Previous : 
<p align="center">
  <img width="800" src=https://github.com/sharifbhuiyan/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png
</p>
  
The command to select all the reading scores from the 9th grade at Thomas High School and replaced them with NaN: 
 

  # Use the graph style fivethirtyeight.

  ```ruby
    
    style.use('fivethirtyeight')

```
  

  The command to replace the overall passing percentage for Thomas High School in the per_school_summary_df: 
 
  # Save Figure
```ruby
    
  
  plt.savefig("analysis/PyBer_fare_summary.png")

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



