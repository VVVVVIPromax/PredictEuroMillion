XGBoost Lottery Prediction Engine
Overview
This project showcases a sophisticated lottery number prediction system powered by a machine learning core. It is designed to analyse historical lottery data and generate predictions for future draws, specifically for formats involving a set of main numbers and a smaller set of bonus numbers (e.g., EuroMillions).

The engine is built to be a self-improving system. It not only predicts outcomes but also incorporates a feedback loop where it learns from actual results to refine its predictive models over time.

Please Note: This public repository contains the user interface and data handling framework for the project. The core predictive algorithms and proprietary model architecture have been intentionally removed to protect intellectual property. The code in this repository is for demonstration purposes and will not perform actual predictions.

Key Features
Machine Learning Core: Utilises a powerful, custom-built machine learning model to drive its predictions.

Continuous Learning: Features an interactive feedback loop. After each draw, the system learns from the actual results to improve its future accuracy.

Automated Data Handling: Seamlessly loads historical data and automatically saves new results, continuously expanding its knowledge base.

Efficient Architecture: Designed for efficient model training and data processing.

User-Friendly Interface: A simple command-line interface allows for easy operation, from generating predictions to inputting new results.

High-Level Workflow
The operational flow of the complete system is as follows:

Load Data: The engine starts by loading all available historical draw data from a local CSV file.

Train Models: It then processes this data to train its proprietary ensemble of predictive models. This is an intensive process where the system learns the underlying patterns from the historical results.

Generate Prediction: Once trained, the engine generates a set of predicted numbers for the next draw.

Feedback & Update: After the official draw, the user is prompted to input the actual winning numbers. The system calculates its accuracy and, most importantly, appends these new results to the historical data file.

Save: The newly updated dataset is saved, ensuring the system is more knowledgeable for the next cycle.

How to Use (Demonstration)
Dependencies: Ensure you have Python 3 and the required libraries installed.

pip install numpy pandas scikit-learn xgboost joblib

Historical Data: You will need a CSV file containing historical lottery results (e.g., EuroHistory.csv).

Run the Script: Execute the main Python script from your terminal.

python your_script_name.py

Follow Prompts: The demonstration script will simulate the training and prediction steps. It will then prompt you to enter the "actual" results to showcase the feedback loop and data-saving functionality.
