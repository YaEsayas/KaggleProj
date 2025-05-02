# KaggleProj

Student Performance Classification
Problem Description
This project uses a dataset about students to predict how well they are doing in school: High (H), Middle (M), or Low (L).
We use machine learning to guess a student's performance level based on their behavior (like raising hands or doing discussions) and some background info.
 Dataset Summary
●	Total students: 480
●	Features (columns): 16 inputs + 1 target (Class)
●	Target values:
○	H = High performance
○	M = Middle
○	L = Low
●	How common each class is:
○	M: 211
○	H: 142
○	L: 127
●	Missing values: None 
●	Outliers: Some extreme values, but they look real, so we kept them
 What We Learned from the Data
●Students who raised their hands and visited resources a lot were usually in the high class.
●	Categorical things like gender or stage level also showed some difference between classes.
●	We made bar charts and histograms to see the patterns clearly.
 Cleaning and Getting Data Ready
●	We turned text columns (like gender) into numbers using one-hot encoding.
●	We turned the target (Class) into numbers:
○	H = 0, L = 1, M = 2
●	We scaled the number features so they all had the same range.
●	Now everything is numbers and ready for training a model.

 Machine Learning Steps
Model:
●	We used a Random Forest (a smart model that uses many decision trees).
Data Split:
●	60% used to train the model
●	20% to check how well it works (validation)
●	20% saved for future testing
Results:
●	Accuracy: About 85%
●	The model made good predictions for most students

 What We Found Out
●	Most useful features: raisedhands, VisITedResources, and Discussion
●	No need to fix class imbalance — it wasn't a big issue
●	The model could tell the difference between low, middle, and high-performing students pretty well
⚙ How to Use This
1.	Load the dataset: xAPI-Edu-Data.csv
2.	Open the notebook and run each cell
3.	You only need basic Python tools:
○	pandas, matplotlib, seaborn
○	scikit-learn

 How to Make It Better
●	Try tuning the model to improve accuracy
●	Test other models like logistic regression
●	Try turning this into a yes/no prediction: High vs Not High

 Thanks
Dataset from: xAPI-Edu-Data on Kaggle


