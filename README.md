# Student Performance Prediction

This project is a web application built with Flask that predicts student performance based on various factors such as gender, race/ethnicity, parental level of education, lunch type, test preparation course, reading score, and writing score.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Installation

To get started with this project, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Abdoo50/Student-Performance-Prediction.git
   cd Student-Performance-Prediction
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment:**
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the Flask application:**
   ```bash
   python app.py
   ```

2. **Open your web browser and navigate to:**
   ```
   http://127.0.0.1:5000/
   ```

3. **Use the web interface to input student data and get predictions.**

## Deployment

### Deploying to Heroku

To deploy this Flask application to Heroku, follow these steps:

1. **Log in to Heroku:**
   ```bash
   heroku login
   ```

2. **Create a new Heroku app:**
   ```bash
   heroku create your-app-name
   ```

3. **Add your files to Git and commit:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

4. **Push your code to Heroku:**
   ```bash
   git push heroku master
   ```

5. **Open your app in a web browser:**
   ```bash
   heroku open
   ```

### Example Project Structure

```
Student-Performance-Prediction/
│
├── app.py
├── requirements.txt
├── Procfile
├── templates/
│   ├── index.html
│   └── home.html
└── src/
    ├── pipeline/
    │   ├── predict_pipeline.py
    │   └── ...
    ├── exception.py
    ├── logger.py
    └── ...
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
