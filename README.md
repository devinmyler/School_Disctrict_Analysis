# Analysing School District Test Scores and Financial Summary

## Overview
### In the beginning
The purpose of the analysis is to use Jupyter Notebook, Python, and Pandas library to clean, merge, sort, and analyze school data, including Student Test Scores, School Budgets, and other information in an entire school district. The data comes in two separate CSV files.

### And Then...
Once the data is cleaned and merged and dataframes are created to analyse the data, some of the student test scores need to be wiped due to cheating. The data is updated to reflect the changes and then re-analyzed, leaving us with two different sources of analysis to comapre: one including the cheating ninth graders from Thomas High School (THS), and one without.

## Results
In total, only 461 out of 39,170 students' math and reading scores were removed from the data. How did that affect the analysis?

### The District Summary
The original data:
![District Summary original](https://user-images.githubusercontent.com/78869891/112777917-53d14700-9011-11eb-85ce-e2d0475d02e8.png)
The updated data:
![District Summary refactored](https://user-images.githubusercontent.com/78869891/112777921-5633a100-9011-11eb-838b-6fbbeb1fcbfb.png)

As you can see, the district's passing percentages were affected negatively by the removal of the THS 9th graders, though not by much. In the district as a whole, the removed group only makes up 1.17% of the data population; so changes on a district level were never going to be drastic.


### The School Summary
THS has 1,635 students. The removed 9th graders make up 28.2% of the population. However, upon their removal from the data, there doesn't seem to be any remarkable shift in the data.
Original:
![per_school_summary_original](https://user-images.githubusercontent.com/78869891/112778990-c0e5dc00-9013-11eb-8dc6-223d5fa8e010.png)

Updated:
![per_school_summary_df_refactored (2)](https://user-images.githubusercontent.com/78869891/112778997-c511f980-9013-11eb-9cea-96230f8a3c88.png)

### Relative Performance
Original:
![school_comparison_original](https://user-images.githubusercontent.com/78869891/112779652-30100000-9015-11eb-9b28-d2f798c77a38.png)
Updated:
![school_comparison_refactored](https://user-images.githubusercontent.com/78869891/112779671-3aca9500-9015-11eb-8afa-897e82f7303c.png)

Relative to other schools, the new data doesn't affect THS's place in the top schools in the district. They remain in second place out of all schools, whther the 9th graders are included or not.

### Other Effects
- Scores by Grade
Obviously only the 9th grade averages would be affected. 
The average of all schools 9th grade reading scores went from 82.5% to 82.42%
The average of all schools 9th grade math scores went from 80.35% to 80.12%
While not a significant change, the ninth grade math scores is where we see tha largest shift.
- Scores by School Spending
Four schools are in the same spending category as THS, and they're all much larger schools. The average scores for this spending category were unaffected by the 9th grader's removal.
- Scores by School Size
The data for the schools in the same size category were also unaffected.
- School Type
The data for schools in the same type were also unaffected.


## Summary
There are no "major" changes to the data. However, Thomas High School's scores did drop-- just not significantly. The areas most affected were: 
- Math scores by grade in the 9th grade bin
- Thomas High Schools overall  passing percentage
- Reading scores by grade in the 9th grade bin
- The district's overall passing percentages
All in all, the 9th graders from Thomas High School do not make up a large enough portion of the data to make significant changes.
