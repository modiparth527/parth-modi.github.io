---
title: "Student Exam Performance Indicator End To End Project"
excerpt: "Demonstrate modular coding with end-to-end data science pipeline with deployment <br/> <br/><img src='/parth-modi.github.io/images/AWS.jpeg'>"
collection: portfolio
---


The main **aim** of the project is to demonsrate **modular coding with necessary logging info and exception handling**, along with **AWS deployment**. This project predicts student exam performance based on various demographic and educational factors using a machine learning model. It is built using **Flask** for the web interface and **AWS BeanStalk** for deployment.

## Table of Contents
- [Deployment](#deployment)
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)


## AWS BeanStalk Deployment [AWS Deployment Link ](http://studentperformance-env.eba-akmabera.eu-north-1.elasticbeanstalk.com/predictdata) (If the link does not work try removing `s` from https url)

![Logo]({{site.baseurl}}/images/deployment_student.png)


## Overview

The **Student Exam Performance Indicator** aims to predict students' mathematics scores based on input features such as gender, ethnicity, parental education, lunch type, and preparation course completion status. The prediction model is a neural network trained using TensorFlow.

### Features:
- **Input**: Demographic and educational details (Gender, Race/Ethnicity, Parental Education, etc.)
- **Output**: Predicted Math Score
- **Model**: Pre-trained Neural Network model saved as `model.h5`
- **Web Interface**: Two UI options - Flask-based interface and a more interactive AWS BeanStalk deployement UI.

## Project Structure
```
MLProject/
├── data/
│   └── external/          # External data sources.
├── notebooks/             # Jupyter notebooks for exploration and analysis.
├── src/                   # Source code for the project.
│   ├── __init__.py        # Makes src a Python module.
│   ├── components/        # Scripts for data ingestion, transformation, and model training.
│   ├── pipeline/          # Scripts for predict and train pipeline.
│   ├── exception.py       # Script to raise custom exceptions.
│   └── logger.py          # Script for logging information.
├── artifacts/             # Contains train, test CSV files and .pkl files for preprocessing and scaling.
├── requirements.txt       # Python package dependencies.
├── README.md              # Project documentation (this file).
└── .gitignore             # Ignored files and directories.
```
## Installation

### Prerequisites:
- **Python 3.8+**
- **pip** for managing Python packages

### Setup:
1. **Clone the repository:**
   ```bash
   git clone https://github.com/modiparth527/mlproject
   cd student_exam_performance

2. **Create and activate a virtual environment (optional but recommended):**
    ```bash
    conda create -p venv python==3.8
    conda activate venv

3. **Install Dependencies**
    ```bash
    pip install -r requirements.txt

4. **Ensure the pre-trained model `model.h5` is present in the root directory. If not, follow `data_ingestion.py` script fot training the model in `src/compoenents` folder.**

## Usage

### Running the Application
1. **Run the Flask app:**
   ```bash
   python app.py

2. **Access the web interface: Open your web browser and go to:**
   ```bash
   http://localhost:5000
   
## Contributing

Contributions are welcome! If you'd like to contribute, please follow these steps:

1. **Fork the repository** to your own GitHub account.
2. **Create a new branch** for your feature or fix:
   ```bash
   git checkout -b feature/AmazingFeature

3. **Make your changes and commit them:**
   ```bash
   git commit -m 'Add some AmazingFeature'
4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
5. **Open a pull request on the original repository**




