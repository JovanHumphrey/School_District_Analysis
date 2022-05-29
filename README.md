# School_District_Analysis

## Background

PyCity School District is preparing to analyze the standardized test scores in reading and math across all high schools in the district. Initially, I was tasked with cleaning the data and sorting it to help the district analyze trends in performance and per-capita spending. Unfortunately, after my initial aggregation and analysis it was discovered that one school, Thomas High School (THS), had shown signs of academic dishonesty in scores of 9th grade students. The data needed to be analyzed again, replacing THS's 9th grade reading and math scores and keeping the rest of the data, such as budget and spending intact. After that I was able to re-run my analysis of the district and school summaries, determine the top five and bottom five performing schools, calculate the average math and reading scores per grade, and compare the scores by per-capita spending.
## Process
The process of replacing the data of THS was straightforward. Using the loc method I was able to extract the inaccurate data and replace it with NaN values. In total the tests of 461 students were updated.
## Results
Once the faulty data was replaced, I was able to provide answers to the following questions:
<b>How has the district summary been affected?</b>
District-wide the results decreased by a small margin. Passing Math counts and percentages went from 2,9370 and 74.98% respectively, to 2,8939 and 74.67%.
Similarly, the results of Passing Reading when from 3,3610 students at 85.80% to 3,3158 students at 85.65%.
Unsurprisingly, students who passed both also went down, from 25,528 and 65.17% to 25,105 and 64.85%.
<b>How is the school summary affected?</b>
TSH itself saw similar changes. After removing the faulty tests 1174 students remained. Originally, when the tests of all 1,635 students were counted 93.27% (1,525 students) got a passing math score, 97.30% (1,591 students) got a passing reading score, and 90.94% (1,487 students) passed both. When 9th grade scores were dropped the new numbers showed that only 93.18% (1,094 students) passed math, 97.01% (1,139 students) passed reading, and 90.63% (1,064 students) passed both.
<b>How does replacing the 9th grade's math and reading score affect Thomas High School’s performance relative to the other schools?</b>
Despite having the 9th-grade data removed THS kept its spot as the number two performing school.

<b>How does replacing the 9th grade scores affect math and reading scores?</b>
Overall average math score at THS went down from 83.41% to 83.35%, while average reading scores went up from 83.84 to 83.89% after 9th grade was removed.
<b>How does replacing the 9th grade scores affect scores by school spending?</b>
I put the spending ranges into 5 bins: "$586", "$586-630", "$631-645", and "$646-675". Initial data showed: ![original_spending](link)
After removing the 9th grade data it looked like ![updated_spending](link)
<b>How does replacing the 9th grade scores affect scores by school size?</b>
I put school sizes into 3 bins: "Small (<1000)", "Medium (1000-1999)", and "Large (2000-5000)". Initial date showed ![original_size](link)
After removing the 9th grade data it looked like ![updated_size](link)
<b>How does replacing the 9th grade scores by school type?</b>
Lastly the schools were divided into two types: distric schools and charter schools. Initially the data looked like ![original_type]
After removing the 9th grade data it looked like ![updated_type](link)
## Summary
In the end I was able to analyze the aggregate date without including the faulty scores provided by testing. Though the changes to the scores and percentages didn't change a lot without that information it is still useful to get accurate metrics. If the accusations of dishonesty are later discovered to be incorrect, THS's 9th grade values can be easily added back.
