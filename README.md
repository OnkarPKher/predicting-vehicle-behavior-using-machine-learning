# **Predicting Car Velocities Using Machine Learning Models**

This project involves implementing and evaluating three machine learning models—Linear Regression, Decision Tree Regression, and Neural Networks—to predict the translational velocity (`v`) and rotational velocity (`w`) of a car. The dataset comprises sensor data from multiple sources.

---

## **Project Structure**

### **Files and Directories**

```
.
├── figures/                      # Contains the figures used in the report
├── presentation.pptx            # Project presentation
├── code/                        # Jupyter notebooks
│   ├── data_preprocessing.ipynb     # Data preprocessing and preparation
│   ├── neural_networks.ipynb        # Neural network model
│   ├── linear_regression.ipynb      # Linear regression model
│   └── decision_tree_regression.ipynb # Decision tree model
├── results.pdf                  # Final report
```

---

## **Setup Instructions**

### **1. Mount Google Drive**

Ensure your datasets are stored in your Google Drive in the following structure:

```
/MyDrive/ML/
├── Train/
│   ├── Aug14_Box_g17.csv
│   ├── July22_23.csv
│   └── July28_Special_2.csv
├── Test/
│   ├── Aug14_Box_g11.csv
│   └── July22_68.csv
```

### **2. Install Required Libraries**

Make sure the following Python libraries are installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `tensorflow`
- `matplotlib`

Install them using pip:

```bash
pip install pandas numpy scikit-learn tensorflow matplotlib
```

---

## **Execution Instructions**

### **Step 1: Data Preprocessing**

- **Notebook**: `data_preprocessing.ipynb`
- **Purpose**:  
  - Concatenate training and test datasets  
  - Handle missing values  
  - Normalize features for consistent scale

**Instructions**:
1. Open the notebook and run all cells in order.
2. Ensure the preprocessed datasets are saved to `/preprocessed_data/` in your Google Drive.

---

### **Step 2: Linear Regression**

- **Notebook**: `linear_regression.ipynb`
- **Purpose**:
  - Implement Linear Regression using the preprocessed data  
  - Evaluate using MSE, MAE, and \( R^2 \)

**Instructions**:
1. Load preprocessed data from `/preprocessed_data/`.
2. Run the notebook to train and evaluate the model.

---

### **Step 3: Decision Tree Regression**

- **Notebook**: `decision_tree_regression.ipynb`
- **Purpose**:
  - Train Decision Tree Regression  
  - Tune hyperparameters such as `max_depth` and `min_samples_split`

**Instructions**:
1. Load preprocessed data from `/preprocessed_data/`.
2. Run the notebook to train and evaluate the model.

---

### **Step 4: Neural Networks**

- **Notebook**: `neural_networks.ipynb`
- **Purpose**:
  - Implement a feedforward neural network  
  - Tune batch size and learning rate  
  - Apply dropout and L2 regularization

**Instructions**:
1. Load preprocessed data from `/preprocessed_data/`.
2. Run the notebook to train the model.
3. Observe training and validation loss curves.

---

## **Important Notes**

1. **Data Location**:  
   Ensure the datasets are properly structured and accessible in your Google Drive under `/MyDrive/ML/`.

2. **Execution Environment**:  
   Use **Google Colab** for seamless integration with Google Drive and faster GPU training.

3. **Hyperparameter Tuning**:  
   Modify hyperparameters (batch size, learning rate, tree depth, etc.) in each notebook to observe effects on performance.

---
