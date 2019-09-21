In this exercise, I build a regression model in Jupyter Notebook to predict box office revenues using data on movies from The Movie Database.

I use Scikit-Learn Pipelines to clean the data and quickly evaluate 8 regression models. I use a Random Forest for my final model. For feature selection, I use a variable selection procedure based on [this paper](https://www.csie.ntu.edu.tw/~b88052/tmp/vietri.pdf) by the Biometrics Research Department at Merck & Co which improved both model error and interpretability, and reduced model features by more than 66%.

The primary goal of this project was to practice processing data using custom transformers and Scikit-Learn Pipelines. I spent longer than I intended on this, but learned a lot about feature selection as well. If I were to return to this project to improve model performance, I'd focus further on external data, feature engineering, and feature selection.

## How to run this project

1. Download `Regression Model.ipynb`. Then download the data for the project from [here](https://www.kaggle.com/c/tmdb-box-office-prediction/data). 
2. Place it in the same directory as the Jupyter Notebook
3. In the notebook, change the file path in `pd.read_csv()` your preferred data name
4. You should be able to work through the entire notebook
5. If you run into issues or have questions, log an issue and I'll get back to you ASAP

## Learning goals

* [x] Practice Python ML workflow
* [x] Learn to build data processing pipelines in Sklearn

## Things learned

* Outlier analysis
* Data cleaning (for exploration) vs. data preprocessing (for modeling)
* Building transformers and Pipelines with Scikit-Learn
* Feature selection using Random Forests
* Apply with anonymous function
* List comprehensions
* Conditional expressions

## Things to improve on in future projects

* Allocate more time upfront to exploration
* Analyze outliers with scatterplots, decide to remove or not
* Separate the data cleaning step (exploration) from data processing step (modeling)
* Use `sklearn.feature_selection` module to speed up feature selection process

## References

* [Forecasting Movie Box Office Profitability](https://pdfs.semanticscholar.org/6d4f/1003fd164ffe30e2e45dd252715efecf9e61.pdf)
* [ML Data Pipelines with Customs Transformers in Python](https://towardsdatascience.com/custom-transformers-and-ml-data-pipelines-with-python-20ea2a7adb65)
* [Andrew Lukyanenko's Kaggle kernel](https://www.kaggle.com/artgor/eda-feature-engineering-and-model-interpretation)
* [Scikit-Learn Documentation](https://scikit-learn.org/stable/tutorial/statistical_inference/putting_together.html)
* [Feature selection or model tuning: which goes first?](https://stats.stackexchange.com/questions/264533/how-should-feature-selection-and-hyperparameter-optimization-be-ordered-in-the-m)