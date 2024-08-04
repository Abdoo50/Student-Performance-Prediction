# Student Performance Prediction

This project aims to predict student performance based on various features such as gender, ethnicity, parental level of education, lunch type, test preparation course, reading score, and writing score. The project uses machine learning techniques to train a predictive model and provides a Flask web application for user interaction.

## Project Structure

```plaintext
.
├── .abextention
│   └── python.config
├── artifacts
│   ├── data.csv
│   ├── model.pkl
│   ├── preprocessor.pkl
│   ├── test.csv
│   └── train.csv
├── notebook
│   ├── catboost_info/Learn
│   └── data
│       ├── stud.csv
│       ├── 1. EDA STUDENT PERFORMANCE.ipynb
│       └── 2. MODEL TRAINING.ipynb
├── src
│   ├── components
│   │   ├── __init__.py
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   ├── pipeline
│   │   ├── __init__.py
│   │   ├── predict_pipeline.py
│   │   ├── train_pipeline.py
│   │   ├── exception.py
│   │   ├── logger.py
│   │   └── utils.py
├── templates
│   ├── home.html
│   └── index.html
├── .gitignore
├── README.md
├── application.py
├── requirements.txt
└── setup.py
```

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/Abdoo50/Student-Performance-Prediction.git
    cd Student-Performance-Prediction
    ```

2. Create and activate a virtual environment:

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```sh
    pip install -r requirements.txt
    ```

## Running the Application

1. Run the Flask application:

    ```sh
    python application.py
    ```

2. Open a web browser and navigate to `http://127.0.0.1:5000/` to access the web interface.

## Project Components

### Notebooks

- `1. EDA STUDENT PERFORMANCE.ipynb`: Exploratory Data Analysis on student performance data.
- `2. MODEL TRAINING.ipynb`: Training and evaluation of the predictive model.

### Data

- `data/stud.csv`: The dataset used for training and evaluation.

### Artifacts

- `model.pkl`: The trained machine learning model.
- `preprocessor.pkl`: The preprocessor used for data transformation.
- `train.csv`, `test.csv`: Training and testing datasets.

### Source Code

- `components/`: Contains modules for data ingestion, transformation, and model training.
- `pipeline/`: Contains the prediction and training pipelines, along with utility modules.
- `templates/`: HTML templates for the Flask web application.

## Deployment

To deploy the application on Heroku:

1. Install the Heroku CLI:

    ```sh
    curl https://cli-assets.heroku.com/install.sh | sh
    ```

2. Log in to Heroku:

    ```sh
    heroku login
    ```

3. Create a new Heroku app:

    ```sh
    heroku create
    ```

4. Push the code to Heroku:

    ```sh
    git push heroku master
    ```

5. Open the deployed app:

    ```sh
    heroku open
    ```

## Usage

The web application allows users to input student data and receive a prediction of their performance. The form accepts the following inputs:

- Gender
- Race or Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Writing Score
- Reading Score

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss any changes or improvements.

## License

This project is licensed under the MIT License.

---

This README provides a comprehensive overview of your project, including instructions for installation, running the application, and deployment on Heroku.
