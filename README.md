
# Mushroom Classification

A machine learning project designed to classify mushrooms as edible or poisonous based on their physical characteristics. This application leverages a trained model to predict mushroom edibility, providing an interactive interface for users.

## Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Installation](#installation)
* [Usage](#usage)
* [Project Structure](#project-structure)
* [Model Training](#model-training)
* [Deployment](#deployment)
* [Contributing](#contributing)
* [License](#license)

## Overview

This project utilizes a dataset of mushroom characteristics to train a classification model. The model predicts whether a mushroom is edible or poisonous, aiding in educational and research purposes.

## Features

* **Data Preprocessing**: Cleans and prepares the dataset for modeling.
* **Model Training**: Implements machine learning algorithms to train the classifier.
* **Web Interface**: Provides a user-friendly interface for input and prediction.
* **Deployment Ready**: Configured for deployment on platforms like Heroku.

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Gauravsin522/Mushroom.git
   cd Mushroom
   ```

2. **Create a virtual environment**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the application**:

   ```bash
   python app.py
   ```

2. **Access the web interface**:
   Open your browser and navigate to `http://localhost:5000`.

3. **Make predictions**:
   Input mushroom characteristics into the form to receive edibility predictions.

## Project Structure

```
├── static/
├── templates/
├── app.py
├── requirements.txt
├── mushroom_classifier.pkl
├── mushrooms.csv
├── Mushroom_Classification_Training.ipynb
├── Mushroom_HLD.pdf
├── Mushroom_LLD.pdf
├── Wireframe_Documentation_Mushroom_Classification.pdf
├── Procfile
└── .gitignore
```

* **static/**: Contains static files like CSS and images.
* **templates/**: HTML templates for rendering web pages.
* **app.py**: Main Flask application script.
* **requirements.txt**: Lists Python dependencies.
* **mushroom\_classifier.pkl**: Serialized trained model.
* **mushrooms.csv**: Dataset used for training.
* **Mushroom\_Classification\_Training.ipynb**: Jupyter notebook detailing the training process.
* **Mushroom\_HLD.pdf**: High-Level Design document.
* **Mushroom\_LLD.pdf**: Low-Level Design document.
* **Wireframe\_Documentation\_Mushroom\_Classification.pdf**: Wireframe designs for the application.
* **Procfile**: Configuration file for deployment on Heroku.
* **.gitignore**: Specifies files to ignore in version control.

## Model Training

The model was trained using the dataset provided in `mushrooms.csv`. The training process includes:

* Data cleaning and preprocessing.
* Feature encoding.
* Model selection and evaluation.
* Saving the trained model as `mushroom_classifier.pkl`.

For detailed steps, refer to the `Mushroom_Classification_Training.ipynb` notebook.

## Deployment

To deploy the application on Heroku:

1. **Install the Heroku CLI**: [Heroku CLI Installation Guide](https://devcenter.heroku.com/articles/heroku-cli)

2. **Login to Heroku**:

   ```bash
   heroku login
   ```

3. **Create a new Heroku app**:

   ```bash
   heroku create your-app-name
   ```

4. **Deploy the application**:

   ```bash
   git push heroku main
   ```

5. **Open the deployed app**:

   ```bash
   heroku open
   ```

Ensure that the `Procfile` and `requirements.txt` are present in the root directory for successful deployment.

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork the repository**.

2. **Create a new branch**:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Commit your changes**:

   ```bash
   git commit -m "Add your message here"
   ```

4. **Push to the branch**:

   ```bash
   git push origin feature/your-feature-name
   ```

5. **Open a pull request**.

Please ensure your code adheres to the project's coding standards and includes relevant tests.

## License

This project is licensed under the [MIT License](LICENSE).

