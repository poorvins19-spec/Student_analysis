# 📊 Student Outcomes Analysis

## 📌 Project Overview

Student Outcomes Analysis is a data analysis project developed using Python to explore student academic performance. The project examines students' marks, identifies high performers, studies the relationship between attendance and marks, calculates pass/fail counts, and visualizes the distribution of marks.

This project is based on a student performance analysis scenario for **EduPulse Analytics**, where the objective is to understand student outcomes using data analysis techniques.

## 🎯 Objectives

- Calculate the average marks of all students.
- Identify students scoring above 75 marks.
- Analyze the correlation between attendance percentage and marks.
- Create a `Pass` column based on students' marks.
- Calculate the total number of students who passed and failed.
- Visualize the distribution of student marks using a histogram.

## 🛠️ Technologies Used

- **Python** — programming language
- **Pandas** — data manipulation and analysis
- **Matplotlib** — data visualization
- **Jupyter Notebook / Google Colab** — interactive coding environment
- **CSV** — dataset format

## 📂 Project Structure

```text
student-outcomes-analysis/
│
├── README.md
├── student_outcomes_analysis.ipynb
└── student_performance_dataset.csv
```

*Note: Upload `student_performance_dataset.csv` separately if you have the dataset. It was not included with the notebook I reviewed.*

## 📊 Project Tasks and Implementation

### 1. Average Marks Calculation

Uses Pandas to calculate the mean of the `Marks` column and display the average to two decimal places.

### 2. High Performers Analysis

Filters students whose marks are greater than 75 and calculates how many students meet this condition.

### 3. Attendance and Marks Correlation

Calculates the Pearson correlation coefficient between `Attendance_Percentage` and `Marks` to examine the relationship between attendance and academic performance.

A positive coefficient indicates a positive relationship, a negative coefficient indicates an inverse relationship, and a value near zero indicates a weak linear relationship. Correlation alone does not establish causation.

### 4. Pass/Fail Classification

Creates a new column named `Pass` using the following rule:

- `True` if Marks ≥ 50
- `False` if Marks < 50

### 5. Pass and Fail Counts

Counts the total number of students who passed and failed based on the `Pass` column.

### 6. Marks Distribution Visualization

Creates a histogram of student marks using Matplotlib, including:
- Chart title
- X-axis label: Marks
- Y-axis label: Number of Students
- Optional grid lines

## ⚙️ Requirements

Install the required Python libraries:

```bash
pip install pandas matplotlib jupyter
```

## ▶️ How to Run the Project

1. Clone or download this repository.
2. Make sure `student_performance_dataset.csv` is available in the correct location.
3. Open the notebook in Jupyter Notebook or Google Colab.
4. Update the dataset path if necessary.
5. Run the notebook cells in order.
6. Review the calculated results and histogram.

Example for opening Jupyter Notebook:

```bash
jupyter notebook
```

**Important:** The current notebook uses this Google Colab path:

```python
pd.read_csv("/content/student_performance_dataset.csv")
```

If running locally, change it to the appropriate local path, for example:

```python
df = pd.read_csv("student_performance_dataset.csv")
```

## 📈 Expected Outcomes

After running the notebook, the analysis provides:

- Average student marks
- Number of students scoring above 75
- Attendance–marks correlation coefficient
- Pass/fail classification for each student
- Total pass and fail counts
- A histogram showing the distribution of marks

Actual numerical results depend on the dataset used.

## 🎓 Learning Outcomes

This project demonstrates practical skills in:

- Loading and analyzing CSV data
- Filtering rows using conditions
- Calculating summary statistics
- Using correlation for exploratory data analysis
- Creating new columns with Boolean conditions
- Counting categories
- Creating visualizations with Matplotlib

## 🚀 Future Improvements

- Add more visualizations to compare attendance and marks.
- Identify students who may need academic support.
- Create an interactive dashboard.
- Include additional factors such as assignment scores and study hours, if the relevant data is available.
- Add data validation and missing-value handling.

## 👩‍💻 Author

**Poorvi N S**

B.Tech — Artificial Intelligence and Machine Learning

## 📄 License

This project is available for educational and learning purposes. Add a formal license if you want to specify permissions for reuse and redistribution.
