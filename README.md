# ExamPerformancePredictor

A machine learning project that predicts student performance based on various academic and socio-economic factors. This project leverages supervised learning techniques to analyze student data and provide insights that can help educators and stakeholders make informed decisions.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Project Structure](#project-structure)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview
This project is aimed at predicting student performance based on a dataset containing academic scores, demographic details, and other influencing factors. The goal is to identify patterns and provide actionable insights that can improve educational outcomes.

## Features
- Data preprocessing and feature engineering
- Exploratory Data Analysis (EDA)
- Supervised learning models for prediction
- Model evaluation and hyperparameter tuning
- Deployment using Flask and AWS Elastic Beanstalk (optional)

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn (for visualization)
- Flask (for API deployment)
- AWS Elastic Beanstalk (for cloud deployment)

## Installation
Clone the repository and install dependencies:

```bash
 git clone https://github.com/rhetav/StudentPerformanceIndicator.git
 cd StudentPerformanceIndicator
 pip install -r requirements.txt
```

## Usage
1. Prepare the dataset and ensure it is placed in the appropriate directory.
2. Run the data preprocessing and model training script:
   ```bash
   python train.py
   ```
3. Evaluate model performance:
   ```bash
   python evaluate.py
   ```
4. (Optional) Deploy the model using Flask:
   ```bash
   python app.py
   ```

## Deployment
### Local Deployment with Flask
To run the application locally:
```bash
python app.py
```
The API will be accessible at `http://127.0.0.1:5000/`.

### AWS Elastic Beanstalk Deployment (Optional)

#### Steps to Deploy:
##### Create a Web App on AWS Elastic Beanstalk:
* Navigate to the AWS Elastic Beanstalk console.
* Select Python as the platform.
* Choose Sample Application for the application code.
* Create the web application.

##### Set Up an Automated Deployment Pipeline with AWS CodePipeline:
* Navigate to AWS CodePipeline and create a new pipeline.
* Select GitHub as the source provider.
* Link your GitHub account and project repository.
* Skip the Build Stage (optional).
* Choose AWS Elastic Beanstalk as the deployment provider.
* Create the pipeline to enable continuous deployment.

## Project Structure
```
StudentPerformanceIndicator/
│── data/                 # Dataset files
│── notebooks/            # Jupyter notebooks for EDA
│── src/                  # Source code
│   ├── preprocessing.py  # Data preprocessing scripts
│   ├── model.py          # Machine learning models
│   ├── train.py          # Training script
│   ├── evaluate.py       # Evaluation script
│── app.py                # Flask API
│── requirements.txt      # Dependencies
│── .ebextensions/        # AWS Beanstalk configuration (if applicable)
│── README.md             # Project documentation
```

## Results
- Model performance metrics (accuracy, precision, recall, etc.)
- Key insights from data analysis
- Feature importance and their impact on predictions

## Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request with your improvements.

## License
This project is licensed under the MIT License.
