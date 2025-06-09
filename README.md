

\# \*\*Predicting Car Velocities Using Machine Learning Models\*\*

This project involves implementing and evaluating three machine learning models—Linear Regression, Decision Tree Regression, and Neural Networks—to predict the translational velocity (v) and rotational velocity (w) of a car. The dataset comprises sensor data from multiple sources.

-——————————————————————————————————-

\## \*\*Project Structure\*\*

\### \*\*Files and Directories\*\*

- figures

`	`-contains the figures used in the report

-‘presentation.pptx’

`	`-the presentation of the project

- code

`	`- `data\_preprocessing.ipynb’

`		`- Contains code to preprocess datasets and saves for reuse.

`	`- `neural\_networks.ipynb`

`		`- Implementation of the Neural Networks model.

`	`- `linear\_regression.ipynb`

`		`- Implementation of the Linear Regression model.

`	`- `decision\_tree\_regression.ipynb`

`		`- Implementation of the Decision Tree Regression model.

- `results.pdf’

`	`- Contains the content of the report

\---

\## \*\*Setup Instructions\*\*

\### \*\*1. Mount Google Drive\*\*

Ensure your datasets are stored in your Google Drive in the specified directory structure:

\```

/MyDrive/ML/

├── Train/

│   ├── Aug14\_Box\_g17.csv

│   ├── July22\_23.csv

│   ├── July28\_Special\_2.csv

├── Test/

│   ├── Aug14\_Box\_g11.csv

│   ├── July22\_68.csv

\```

\### \*\*2. Install Required Libraries\*\*

Make sure the following Python libraries are installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `tensorflow`
- `matplotlib`

To install them, run:

\```bash

pip install pandas numpy scikit-learn tensorflow matplotlib

\```

\---

\## \*\*Execution Instructions\*\*

\### \*\*Step 1: Data Preprocessing\*\*

- \*\*Notebook\*\*: `data\_preprocessing.ipynb`
- \*\*Purpose\*\*:
- Concatenate training and testing datasets.
- Handle missing values.
- Scale features for consistency.
- \*\*Steps\*\*:
1. Open the notebook and execute the cells sequentially.
1. Ensure the preprocessed datasets are saved to `/preprocessed\_data/`. On your google drive folder.

\### \*\*Step 2: Linear Regression\*\*

- \*\*Notebook\*\*: `linear\_regression.ipynb`
- \*\*Purpose\*\*:
- Implement Linear Regression on preprocessed data.
- Evaluate performance using MSE, MAE, and \(R^2\).
- \*\*Steps\*\*:
1. Load the preprocessed datasets saved in `/preprocessed\_data/`.
1. Run the notebook to train and evaluate the Linear Regression model.

\### \*\*Step 3: Decision Tree Regression\*\*

- \*\*Notebook\*\*: `decision\_tree\_regression.ipynb`
- \*\*Purpose\*\*:
- Implement Decision Tree Regression on preprocessed data.
- Fine-tune hyperparameters like `max\_depth` and `min\_samples\_split`.
- \*\*Steps\*\*:
1. Load the preprocessed datasets saved in `/preprocessed\_data/`.
1. Run the notebook to train and evaluate the Decision Tree model.

\### \*\*Step 4: Neural Networks\*\*

- \*\*Notebook\*\*: `neural\_networks.ipynb`
- \*\*Purpose\*\*:
- Implement a feedforward neural network with dropout and L2 regularization.
- Fine-tune batch size and learning rate.
- \*\*Steps\*\*:
1. Load the preprocessed datasets saved in `/preprocessed\_data/`.
1. Run the notebook to train and evaluate the Neural Network model.
1. Observe training and validation loss curves.

\---

\## \*\*Important Notes\*\*

1. \*\*Data Location\*\*:
- Ensure datasets are correctly placed in the specified directory structure on Google Drive.

2\. \*\*Execution Environment\*\*:

- Use Google Colab for seamless integration with Google Drive.

3\. \*\*Hyperparameter Tuning\*\*:

- Modify the hyperparameters in each notebook's respective section to observe their effects.

\---
