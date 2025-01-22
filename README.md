# Bike Rental Demand Prediction Project

This project predicts bike rental demand using machine learning techniques. It downloads data from a specified URL, performs feature engineering, trains several regression models (including a stacked model), and generates a submission file.

## Table of Contents

1.  [Introduction](#introduction)
2.  [Features](#features)
3.  [Getting Started](#getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Usage](#usage)
4.  [Project Structure](#project-structure)
5.  [Model Training](#model-training)
6.  [File Descriptions](#file-descriptions)
7.  [Contributing](#contributing)
8.  [License](#license)

## Introduction

This project aims to build a predictive model for bike rental demand based on various environmental and temporal features. It demonstrates a full data science workflow from downloading data to making predictions using various models.

## Features

*   **Data Download:** Downloads compressed data from a specified URL.
*   **Data Preprocessing:** Handles missing values, performs feature engineering, and encodes categorical features.
*   **Model Training:** Implements several regression models:
    *   Ordinary Least Squares (OLS) Regression
    *   Decision Tree Regression
    *   Random Forest Regression
    *   AdaBoost Regression
    *   XGBoost Regression
    *   Stacked Model
*   **Model Evaluation:** All models are validated using the RMSLE error metric.
*   **Feature Importance:** Provides a visualization of XGBoost feature importances.
*   **Submissions:** Generates a submission CSV file with predictions.
*   **Command-Line Interface:** Uses `argparse` to allow configuration of paths from the command line.
*   **Logging:** Provides informative logging of project execution.

## Getting Started

### Prerequisites

*   Python 3.6 or higher
*   `pip` (Python package installer)
*   Internet connection (for data download)
### Installation

1.  Clone the repository:

    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2.  Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

### Usage

1.  Download the data and generate a submission file

    ```bash
    python bike_rental_project.py --input_path /path/to/your/input --working_path /path/to/your/working --submission_file submission.csv
    ```
    * Replace `/path/to/your/input` with the desired input directory, `/path/to/your/working` with the working directory, and `submission.csv` with the desired name of the submission file.

    or for the default folders:

    ```bash
    python bike_rental_project.py
    ```

   * The model will use the `/kaggle/input` and `/kaggle/working` folders for input, and create the output `submission.csv` file, you can use the parameter `--force_download` if you want to download again the data.

## Project Structure
├── bike_rental_project.py # Main Python script
├── requirements.txt # Libraries to install
└── README.md # This file

## Model Training

The code trains several models, and it shows the feature importances of the XGBoost Model, and saves the submission of the stacked model.

## File Descriptions

*   `bike_rental_project.py`: Contains the main Python script with all the project logic.
*   `requirements.txt`:  A list of the python packages required to execute the program.
*   `data`: The input folder, where the training and test set reside.
*   `submission.csv`: the submission that was created

## Contributing

Contributions are welcome! To contribute:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them.
4.  Push your changes to your fork.
5.  Submit a pull request.
