
# Module-4-Challenge
Dear Grader,

Sorry for the late submission. I've been working through challenges but fell behind and haven't submitted. 

Module 4 Challenge citations
1. Combining the data into a single dataset
# Read School and Student Data File and store into Pandas DataFrames
school_data = pd.read_csv(school_data_to_load)
student_data = pd.read_csv(student_data_to_load)

# Combine the data into a single dataset.  
school_data_complete = pd.merge(student_data, school_data, how="left", on=["school_name", "school_name"])
school_data_complete.head()

I received this code from a study group to get started on this challenge

2. Float function
   # Use the following to calculate the percentage of students who passed math (math scores greather than or equal to 70)
passing_math_count = school_data_complete[(school_data_complete["math_score"] >= 70)].count()["student_name"]
passing_math_percentage = passing_math_count / float(student_count) * 100
passing_math_percentage

This was from a study group

3. Dataframe construction
# Use the following to calculate the percentage of students who passed math (math scores greather than or equal to 70)
passing_math_count = school_data_complete[(school_data_complete["math_score"] >= 70)].count()["student_name"]
passing_math_percentage = passing_math_count / float(student_count) * 100
passing_math_percentage

# Create a DataFrame called per_school_summary with columns for the calculations
per_school_summary = pd.DataFrame({
    "School Type": school_type,
    "Total Students": per_school_counts,
    "Total School Budget": per_school_budget,
    "Per Student Budget": per_school_capita,
    "Average Math Score": per_school_math,
    "Average Reading Score": per_school_reading,
    "overall_passing_rate": overall_passing_rate,
})

unique_school_types

# Display the DataFrame
print("PER_SCHOOL_SUMMARY")
per_school_summary

Chat GPT
