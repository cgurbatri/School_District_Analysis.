# School District Analysis

## Purpose of Analysis
The goal of this analysis is to use school and student data to provide insight into school and student performance trends and patterns. Information gathered here will ultimately inform decisions made at the district level about budget priorities. The original data files can be found in the **Resources** folder and are also linked here: [schools_complete.csv](https://github.com/cgurbatri/School_District_Analysis./files/6490552/schools_complete.csv) and [students_complete.csv](https://github.com/cgurbatri/School_District_Analysis./files/6490553/students_complete.csv). Between these two datasets a plethora of information is available to aid in evaluating trends. These parameters include: School name, school type, school size, school budget, student name, gender, grade, reading score, math score, and which school the students attend.

## Challenge
The district uncovered some academic dishonesty at Thomas High School among the 9th grade students. The district requested an updated analysis with these incorrect math and reading scores removed. This represented 461 students of the 1,635 students at Thomas High School and of the total 31,970 students across the 15 schools. To do this, the scores were replaced with "NaN" values and all other correspinding information was kept to minmize affect on subsequent analysis. Our analysis explores how this affected the average math and reading scores, percent passing, school spending, budgets, and overall performance/ranking of schools in the district.

## Results
### District School Summary 

**Fig. 1** Prior to THS 9th grade student score removal

<img width="632" alt="District_summary_includes_THS_9th" src="https://user-images.githubusercontent.com/45336910/118423907-1cd3f500-b694-11eb-964a-3181f6a52050.png">

**Fig. 2** After to THS 9th grade student score removal

<img width="631" alt="District_summary_removes_THS_9th" src="https://user-images.githubusercontent.com/45336910/118423828-e4ccb200-b693-11eb-81cd-2091970a3f4d.png">

Since we only replaced the math and reading scores, parameters like "Total Schools, Total students, Total Budget" will remain the same, as is shown in **Fig 1 and 2**. In fact, the avaerage scores and percent passing metrics remain relatively similar as well. While removing the scores of those 461 students, slightly decreased overall average scores and the percent of students who had passing math and reading scores, the affect is less than a percentage. **We can therefore conclude that the district summary was minimally affected across all metrics**


### School Summary 

**Fig. 3** Prior to THS 9th grade student score removal

<img width="910" alt="school_summary_includes_THS_9th" src="https://user-images.githubusercontent.com/45336910/118424344-15f9b200-b695-11eb-81c9-7f9de88ebe84.png">

**Fig. 4** After to THS 9th grade student score removal
<img width="902" alt="school_summary_removes_THS_9th" src="https://user-images.githubusercontent.com/45336910/118425212-b56b7480-b696-11eb-91ea-49b1e26f349d.png">

* As shown in **Fig. 3 and 4**, the percent who passed math, reading, and both standardized for Thomas High School decreased by ~25 -30% across all those categories when 9th grade scores were removed, but students were still included in total student count.

**Fig. 6** Removal of THS 9th grade scores and inclusion of only 10th - 12th graders. 
* When only 10th-12th graders are considered in the student count, Thomas High school maintained it's position in the top 5 performing school's in the district with an overall passing percentage of ~90%. 

### Effect of Budget
**Fig. 6** Budget and scores

<img width="767" alt="budget" src="https://user-images.githubusercontent.com/45336910/118427211-b0102900-b69a-11eb-8319-14d4c41d5f05.png">

Analysis shows that an schools that spend less money per student appear to have higher average scores and a higher percentage of overall passing. Thomas High School, outperforms other schools that spend similarly to it ($630-644) with an average percent passing of ~90 as shown in **Fig. 6**.

### Effect of School size
**Fig. 7 School size and scores**

<img width="696" alt="school_size" src="https://user-images.githubusercontent.com/45336910/118427628-a935e600-b69b-11eb-8f02-5191376ab16c.png">

Thomas High school was categrozied as a medium size school with 1,000-2,000 students. When the metrics and scores in **Fig. 6** are considered, Thomas High School performed similarly to other schools its size (**Fig. 7**). Indeed, smaller schools tended to have better average scores, but the difference between small and medium sizes is negligible. 

### Effect of School Type
**Fig. 8 Charter vs District and scores**

 <img width="652" alt="school_type" src="https://user-images.githubusercontent.com/45336910/118427922-4a24a100-b69c-11eb-91e0-1db49c835114.png">

Charter schools (like Thomas High School) drastically outperform district type schools as shown in **Fig. 8** with ~40% more students passing overall. In fact all top 5 performing schools were charter schools and all bottom 5 performing schools were district-type schools.

### Effect of Grade Level
**Fig. 9 Average math score by grade**

<img width="270" alt="math_scores_by_grade" src="https://user-images.githubusercontent.com/45336910/118428480-8dcbda80-b69d-11eb-8847-0eceaca474e1.png">

**Fig. 10 Average reading score by grade**

<img width="285" alt="reading_scores_by_grade" src="https://user-images.githubusercontent.com/45336910/118428515-9e7c5080-b69d-11eb-8f34-2d3a0050ed9d.png">

Student grade level does not affect average scores as much as the school attended and other aforementioned metrics. Average math scores and reading scores are shown in **Fig. 9 and 10** respectively. 

## Summary
* Replacing the ninth graders' scores with NaN decreased the overall passing percentages at Thomas High School
* Thomas High School was no longer in the top 5 ranked schools when the analysis still included 9th graders in the total student count, but ommitted their scores
* When considering only 10th through 12th graders in the student count, Thomas High school performed as expected from a school with it's spending per student, size, and type. 
* In general, smaller charter schools that spend < $584 per student have the higher average scores and overall passing percentages. 
