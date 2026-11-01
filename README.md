🌧️ Rainfall Prediction System Using Data Mining
📌 Project Overview
This project applies data mining techniques to predict the likelihood of rainfall on the following day based on daily meteorological measurements. Accurate weather prediction is crucial for agriculture, transportation, and water resource management. Four classification algorithms were implemented and compared to find the most accurate predictive model.
🎯 Problem Statement
Atmospheric factors are highly variable, making manual forecasting difficult. This project leverages data mining to extract non-obvious patterns from complex weather data.
🛠️ Technologies & Libraries
Language: Python
Data Manipulation: Pandas, NumPy
Machine Learning: Scikit-learn (Decision Tree, SVM, Naive Bayes, Random Forest)
Data Visualization: Matplotlib, Seaborn
Environment: Jupyter Notebook / Google Colab
📊 Dataset Description
A synthetic dataset was generated to simulate real-world weather data:
Total Records: 1,000
Features: 15 meteorological features (e.g., MinTemp, MaxTemp, Rainfall, Evaporation, Humidity, Pressure).
Target Variable: RainTomorrow (Created using logic: if Humidity3pm > 60 OR Rainfall > 5, it is classified as rain).
Preprocessing: Missing values were imputed using the mean, and features were standardized using StandardScaler to ensure optimal performance for algorithms like SVM.
⚙️ Methodology & Models
The data was split into 70% training and 30% testing. Four models were trained and evaluated:
Decision Tree: Used for clear and interpretable rules (max_depth=5).
Support Vector Machines (SVM): Effective in high-dimensional spaces (kernel='rbf').
Naive Bayes: A fast, probabilistic baseline model.
Random Forest: An ensemble model used to reduce variance and improve accuracy (n_estimators=100).
🏆 Results & Discussion
The Random Forest model demonstrated the best performance, achieving an accuracy of ~99%. This indicates a strong relationship between the selected meteorological factors (especially humidity and pressure) and rainfall prediction.
Model Accuracy F1-Score
Random Forest 0.9933 0.9895
Decision Tree 0.9867 0.9789
Naive Bayes 0.9133 0.8571
SVM 0.9000 0.8295
🚀 How to Run
Clone the repository.
Install the required libraries: pip install pandas numpy scikit-learn matplotlib seaborn
Run the Jupyter Notebook file to see the data generation, preprocessing, model training, and visualizations.
👤 Author
Shahad Abu Jabl
GitHub: @shahadabujabl
📄 Project Report: Click here to view the full report
https://github.com/shahadabujabl/Rainfall-Prediction-System/blob/main/Project_Report.pdf
