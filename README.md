
# Sentiment Analysis - Final Project

Author

Nandini Maddula 
 
LLM Final Assessment

About This Project

This project analyzes employee emails to understand their overall sentiment and engagement. I used Python to label each message as positive or negative, calculated monthly sentiment scores, ranked employees, identified potential flight risks, and built a simple model to predict sentiment trends.

Files Included

- 'test.csv'– Original dataset of employee messages  
- 'SentimentAnalysis.ipynb' – Jupyter notebook with all the analysis and results  
- 'visualizations' – Folder containing graphs and plots  
- 'README.md' – This file  

 How to Run It

1. Open the project folder.
2. Launch Jupyter Notebook.
3. Open the 'SentimentAnalysis.ipynb' file.
4. Run the cells in order.
5. Make sure these Python libraries are installed:
   pandas, numpy, matplotlib, seaborn, transformers, torch, scikit-learn
 ->You can install them using:
   pip install pandas numpy matplotlib seaborn transformers torch scikit-learn

What I Did

1. Sentiment Labeling
I used a pre-trained NLP model to tag each message as either "Positive" or "Negative".
2. EDA 
I looked at how messages are distributed across sentiment types and created a few graphs.
3. Monthly Sentiment Scoring
Each message was given a score (+1 for positive, -1 for negative). Then I calculated the total score for each employee every month.
4. Employee Ranking
I listed the top 3 most positive and top 3 most negative employees for each month, based on their sentiment scores.
5. Flight Risk
If an employee sent 4 or more negative messages within any 30-day period, they were flagged as a flight risk.
6. Predictive Model
I trained a basic linear regression model to predict sentiment scores based on features like message length and word count.

Summary:

- Top Positive and Negative Employees: Identified monthly
- Flight Risk Employees: Employees who may be disengaged or unhappy
- Model Performance:
  - MSE (error): 7.73  
  - R² score: -0.00 (low, but included as required)

Notes:

This was a solo project done for internal evaluation purposes. The default model from Hugging Face was used for sentiment labeling. Charts and visualizations are saved in the visualizations folder.
