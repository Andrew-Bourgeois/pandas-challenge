**# pandas-challenge**
**UNC-CH-DA Module 4-Python Challenge**

**Instructions for Running Scripts:**
* Clone the repository to your local
* Ensure you cd into the /PyCitySchools directory, and use the **PyCitySchools_Bourgeois.ipynb** Jupyter Notebook.
* The 'Resources' folder containing the relevant csvs should also be located in
the /PyCitySchools folder.

**Background:** As the new Chief Data Scientist for your city's school district, use a Jupyter Notebook and the Pandas library: analyze the district-wide standardized test results. Aggregate and organize the data to showcase obvious trends in school performance.

Report your findings so the school board and mayor can make strategic decisions regarding future school budgets and priorities.

**Assignment Requirements:**

**District Summary (20 points)**
*   Calculate the total number of unique schools (2 points)
*   Calculate the total number of students (2 points)
*   Calculate the total budget (2 points)
*   Calculate the average (mean) math score (2 points)
*   Calculate the average (mean) reading score (2 points)
*   Use the code provided to calculate the percentage of students who passed math (2 points)
*   Calculate the percentage of students who passed reading (2 points)
*   Use the code provided to calculate the percentage of students that passed both math and reading (2 points)
*   Create a new DataFrame for the above calculations called district_summary (4 points)

**School Summary (20 points)**
*   Use the code provided to select the school type (2 points)
*   Calculate the total student count (2 points)
*   Use the code provided to calculate the per capita spending (2 points)
*   Calculate the average test scores (2 points)
*   Calculate the number of schools with math scores of 70 or higher (2 points)
*   Calculate the number of schools with reading scores of 70 or higher (2 points)
*   Use the provided code to calculate the schools that passed both math and reading with scores of 70 or higher (2 points)
*   Use the provided code to calculate the passing rates (2 points)
*   Create a new DataFrame for the above calculations called per_school_summary (4 points)

**Highest-Performing Schools by Percentage of Overall Passing (5 points)**
*   Sort the schools by % Overall Passing in descending order (2 points)
*   Save the results to a DataFrame called top_schools (2 points)
*   Display the first 5 rows (1 point)

**Lowest-Performing Schools by Percentage of Overall Passing (5 points)**
*   Sort the schools by % Overall Passing in ascending order (2 points)
*   Save the results to a DataFrame called bottom_schools (2 points)
*   Display the first 5 rows (1 point)

**Math Scores by Grade (10 points)**
*   Use the code provided to separate the data by grade (1 points)
*   Group by "school_name" and take the mean of each (4 points)
*   Use the code to select only the math_score (1 points)
*   Combine each of the scores above into single DataFrame called math_scores_by_grade (4 points)

**Reading Scores by Grade (10 points)**
*   Use the code provided to separate the data by grade (1 points)
*   Group by "school_name" and take the mean of each (4 points)
*   Use the code to select only the reading_score (1 points)
*   Combine each of the scores above into single DataFrame called reading_scores_by_grade (4 points)

**Scores by School Spending (5 points)**
*   Use pd.cut with the provided code to bin the data by the spending ranges (2 points)
*   Use the code provided to calculate the averages (1 points)
*   Create the spending_summary DataFrame using the binned and averaged spending data (2 points)

**Scores by School Size (5 points)**
*   Use pd.cut with the provided code to bin the data by the school sizes (2 points)
*   Use the code provided to calculate the averages (1 points)
*   Create the size_summary DataFrame using the binned and averaged size data (2 points)

**Scores by School Type (5 points)**
Group the per_school_summary DataFrame by "School Type" and average the results (2 points)
Use the code provided to select the new column data (1 point)
Create a new DataFrame called type_summary that uses the new column data (2 points)

**Written Report (15 points)**
To receive all points, the written report presents a cohesive written analysis that:
*   Summarizes the analysis (5 points)
*   Draws two correct conclusions or comparisons from the calculations (10 points)


**References:**
* For revieweing additional parameters available with the .grouby() method: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html?highlight=groupby#pandas.DataFrame.groupby

* For determining how best to handle setting the index of a DataFrame: https://sparkbyexamples.com/pandas/pandas-set-index-to-column-in-dataframe/

* The .nunique() method for counting the number of schools by name: https://www.w3schools.com/python/pandas/ref_df_nunique.asp 

* .str.replace() to remove "$" to cast the Per Student Budeget to a "flaot", and clarification on a "regex" warning: https://stackoverflow.com/questions/66603854/futurewarning-the-default-value-of-regex-will-change-from-true-to-false-in-a-fu

* Data generated by Mockaroo, LLC, (2022), https://mockaroo.com/. Realistic Data Generator. Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.