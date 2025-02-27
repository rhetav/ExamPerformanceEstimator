# Student Performance Indicator

## Overview
The **Student Performance Indicator** is an end-to-end machine learning project that predicts students' performance based on various academic and socio-economic factors. The project follows a structured ML pipeline, from data preprocessing to model deployment.

## Features
- Data collection and preprocessing
- Feature engineering and selection
- Model training and evaluation
- Web application for predictions
- Deployment using cloud services

## Tech Stack
- **Programming Language:** Python
- **Machine Learning:** Scikit-learn, CatBoost
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Web Framework:** Flask
- **Deployment:** AWS Elastic Beanstalk

## Project Structure
```
StudentPerformanceIndicator/
│-- .ebextensions/        # AWS deployment configurations
│-- artifacts/            # Stores model artifacts
│-- catboost_info/        # CatBoost logs
│-- notebook/             # Jupyter Notebooks for analysis
│-- src/                  # Source code
│   │-- components/       # ML pipeline components
│   │-- config/           # Configuration settings
│   │-- pipeline/         # Data pipeline scripts
│   │-- utils/            # Utility functions
│-- templates/            # HTML templates for web app
│-- application.py        # Flask app entry point
│-- requirements.txt      # Python dependencies
│-- setup.py              # Installation script
│-- README.md             # Project documentation
```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/rhetav/StudentPerformanceIndicator.git
   ```
2. Navigate to the project directory:
   ```bash
   cd StudentPerformanceIndicator
   ```
3. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the Flask application locally:
   ```bash
   python application.py
   ```
2. Open a browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```
3. Upload student data and get predictions.

## Deployment
To deploy the application on AWS Elastic Beanstalk:
1. Install AWS Elastic Beanstalk CLI.
2. Initialize and deploy:
   ```bash
   eb init -p python-3.7 StudentPerformanceIndicator
   eb create student-performance-env
   ```

## Contributing
Feel free to submit issues or pull requests for improvements.

## License
This project is licensed under the MIT License.

