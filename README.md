# pandas-challenge
## PyCitySchools Report
I used `pandas` to create a report analyzing the performance of schools in a district.

1. First, I loaded the data from a csv file containing all school data, `schools_complete.csv`, and a csv file containing all student data, `students_complete.csv`. I used `merge()` to store the school and student data in one dataframe.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/students_schools_merged.png)

2. I created a district summary by using `count()` to obtain the number of schools in the dataset and to obtain the total number of students in the dataset. I used `sum()` to calculate the total budget of the district. I used `mean()` to calculate the average math and reading scores of the district, calculated the percentage of students passing math, the percentage of students passing reading, and the percentage of students passing both. I stored this data in a dataframe. 

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/district_summary.png)

3. I created a list of the schools and what type of school they are, district or charter, by selecting only the `school_name` and `type` columns from the dataset and using `groupby()` to show each school only once in the list. 

4. I used `value_counts()` to obtain the number of students in each school. I obtained the budget of each school and divided it by the number of students to obtain the budget per student. I also obtained the average math score and average reading score per school. I obtained the percentage of students passing math, the percentage passing reading, and the percentage passing both for each school. I used this data to create a school summary.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/school_summary.png)

5. I acquired the names of the highest performing school based on the percentage of students passing both math and reading using `sort_values()` on the `% Overall Passing` column. The top 5 performing schools were:
    - Cabrera High School, Thomas High School, Griffin High School, Wilson High School, and Pena High School.
    - All of these schools are charter schools.
    - Three of the top schools have a total number of students between 1000 and 2000, one of the schools has a total number of students below 1000, and one of the schools has a total number of students above 2000.
    - Two of the schools have a per students budget below $585, two of the schools have a per student budget between $585 and $630, one school has a per student budget between $630 and $645.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/highest_performing.png)

6. I acquired the names of the lowest performing school based on the percentage of students passing both math and reading, I used `sort_values()` on the `% Overall Passing` column. The bottom 5 performing schools were:
    - Rodriguez High School, Figueroa High School, Huang High School, Hernandez High School, and Johnson High School.
    - All of these schools are district schools.
    - All of the schools have a total number of students between 2000 and 5000.
    - Two of the schools have a per students budget between $630 and $645, three of the schools have a per student budget between $645 and $680.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/lowest_performing.png)

7. I calculated the average math scores of each school by grade. The average math scores of each school are about the same across all grades.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/math_grade.png)

8. I calculated the average reading scores of each school by grade. The average reading scores of each school are about the same across all grades.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/reading_grade.png)

9. I divided school spending per student into four categories and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing. The categories are:
    - <$585: the averages and percentage of passing students are the highest in this group across all categories.
    - $585-630: this group is the second best performing across all categories.
    - $630-645: this group is the third best performing across all categories.
    -$645-680: the averages and percentage of passing students are the lowest in this group across all categories.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/scores_spending.png)

10. I divided schools by number of students into three categories and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing. The categories are:
    - Small (<1000): this group has the highest average math score, and the highest average reading score.
    - Medium (1000-2000): this group has the highest % passing math, % passing reading, and % overall passing.
    - Large (2000-5000): this group is the worst performing across all categories.
    - There is not much difference between the averages and % passing of small and medium schools.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/scores_size.png)

11. I divided the schools by school type and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing.
    - Charter: charter schools perform better across all categories.
    - District: district schools perform worse across all categories.

![alt text](https://github.com/glongo001/pandas-challenge/blob/main/PyCitySchools/Images/scores_type.png)

### Conclusions
- The charter schools in the district tend to perform better in math and reading. This is proven by the fact that the top 5 performing schools were all charter schools, and the bottom 5 performing schools were all district schools.
- It seems that large schools perform worse, their scores in math and reading were much lower than the scores of schools of small and medium size. The bottom 5 performing schools were all large schools.
- It seems that as per student budget increases performance decreases, with the worst performing schools having a per student budget above $630, while all the top performing schools except one had a per student budget below $630.