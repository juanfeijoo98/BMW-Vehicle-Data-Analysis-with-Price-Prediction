# BMW Vehicle Data Analysis with Price Prediction

📌 Overview

This project focuses on analyzing BMW vehicle data using Exploratory Data Analysis (EDA) and Machine Learning to estimate vehicle prices. The dataset contains various features such as mileage, model year, and fuel type, which are used to develop a pricing prediction model.

📂 Project Structure

📁 data/ → Contains the datasets used for training and testing.

📁 notebooks/ → Jupyter Notebooks with analysis and model development.

📁 images/ → Visualizations and performance comparison graphs.

📄 requirements.txt → List of dependencies required to run the project.

📄 README.md → Documentation about the project.

📊 Data Analysis and Preprocessing

The following steps were performed on the dataset:

Data Cleaning: Handling missing values, duplicate entries, and inconsistent formats.

Exploratory Data Analysis (EDA): Statistical analysis, correlation studies, and visualization using Seaborn & Matplotlib.

Feature Engineering: Transforming categorical variables, scaling numerical features, and feature selection.

Splitting Data: Training and test datasets to ensure proper model validation.

🤖 Machine Learning Model

The project implemented a Random Forest Regressor to predict vehicle prices. The model was trained and evaluated using the following metrics:

Mean Squared Error (MSE)

R-squared (R²) Score

Model Implementation

# Import required libraries
from sklearn.ensemble import RandomForestRegressor
from sklearn.metrics import mean_squared_error, r2_score

# Create the model
model = RandomForestRegressor(random_state=42)

# Train the model
model.fit(X_train, y_train)

# Make predictions
y_pred = model.predict(X_test)

# Evaluate model performance
mse = mean_squared_error(y_test, y_pred)
r2 = r2_score(y_test, y_pred)
print(f"MSE: {mse}")
print(f"R2 Score: {r2}")

Model Results:

MSE: 17684408.806016598
R2 Score: 0.7779191886858828

🔧 Technologies Used

Python (pandas, NumPy, scikit-learn, Seaborn, Matplotlib)

Jupyter Notebook (for interactive data analysis)

Git & GitHub (for version control and collaboration)

📌 How to Run the Project

Clone the repository:

git clone https://github.com/juanfeijoo98/BMW-Vehicle-Data-Analysis-with-Price-Prediction.git

Install dependencies:

pip install -r requirements.txt

Open the Jupyter Notebook and run the analysis.

📌 Project Status

✅ Data Cleaning and Preprocessing
✅ Exploratory Data Analysis (EDA)
✅ Feature Engineering
✅ Model Training with Random Forest Regressor
✅ Model Evaluation

🛠 Last updated: (dd/mm/yyyy)

📌 How to Contribute

Fork this repository.

Create a new branch:

git checkout -b feature/new-feature

Make changes and commit them:

git commit -m "Added improvements to model evaluation"

Submit a Pull Request for review.

📩 Contact

📧 Email: juanfeijoo98@gmail.com🔗 LinkedIn: Profile🔗 GitHub: Repository

