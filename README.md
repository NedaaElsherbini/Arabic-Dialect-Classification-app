# Arabic Dialect Classification

Welcome to the **Arabic Dialect Classification** project! 🌟 This project is designed to predict the dialect of Arabic text using natural language processing (NLP) and machine learning techniques. It distinguishes between various Arabic dialects, enabling linguistic analysis and cultural insights.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Project Overview

Arabic is a rich and diverse language with distinct dialects across different regions. This project addresses the challenge of identifying these dialects by implementing a robust classification system. It leverages machine learning and deep learning models to accurately predict the dialect of input Arabic text.

## Features

- **Multiclass Classification**: Classifies Arabic text into one of five dialects: Egyptian, Lebanese, Sudanese, Moroccan, and Libyan.
- **Machine Learning Models**: Utilizes logistic regression and multinomial Naive Bayes for efficient classification.
- **Deep Learning Model**: Implements an LSTM-based architecture for advanced text analysis.
- **Web Application**: Provides a Flask-based web interface and RESTful API for real-time dialect predictions.
- **Text Preprocessing**: Employs TF-IDF and CountVectorizer for feature extraction to enhance NLP accuracy.

## Dataset

The dataset for this project is sourced from the **Qatar Computing Research Institute**. It includes a diverse collection of Arabic text samples labeled with their corresponding dialects. For more details, refer to their paper: [Dialect Identification in the Arab World](https://example.com).

## Installation

To set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/NedaaElsherbini/Arabic-Dialect-Classification-app.git
   cd Arabic-Dialect-Classification-app
   ```

2. **Install Dependencies**:
   Ensure you have Python 3.8+ installed. Then, install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up the Environment**:
   - Ensure you have the dataset from the Qatar Computing Research Institute.
   - Update the dataset path in the configuration file (e.g., `config.py`).

4. **Run the Application**:
   Start the Flask web server:
   ```bash
   python app.py
   ```

## Usage

1. **Web Interface**:
   - Open your browser and navigate to `http://localhost:5000`.
   - Enter Arabic text in the provided input field to receive dialect predictions.

2. **API Access**:
   - Send a POST request to the API endpoint:
     ```bash
     curl -X POST -H "Content-Type: application/json" -d '{"text": "Your Arabic text here"}' http://localhost:5000/predict
     ```
   - The response will include the predicted dialect and confidence score.

3. **Command Line**:
   - Run the prediction script directly:
     ```bash
     python predict.py --text "Your Arabic text here"
     ```

## Model Details

The project employs the following models:

- **Logistic Regression**: A baseline machine learning model for text classification.
- **Multinomial Naive Bayes**: Optimized with CountVectorizer, achieving 82% accuracy in deployment.
- **LSTM-based Deep Learning Model**: Captures sequential patterns in text for improved accuracy.

**Preprocessing**:
- Text is preprocessed using TF-IDF and CountVectorizer to convert raw text into numerical features.
- Stop words, punctuation, and special characters are removed to enhance model performance.

## Results

The Multinomial Naive Bayes model, combined with CountVectorizer, achieved an accuracy of **82%** in the deployment phase. This model demonstrates robust performance in real-world scenarios, effectively distinguishing between the five Arabic dialects.

| Model                  | Accuracy  | Notes                              |
|------------------------|-----------|------------------------------------|
| Logistic Regression    | TBD       | Baseline model, fast training     |
| Multinomial Naive Bayes| 82%       | Best performing in deployment     |
| LSTM (Deep Learning)   | TBD       | Captures complex text patterns     |

## Future Enhancements

- **Model Fine-tuning**: Improve classification accuracy through hyperparameter optimization.
- **Expanded Dialects**: Include additional Arabic dialects for broader coverage.
![Web App Screenshot](https://github.com/NedaaElsherbini/Arabic-Dialect-Classification-app/blob/master/Web%20App.png)



## Acknowledgements

- **Qatar Computing Research Institute** for providing the dataset.
- Thanks to **Mariam Mahmoud** for their inspiring work in this area, which greatly influenced the direction and approach of this project.

## Contact

For questions or feedback, please reach out to:
- **GitHub**: [NedaaElsherbini](https://github.com/NedaaElsherbini)
- **Email**: [nedaaelsherbini@gmail.com]

---




