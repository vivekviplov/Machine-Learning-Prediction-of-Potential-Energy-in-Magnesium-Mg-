
🚀 Machine Learning Prediction of Potential Energy in Magnesium (Mg)
This repository contains the code and resources for the research study on applying machine learning techniques to accurately predict the potential energy of Magnesium (Mg). Accurate prediction of potential energy is crucial for understanding magnesium's structural stability and mechanical behavior in diverse industrial applications.

🌟 OverviewMagnesium is a lightweight, abundant metal widely used in aerospace, automotive, and consumer electronics sectors due to its exceptional properties like low density ($1.74~g/cm^{3}$), high damping capacity, and good thermal conductivity.
Traditional methods for characterizing material properties are often computationally intensive and time-consuming. This work integrates Machine Learning (ML) with data generated from Molecular Dynamics (MD) simulations (both ab initio and classical) to create efficient, predictive models for magnesium's potential energy.

💡 Key Findings
The study evaluated several regression models, and the Random Forest model emerged as the superior predictor.
Top-Performing Model: Random Forest Regression
.Performance Metrics (Test Data):Root Mean Squared Error (RMSE): $16.08$
.Coefficient of Determination ($R^{2}$ Score): $0.9999$
This high accuracy demonstrates the potential of ML to accelerate materials design and reduce dependence on costly atomistic simulations.

🛠️ Methodology and Pipeline
The machine learning pipeline involves several critical stages:


Data Collection: A foundational dataset was generated from Molecular Dynamics (MD) simulations (e.g., using LAMMPS) capturing physical states under diverse thermodynamic conditions.



Data Preprocessing and Augmentation: Rigorous quality control, outlier detection, and standardization/normalization were applied. Data augmentation included adding controlled statistical noise and synthetic data generation to enhance model generalization.





Feature Engineering and Selection: Primary features (e.g., Temperature, Pressure, Kinetic Energy, Volume) were used, along with derived features (rate of change, ratios) to capture dynamic behavior. Correlation analysis guided the selection of influential features.






Model Training and Evaluation: Four models were benchmarked: Linear Regression, Ridge Regression, Decision Tree, and Random Forest. Training incorporated k-fold cross-validation and stratified sampling.





Hyperparameter Tuning: A systematic grid search with cross-validation was used to optimize parameters (e.g., regularization strength, max tree depth) to maximize accuracy and minimize overfitting.
