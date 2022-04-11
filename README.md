
# **PyCitySchools District Analysis** :school: :green_apple:

## Overview of the school district analysis:

The purpose of this project was to uphold state-testing standards after information came out about academic dishonesty in Thomas High School. The data affected by the dishonesty was in 9th grade in the reading and math scores. We were tasked with replacing all of the reading and math scores with for 9th grade with NaN in order to rewrite the data from the averages that were calculated out from 10th-12th grade at Thomas High School. Below we will go into detail on how we achieved this and how the data changed after we completed this task. 

## Results: 

1. ### How is the district & school summary affected?

    - The districrt summary is affected by inaccurate data if the school gets funding based off of student performance, Thomas High School may be granted more money than deserved if there are inaccurate reading and math scores for students in 9th grade. 

    - If any of the data has been tampered with and is incorrect, it will affect the ranking of the school when ranked on averages of reading and math scores. This would place Thomas High School near the top of the list of best ranking averages when in fact, their rank might be greatly affected once the data is corrected and accurate. 

    - The school summary is affected by the inaccurate data by showing that 9th graders are performing the best in both reading and math. This has negative impacts on how the district may view the teachers who are teaching those subjects. The district may think they are doing very well, when in fact, they are performing poorly and might need additional guidance that wouldnt be granted unless the data is accurate. 

## How does replacing the ninth-grade scores affect the following:

1. ### Math and reading scores by grade: 

    - By replacing the 9th grade math and reading scores, we can start to manage the data in a more accurate way. We are no longer getting false information. We can now calculate the percent passing for both math and reading, along with, the overall passing percentage without have to worry about the inaccurate data. The example shows the average math score based on grade. By replacing the 9th grade score with NaN we can now get an accurate set of data for 10th-12th grade:   

    ```
                            9th	    10th	11th	12th
    Rodriguez High School	76.9	76.6	76.4	77.7
    Shelton High School	    83.4	82.9	83.4	83.8
    Thomas High School	    nan	    83.1	83.5	83.5
    Wilson High School	    83.1	83.7	83.2	83.0
    Wright High School	    83.3	84.0	83.8	83.6 

    ```

    - The same is true from the above as the reading scores. Replacing 9th grade with NaN we accuratly get the rest of the results for 10th-12th grade as shown below:

    ```
                            9th	    10th	11th	12th
    Rodriguez High School	81.0	80.6	80.9	80.4
    Shelton High School	    84.1	83.4	84.4	82.8
    Thomas High School	    nan	    84.3	83.6	83.8
    Wilson High School	    83.9	84.0	83.8	84.3
    Wright High School	    83.8	83.8	84.2	84.1

    ```

2. ### Scores by school spending:

    - As stated previously, getting inaccurate may cause an issue when it comes to school funding and how much they receive. as you can see below, the schools who spend more on students are the ones with the lowest average scores and overall passing percentage. If Thomas High School fell into this category where they did need more money to better provide for their students, they would not receieve as much as they need due to inaccurate data. 

    ```
    Spending Ranges (Per Student)
        
            Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing					
    <$586	        83.5	               83.9	                 93	             97	                90
    $586-630	    83.6	               83.9	                 94	             96	                90
    $631-645	    79.1	               81.9	                 76	             86	                66
    $646-675	    77.0	               81.0	                 66	             81	                54

    ```

3. ### Scores by school size:

    ```
    School Size

                    Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Pass
    Small (<1000)	       83.8	                83.9	               94	            96	             90
    Medium (1000-1999)	   83.4	                83.9	               94	            97	             91
    Large (2000-5000)	   77.7	                81.3	               70	            83	             58

    ```

4. ### Scores by school type:

    ```
    School Type

                    Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Pass
    Charter	                83.5	            83.9	                94	             97	                90
    District	            77.0	            81.0	                67	             81	                54

    ```

