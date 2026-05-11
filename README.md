# Salary-Prediction


This project aims to predict employee salaries based on demographic and professional features using a machine learning approach. It includes a dataset of employee records and a Jupyter Notebook that performs data preprocessing, exploratory data analysis, and predictive modeling.

## Project Structure

- `Dataset.csv`: The raw dataset containing employee information.
- `Predictor.ipynb`: A Jupyter Notebook containing the end-to-end pipeline (Data Loading, Encoding, Training, and Prediction).

## Dataset Overview

The dataset contains **375** entries with the following features:

- **Age**: Age of the employee.
- **Gender**: Male or Female.
- **Education Level**: Highest degree earned (Bachelor's, Master's, PhD).
- **Job Title**: The professional role held by the employee.
- **Years of Experience**: Total years of professional experience.
- **Salary**: The target variable (Annual Salary in USD).

### Sample Data
|   Age | Gender   | Education Level   | Job Title         |   Years of Experience |   Salary |
|------:|:---------|:------------------|:------------------|----------------------:|---------:|
|    32 | Male     | Bachelor's        | Software Engineer |                     5 |    90000 |
|    28 | Female   | Master's          | Data Analyst      |                     3 |    65000 |
|    45 | Male     | PhD               | Senior Manager    |                    15 |   150000 |
|    36 | Female   | Bachelor's        | Sales Associate   |                     7 |    60000 |
|    52 | Male     | Master's          | Director          |                    20 |   200000 |

## Technical Workflow

1.  **Data Preprocessing**:
    - Handling missing values (if any).
    - Encoding categorical variables (Gender, Education Level, Job Title) using Label Encoding to convert text data into numerical format for the model.
2.  **Exploratory Data Analysis (EDA)**:
    - Visualization of salary trends across different education levels and experience tiers using `matplotlib`.
3.  **Model Implementation**:
    - The project utilizes a **Linear Regression** model from the `sklearn` library.
    - Features used for training: `Age`, `Gender`, `Education Level`, `Job Title`, and `Years of Experience`.
4.  **Prediction**:
    - The notebook includes a prediction block where user-defined inputs are encoded and passed to the trained model to estimate a salary.

## Requirements

To run the notebook, you will need the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

## Usage

1. Ensure `Dataset.csv` is in the same directory as `Predictor.ipynb`.
2. Open `Predictor.ipynb` in a Jupyter environment (VS Code, JupyterLab, etc.).
3. Run all cells to train the model.
4. Use the final cells to input specific employee details and get a salary prediction.

---
