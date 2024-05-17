# Water Quality Classification Using KNN

## Introduction

In this project, we classify the potability of water samples using the K-Nearest Neighbors (KNN) algorithm. Ensuring safe and potable water is crucial for public health, and machine learning techniques can provide valuable insights and predictions about water quality based on various chemical and physical attributes.

## Dataset

The dataset used for this project is sourced from Kaggle: [Water Quality Dataset](https://www.kaggle.com/code/amitpant7/k-nearest-neighbor/input)

## Project Structure

- **data**: Contains the dataset files.
- **notebooks**: Jupyter notebooks for data analysis and model training.
- **src**: Source code for data preprocessing, model training, and evaluation.
- **README.md**: Project overview and instructions.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/water-quality-classification.git
    cd water-quality-classification
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate   # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Preprocess the data:
    ```python
    # Example code snippet
    from src.preprocessing import preprocess_data
    data = preprocess_data('data/water_quality.csv')
    ```

2. Train and evaluate the model:
    ```python
    from src.model import train_eval
    train_eval(data)
    ```

3. Testing different k-values:
    ```python
    from src.model import test_k_values
    test_k_values(data)
    ```

## Example

Below is an example of how to use the provided scripts to train and evaluate the KNN model:

```python
# Import necessary functions
from src.preprocessing import preprocess_data
from src.model import train_eval, test_k_values

# Load and preprocess the data
data = preprocess_data('data/water_quality.csv')

# Train and evaluate the KNN model
train_eval(data)

# Test different k-values for KNN
test_k_values(data)


##Thank You ChatGPT :)