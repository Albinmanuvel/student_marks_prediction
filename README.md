# Student marks prediction

Linear regression that predicts a student's marks from weekly study time and the number of courses taken. A small learning project.

## Data
`Student_Marks.csv` - 99 students, 3 columns: `number_courses`, `time_study`, `Marks`.

## What the script does (`prediction.py`)
- Quick EDA with Plotly scatter plots and a correlation check (study time vs marks: 0.94, number of courses vs marks: 0.42).
- 80/20 train/test split (`random_state=42`) and a `LinearRegression` model.
- Asks for a study time and number of courses and prints the predicted marks.

## Result
Test R2 = 0.946. With only 99 rows, one feature doing most of the work and no cross-validation, treat this as a demo of the workflow, not a reliable predictor.

## Run it
```
pip install -r requirements.txt
python prediction.py
```
`prediction.ipynb` is the notebook version of the same script.
