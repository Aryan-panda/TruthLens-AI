# TruthLens AI - Automated Fake News Classification

TruthLens AI is a machine learning project dedicated to classifying news articles as either real or fake. This project leverages natural language processing and machine learning models to detect potentially misleading information.

## Project Structure

- `TruthLens-AI.ipynb`: The main Jupyter Notebook containing the data exploration, preprocessing, model training, and evaluation code.
- `requirements.txt`: List of Python dependencies required to run the project.
- `data/`: Directory intended to contain the datasets used for training and testing.
  - `Fake.csv`: Dataset containing fake news articles.
  - `True.csv`: Dataset containing true news articles.
  - *(Note: Datasets are excluded from source control due to size limitations.)*
- `models/`: Directory containing the trained models and vocabulary vectorizer.
  - `decision_tree_model.pkl`: Decision Tree model.
  - `logistic_regression_model.pkl`: Logistic Regression model.
  - `gradient_boosting_model.pkl`: Gradient Boosting model.
  - `random_forest_model.pkl`: Random Forest model.
  - `tfidf_vectorizer.pkl`: TF-IDF Vectorizer.
  - *(Note: Models are excluded from source control due to size limitations.)*

## Setup and Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Aryan-panda/TruthLens-AI.git
   cd TruthLens-AI
   ```

2. **Download Datasets**
   - Obtain the datasets (`Fake.csv` and `True.csv`) and place them inside the `data/` directory.

3. **Install Dependencies**
   - Ensure you have Python installed.
   - It is recommended to use a virtual environment.
   - Install the required libraries using the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Notebook**
   ```bash
   jupyter notebook TruthLens-AI.ipynb
   ```
   - Or you can use Google Colab as well.

## Workflow

- **Data Loading and Preprocessing**: The notebook loads the data, creates a target 'class' variable, and performs necessary text cleaning.
- **Model Training**: Uses classification algorithms provided by `scikit-learn` to train models on the text data.
- **Model Saving and Loading**: The trained models and vocabulary vectorizer are saved into a `models/` directory using `joblib`. 
   - *Quick Start*: If the models are already saved in the `models/` folder, you do not need to run the entire notebook again. You can simply run the first two cells (for imports and data prep), then scroll directly to the **"Loading the Models and Predicting"** section to load the models, and run the final cell to test custom news inputs.
- **Evaluation**: The models are evaluated using accuracy scores and classification reports to determine their effectiveness in identifying fake news.
