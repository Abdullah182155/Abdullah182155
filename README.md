NLP Portfolio App is a Streamlit application for analyzing stock performance through NLP-driven strategies. The app processes historical stock data, applies machine learning models to predict trends, and provides portfolio optimization strategies based on predicted stock returns. The app supports multiple investment strategies, including return-based, risk-adjusted, expected return, and positive news impact.

Table of Contents
Features
Installation
Usage
Folder Structure
Available Strategies
Contributing
License
Features
NLP-Driven Predictions: Uses pre-trained models to predict stock performance based on textual data.
Portfolio Optimization: Supports various investment strategies, including return-based, risk-adjusted, expected return, and positive news impact.
Interactive Visualizations: Displays portfolio metrics like model return, invested cash, and accuracy over time.
Dynamic Rolling Windows: Divides data into time-based windows for better analysis and visualization.
Installation
Clone the repository:

bash
نسخ الكود
git clone https://github.com/yourusername/nlp-portfolio-app.git
cd nlp-portfolio-app
Install dependencies:

bash
نسخ الكود
pip install -r requirements.txt
Set up folders: Ensure the following folders are created in the project root:

Processed_Datasets/: Folder for processed stock data files.
best_models/: Folder containing pre-trained model files (.pkl format).
Stocks Updates/: Folder for storing updated stock price information.
Usage
Run the application with the following command:

bash
نسخ الكود
streamlit run app.py
Steps:
Input Data Folder: Specify the folder containing processed datasets.
Select Model Folder: Specify the folder containing pre-trained models.
Set Date Range: Choose the start and end dates for your analysis.
Choose Stocks: Select stocks for analysis based on available models.
Select Strategies: Choose one or more strategies for portfolio optimization.
Input Initial Cash: Set the initial cash investment amount.
Run Predictions: Click "Run Predictions" to start processing.
The app will display a stock price table, portfolio results for each strategy, and dynamic plots showing model return, invested cash, and accuracy over time.

Folder Structure
This project uses the following folder structure:

Processed_Datasets/: Stores CSV files containing processed stock data.
best_models/: Contains the pre-trained models for each stock.
Stock Window/: Saves stock prediction results for each stock.
rolling_windows/: Stores rolling window data for each time interval.
Portfolio/: Stores results and weights generated by each strategy.
Available Strategies
The app supports the following investment strategies:

Return-Based: Allocates portfolio weights based on stock returns.
Risk-Adjusted: Weights are adjusted based on risk assessments.
Expected Return: Uses expected returns to calculate portfolio weights.
Positive News: Weights are adjusted based on positive sentiment analysis.
Contributing
Fork the project and clone the repository locally.
Create a branch for each feature or bug fix: git checkout -b feature-name.
Commit your changes: git commit -m 'Add feature'.
Push to your branch: git push origin feature-name.
Open a Pull Request with a clear description of the changes.
Contributions are welcome! Please follow the code of conduct and check issues for ways to get involved.

License
This project is licensed under the MIT License. See the LICENSE file for details.
