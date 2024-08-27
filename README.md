# Customer Churn Prediction for Subscription

## Author : Uddipan Bhattacharjee


### Introduction to the Challenge

In this case study, we'll be working with a fintech company aiming to offer its customers a paid mobile app subscription that consolidates all their financial information in one place. To attract users, the company provides a free version of the app, with some core features unlocked.

The task is to identify users who are unlikely to subscribe to the paid version, so the company can target them with additional offers. Due to the costs associated with these offers, the company prefers not to extend them to all users—especially those who are likely to subscribe without any incentives.

**Market:** The target audience consists of customers using the company's free product—in this case, users who have installed and engaged with the company's free mobile app.

**Product:** The paid subscription includes enhanced versions of the features available in the free version, along with new functionalities.

**Goal:** The objective is to build a predictive model to identify which users are unlikely to subscribe to the paid membership. This will allow the company to focus its marketing efforts on converting these users into paid subscribers.

### Dataset

As part of the company, you have access to data on each customer's app behavior. This dataset includes the date and time of app installation, as well as details on the features the users engaged with within the app. App behavior is captured through the screens users viewed and whether they played the available financial mini-games.

The dataset only covers the user's first day in the app because the company offers a 24-hour free trial of premium features and wants to target users with new offers immediately after the trial ends.

The dataset is stored in a file named "appdata10.csv". Additionally, the company has provided a list of the most frequently used app screens in the "top_screens.csv" file to help reduce the number of features.

### Files

- **"fintech.py"** and **"fintech.ipynb"**: Python script and Jupyter Notebook files, respectively.

### Tasks Performed

1. Statistical analysis of numerical variables with the dependent variable and correlation matrix.
2. Data cleaning and analysis based on the difference between `first_open` and `enrolled_time`.
3. Feature extraction from the "screen_list" field into several new fields listed in "top_screens".
4. Training a Logistic Regression model with hyperparameter tuning.
5. Training an XGBoost model and comparing performance based on classification metrics such as confusion matrix, accuracy, precision, recall, and F1 score.
