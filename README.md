# Housing Price Prediction – 

This project demonstrates how to run **inference on housing data** using a trained Machine Learning model and preprocessing pipeline. The notebook loads a saved model, applies transformations to new input data, and generates predictions for `median_house_value`.

## 📌 Features
* Loads a pre-trained regression model (`model.pkl`)
* Applies preprocessing using a saved pipeline (`pipeline.pkl`)
* Reads input data from `input.csv`
* Generates predictions and adds them to the dataset
* Saves the final output to `output.csv`

## 📁 Project Structure
```
.
├── main.ipynb          # Main inference notebook
├── model.pkl            # Trained ML model (required)
├── pipeline.pkl         # Preprocessing pipeline (required)
├── input.csv            # Input data for prediction
└── output.csv           # Generated predictions
```

## 🚀 How to Run the Project
1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```
2. Make sure the following files are present:
   * `model.pkl`
   * `pipeline.pkl`
   * `input.csv`
3. Open the notebook:
   ```bash
   jupyter notebook main.ipynb
   ```
4. Run the cells — the script will:
   * Load the model and pipeline
   * Transform the input data
   * Predict housing prices
   * Save results to `output.csv`

## 📊 Input Format
The `input.csv` file should contain the same columns used during training, except for the target column (`median_house_value`).
Example:
```
longitude,latitude,housing_median_age,total_rooms,total_bedrooms,population,households,median_income
-122.23,37.88,41,880,129,322,126,8.3252
```

## 📤 Output
A new `output.csv` file will be created containing the original input data plus an additional column:
```
median_house_value
```
This represents the predicted price for each row.

## 🧠 Tools & Libraries Used
* Python
* Pandas
* NumPy
* Scikit-learn
* Joblib
* Jupyter Notebook

## 🙌 Contribution
Feel free to open issues or submit pull requests if you want to improve or extend this project.

## 📄 License

This project is open-source and available under the MIT License.
