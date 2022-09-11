# Fraud-Detection-in-Credit-Card-Transactions

# Case and Data Description
This project aimed to build an effective and efficient model to predict transaction fraud. The analyzed dataset contains a list of government-related credit card transactions over the 2010 calendar year. The data presented a supervised problem containing the fraud label and attributes such as credit card number, merchant, merchant state, etc. The dataset had 96,753 records and 10 data fields. There were nine categorical variables and one numeric variable. EDA revealed that the dataset is imbalanced as many of the variables had a right-skewed distribution. Overall, the dataset had 1,059 fraudulent transactions of the total 96,753 records (1.09%). This project focused on the ‘purchase’ transactions.

# Approach
Step 1: Exploratory data analysis and Data Cleaning: /n
Exploratory data analysis was conducted to describe and visualize each of the 10 data fields. The data cleaning involved removing outliers upon knowledge group approval and addressing missing values by carefully crafted data imputation techniques.

Step 2: Feature Engineering:
There were six different types of variables: amount variables, frequency variables, days-since variables, velocity change variables on eight time periods were created along with two Benford’s Law variables, and a day-of-the-week risk table variable. Target encoding and statistical smoothing was conducted on Day-of-week variable and Merchant state variables.

Step 3: Feature Selection:
The data was divided into three sections for model development and analysis: training, testing, and out-of-time (OOT). Feature selection involved filtering based on Kolmogorov-Smirnov(KS) score and using the wrapper method. Top 20 best variables with each having a wrapper score above 0.6

Step 4: Model Selection:
Having a logistic regression model as a baseline, several non-linear models with varying hyper parameters were explored. These non-linear models included Decision Tree, Random Forest, Gradient Boosting, and Neural Network. Gradient Boosting Tree delivered the best training, testing, and OOT data results.
