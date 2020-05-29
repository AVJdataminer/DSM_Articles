# Which machine learning model should you try first?

[](https://medium.com/@aiden.dataminer?source=post_page-----e35579f15924----------------------)

![Aiden V Johnson](https://miro.medium.com/fit/c/48/48/1*WDVszdcJs5A1fXhnjHZPig.jpeg)

[Aiden V Johnson](https://medium.com/@aiden.dataminer?source=post_page-----e35579f15924----------------------)

[Mar 8](https://medium.com/@aiden.dataminer/which-machine-learning-model-should-you-try-first-e35579f15924?source=post_page-----e35579f15924----------------------)  ·  3  min read

Recently, I received an email from an aspiring data scientist asking a common question in data science.  _How do I know when to use which model?_  The data scientist that sent the question provided more context and had a good approach in mind, but I’d like to answer this question for everyone just starting out in data science.

> How do I know when to use which machine learning model?

This is one of those it depends on everything questions; but here is my approach strongly rooted in the elegance of simplicity.

> _“Make everything as simple as possible but not simpler.” — Albert Einstein_

## **Diagram of the first model selection**

![](https://miro.medium.com/max/30/1*WBaYR8qUT1K53h87PmJppw.png?q=20)

![](https://miro.medium.com/max/3300/1*WBaYR8qUT1K53h87PmJppw.png)

## **Why Random Forest, Logistic, Lasso and Linear Regression?**

Starting with the Multi-Class response variable, Random Forest is well suited to highly correlated features and easy to interpret and understand. In addition, the easy extraction of relative feature importances provides the user a preliminary view of features with strong predictive power for the response variable. Logistic regression is even easier to understand and highly efficient in terms of model run time and provides the simplest approach when model performance is good for the classification in hand. Although multi-class logistic regression is feasible, implementing Random Forest in a multi-class situation is more commonly accepted.

Now, looking at the numeric response side starting with multiple linear regression as the simplest option, however, it is likely to suffer from over-fitting, thus we introduce Lasso regression. Lasso regression through L1-regularization is able to ‘automatically’ complete feature selection for the user by pushing all unimportant feature coefficients to zero. Finally, if the data has many (more than 20) features and some of them are correlated with each other, applying a random forest regression is an easy to understand modeling method usual performing well in non-ideal situations, such as the assumptions for linear regression being unmet.

## Design Your Own Decision Framework

You can design your own decision framework based on the algorithms you prefer and your project constraints following these questions:

1.  Is your response variable numeric or categorical?
2.  How many features are in the data?
3.  Do the features have a high likelihood of collinearity?
4.  What is the importance of interpretability to the model outcome?
5.  What will be the application of the model?

## Be Decisive, not Exhaustive

No matter which model you start with the idea is to balance the constraints of efficiency in implementation, level of understanding required, and overall model performance. It is a best practice to test a couple algorithms and compare their performances, and by a couple I mean two to three with a max of five. You should compare models that leverage different aspects of the features and modeling performance. Don’t compare a decision tree model to a random forest model and expect vastly different results. Hyperparameter tuning is great, but it is also time-consuming and often only yields slight increases in model performance metrics.

## Move on to More Feature Engineering

Feature engineering is more likely to improve model performance than hyperparameter tuning, so consider where your time is best spent and develop more features if your models aren’t performing as you would like.

#### Keywords

-   [Data Science](https://medium.com/tag/data-science)
-   [Machine Learning](https://medium.com/tag/machine-learning)
-   [Python](https://medium.com/tag/python)
-   [Model Selection](https://medium.com/tag/model-selection)
-   [AI](https://medium.com/tag/ai)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNzAzMjc2MzJdfQ==
-->