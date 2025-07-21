# Graduate Admission Prediction

This repository contains a machine learning project to predict the chance of admission for graduate school applicants. The prediction is based on several factors, including GRE Score, TOEFL Score, University Rating, Statement of Purpose (SOP), Letter of Recommendation (LOR), CGPA, and Research experience.

## Table of Contents

  - [Overview](https://www.google.com/search?q=%23overview)
  - [Dataset](https://www.google.com/search?q=%23dataset)
  - [Project Structure](https://www.google.com/search?q=%23project-structure)
  - [Features](https://www.google.com/search?q=%23features)
  - [Installation](https://www.google.com/search?q=%23installation)
  - [Usage](https://www.google.com/search?q=%23usage)
  - [Results](https://www.google.com/search?q=%23results)
  - [Contributing](https://www.google.com/search?q=%23contributing)
  - [License](https://www.google.com/search?q=%23license)

## Overview

The goal of this project is to build a predictive model that can estimate an applicant's probability of gaining admission to a graduate program. This can be a useful tool for prospective students to assess their chances and for universities to screen applicants.

The core of the project is a Jupyter Notebook (`Admission prediction.ipynb`) that demonstrates the data exploration, preprocessing, model training, and prediction steps.

## Dataset

The `admission_predict.csv` file contains the dataset used for this project. It includes the following columns:

  - `Serial No.`: Unique identifier for each applicant.
  - `GRE Score`: Graduate Record Examination (GRE) score (out of 340).
  - `TOEFL Score`: Test of English as a Foreign Language (TOEFL) score (out of 120).
  - `University Rating`: Rating of the university (1-5, where 5 is best).
  - `SOP`: Statement of Purpose strength (out of 5).
  - ` LOR  `: Letter of Recommendation strength (out of 5).
  - `CGPA`: Cumulative Grade Point Average (out of 10).
  - `Research`: Binary variable (0 or 1) indicating whether the applicant has research experience.
  - ` Chance of Admit  `: Chance of admission (ranging from 0 to 1). This is the target variable.

## Project Structure

```
.
├── Admission prediction.ipynb
├── admission_predict.csv
└── README.md
```

  - `Admission prediction.ipynb`: The main Jupyter Notebook containing the Python code for data analysis, model training, and prediction.
  - `admission_predict.csv`: The dataset used in the project.
  - `README.md`: This file, providing an overview of the project.

## Features

  - **Data Exploration**: Initial analysis of the dataset to understand its structure and distributions.
  - **Data Preprocessing**: Handling of any missing values or data transformations (though the provided notebook snippet doesn't explicitly show this, it's a common step in such projects).
  - **Model Training**: Training a machine learning model (likely a regression model given the "Chance of Admit" target) to predict admission probabilities. The notebook snippet shows `model.predict`, implying a model has been trained.
  - **Prediction**: Demonstrating how to make predictions with new input data.

## Installation

To run this project locally, you need to have Python and Jupyter Notebook installed.

1.  **Clone the repository:**

    ```bash
    git clone https://your-github-repo-link.git
    cd your-repo-name
    ```

2.  **Install the required libraries:**
    You can install the necessary libraries using `pip`. Based on the notebook, you'll likely need:

    ```bash
    pip install numpy pandas matplotlib scikit-learn
    ```

    (Note: If you encounter issues, check the `Admission prediction.ipynb` file for a complete list of imported libraries and install them accordingly.)

## Usage

1.  **Open the Jupyter Notebook:**

    ```bash
    jupyter notebook "Admission prediction.ipynb"
    ```

2.  **Run the cells:**
    Execute the cells in the notebook sequentially to explore the data, train the model, and see the prediction examples.

    The notebook includes examples of predicting the "Chance of getting into UCLA" (this is likely a placeholder for a general university, as the dataset doesn't specify UCLA). You can modify the input values in the prediction cells to test different applicant profiles.

    Example prediction from the notebook:

    ```python
    # Prediction 1
    # Input in the form : GRE, TOEFL, University Rating, SOP, LOR, CGPA, Research
    print('Chance of getting into UCLA is {}%'.format(round(model.predict([[337, 118, 4, 4.5, 4.5, 9.65, 0]])[0]*100, 3)))
    ```

## Results

The trained model provides a predicted "Chance of Admit" percentage. For instance, the notebook demonstrates predictions like:

  - `Chance of getting into UCLA is 92.855%`
  - `Chance of getting into UCLA is 73.627%`

These results indicate the model's estimated probability of admission for given applicant profiles.

## Contributing

Contributions are welcome\! If you have suggestions for improvements, new features, or bug fixes, please open an issue or submit a pull request.

## License

This project is open-sourced under the [MIT License](https://www.google.com/search?q=LICENSE). 
