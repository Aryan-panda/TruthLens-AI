# TruthLens AI - Automated Fake News Classification

TruthLens AI is a machine learning project dedicated to classifying news articles as either real or fake. This project leverages natural language processing and machine learning models to detect potentially misleading information.

## Project Structure

- `TruthLens-AI.ipynb`: The main Jupyter Notebook containing the data exploration, preprocessing, model training, and evaluation code.
- `data/`: Directory intended to contain the datasets used for training and testing.
  - `Fake.csv`: Dataset containing fake news articles.
  - `True.csv`: Dataset containing true news articles.
  - *(Note: Datasets are excluded from source control due to size limitations.)*

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
   - Install the required libraries (pandas, numpy, seaborn, matplotlib, scikit-learn).
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn notebook
   ```

4. **Run the Notebook**
   ```bash
   jupyter notebook TruthLens-AI.ipynb
   ```

## Workflow

- **Data Loading and Preprocessing**: The notebook loads the data, creates a target 'class' variable, and performs necessary text cleaning.
- **Model Training**: Uses classification algorithms provided by `scikit-learn` to train models on the text data.
- **Evaluation**: The models are evaluated using accuracy scores and classification reports to determine their effectiveness in identifying fake news.
