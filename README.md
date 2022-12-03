# pandas-challenge
## PyCitySchools Report
# District Summary
- I created a district summary that displayed the total number of schools, the total budget of the district, the average math score, the average reading score, the percentage of students passing math, the percentage of students passing reading, and the percentage of students passing both math and reading.
# School Summary
- I created a school summary that displays the school name, school type, total students per school, total school budget, per student budget, average math score, average reading score, percentage of students passing math, percentage of students passing reading, and the percentage of students passing both math and reading.
# Highest-Performing Schools
- I acquired the names of the highest performing school based on the percentage of students passing both math and reading. The top 5 performing schools were:
    - Cabrera High School, Thomas High School, Griffin High School, Wilson High School, and Pena High School.
    - All of these schools are charter schools.
    - Three of the top school have a total number of students between 1000 and 2000, one of the schools has a total number of students below 1000, and one of the schools has a total number of students above 2000.
    - Two of the schools have a per students budget below $585, two of the schools have a per student budget between $585 and $630, one school has a per student budget between $630 and $645.
# Lowest-Performing Schools
- I acquired the names of the lowest performing school based on the percentage of students passing both math and reading. The bottom 5 performing schools were:
    - Rodriguez High School, Figueroa High School, Huang High School, Hernandez High School, and Johnson High School.
    - All of these schools are district schools.
    - All of the schools have a total number of students between 2000 and 5000.
    - Two of the schools have a per students budget between $630 and $645, three of the schools have a per student budget between $645 and $680.
# Math Scores by Grade
- I calculated the average math scores of each school by grade. The average math scores of each school are about the same across all grades.
# Reading Scores by Grade
- I calculated the average reading scores of each school by grade. The average reading scores of each school are about the same across all grades.
# Scores by School Spending
- I divided school spending per student into four categories and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing. The categories are:
    - <$585: the averages and percentage of passing students are the highest in this group across all categories.
    - $585-630: this group is the second best performing across all categories.
    - $630-645: this group is the third best performing across all categories.
    -$645-680: the averages and percentage of passing students are the lowest in this group across all categories.
# Scores by School Size
- I divided schools by number of students into three categories and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing. The categories are:
    - Small (<1000): this group has the highest average math score, and the highest average reading score.
    - Medium (1000-2000): this group has the highest % passing math, % passing reading, and % overall passing.
    - Large (2000-5000): this group is the worst performing across all categories.
- There is not much difference between the averages and % passing of small and medium schools.
# Scores by School Type
- I divided the schools by school type and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing.
    - Charter: charter schools perform better across all categories.
    - District: district schools perform worse across all categories.
# Conclusions
- The charter schools in the district tend to perform better in math and reading. This is proven by the fact that the top 5 performing schools were all charter schools, and the bottom 5 performing schools were all district schools.
- It seems that large schools perform worse, their scores in math and reading were much lower than the scores of schools of small and medium size. The bottom 5 performing schools were all large schools.
- It seems that as per student budget increases performance decreases, with the worst performing schools having a per student budget above $630, while all the top performing schools except one had a per student budget below $630.