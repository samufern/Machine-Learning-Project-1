# Machine Learning Project 1

## 📌 Project Overview
This project focuses on **classification using machine learning**. It includes multiple iterations of model development, datasets, and a final trained model ready for predictions.

## 🚀 Getting Started

### 📋 Prerequisites
Ensure you have the following installed:
- Python 3.x
- Jupyter Notebook
- Required dependencies (install using `requirements.txt` if available)

Install dependencies using:
```sh
pip install -r requirements.txt
```

### 🔧 Installation
Clone the repository:
```sh
git clone https://github.com/your_username/Machine-Learning-Project-1.git
cd Machine-Learning-Project-1
```

## 🏗 Project Structure
```
Machine-Learning-Project-1/
│── aprendizaje automatico.pdf  # Documentation about the project
│── modelo_inicial.ipynb         # Initial approach to the model
│── modelo_clasificacion.ipynb   # Classification model development
│── modelo_final.ipynb           # Optimized model
│── modelo_final.pkl             # Trained machine learning model
│── predicciones.csv             # Output predictions from the model
│── wind_ava.csv.gz              # Input dataset (compressed)
│── wind_comp.csv.gz             # Additional dataset (compressed)
```

## 🎯 Usage

### Running the Model
Open the Jupyter Notebooks:
```sh
jupyter notebook modelo_final.ipynb
```

Or use the trained model for predictions:
```python
import pickle
import pandas as pd

# Load model
with open("modelo_final.pkl", "rb") as f:
    model = pickle.load(f)

# Example usage
X_new = pd.read_csv("wind_ava.csv.gz")
predictions = model.predict(X_new)
print(predictions)
```

## ✅ Testing
To test the model's performance, use `modelo_final.ipynb`, where evaluation metrics are included.

## 🛠 Built With
- **Python 3**
- **scikit-learn** - Machine Learning Library
- **pandas & NumPy** - Data processing
- **Jupyter Notebook** - Interactive model development

## 🤝 Contributing
If you wish to contribute, feel free to fork the repository, make improvements, and submit a pull request.

---

