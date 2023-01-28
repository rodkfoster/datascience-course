# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Linear Regression

> Unit 3: Required

---

## Materials We Provide

| Topic | Description | Link |
| --- | --- | --- |
| Lesson | Linear Regression lesson | [Here](./linear_regression.ipynb) |
| Solution  | Solution code for Lesson Prompts | [Here](./solution-code/linear_regression-solution.ipynb) |
| Slides | Sample slides for this lesson (PPTX) | [Here](./slides/) |
| Practice | Sacramento Regression Review Lab  | [Here](./practice) |
|          | Kobe Shot Regularization (Advanced) | [Here](./practice) |
| Datasets | Capital Bikeshare Rider Data, Kobe NBA data, Sacremento Real Estate Data | [Here](./data/) |


> The lesson data was chosen because it generates approximate linear relationships using real-world data.

NOTE: Kobe lab requires regularization (lasso/ridge) knowledge.

---

## Learning Objectives

After this lesson, students will be able to:
- Define data modeling and how to apply a simple linear regression.
- Build a linear regression model using a dataset that meets the linearity assumption, using the sci-kit learn library.
- Define and identify multicollinearity in a multiple regression.

---

## Student Requirements

Before this lesson(s), students should already be able to:
- Collect data and perform basic data manipulations with Pandas
- Import libraries into Python scripts
- Create simple data visualizations using Python
- Explain basic statistical concepts including linear algebra and descriptive statistics

----

## Lesson Outline

> TOTAL (170 min)
- Introduce the bikeshare dataset (20 min)
  - Read in the Capital Bikeshare data (15 min)
  - Visualizing the data (5 min)
- Linear regression basics (15 min)
  - Form of linear regression
- Overview of supervised learning (25 min)
  - Benefits and drawbacks of scikit-learn (5 min)
  - Requirements for working with data in scikit-learn (5 min)
  - Building a linear regression model in sklearn (5 min)
  - scikit-learn's 4-step modeling pattern (10 min)
- Build a linear regression model (10 min)
- Using the model for prediction (15 min)
  - Does the scale of the features matter?
- Work with multiple features (20 min)
  - Visualizing the data (part 2) (15 min)
  - Adding more features to the model (5 min)
- What is Multicollinearity? (10 min)
- How to select a model (25 min)
  - Feature selection (5 min)
  - Evaluation metrics for regression problems (10 min)
  - Comparing models with train/test split and RMSE (5 min)
  - Comparing testing RMSE with null RMSE (5 min)
- Feature engineering to improve performance (30 min)
  - Handling categorical features (15 min)
  - Feature engineering (15 min)
- Bonus material: Regularization
  - How does regularization work?
  - Lasso and ridge path diagrams
  - Advice for applying regularization
  - Ridge regression
- Comparing linear regression with other models


---

## Additional Resources

#### Safari Resources

+ [Book: Chapter with "Linear Regression" (from "Statistics for Machine Learning")](https://www.safaribooksonline.com/library/view/statistics-for-machine/9781788295758/25ffb48f-78e4-4135-a0d3-a5d3ad08fca2.xhtml)

+ [Book: "In Depth: Linear Regression" (from "Python Data Science Handbook")](https://www.safaribooksonline.com/library/view/python-data-science/9781491912126/ch05.html#in-depth-linear-regression)

+ [Video+Article: O'Reilly Learning Path - "Python for Machine Learning" (1.5 hours)](https://www.safaribooksonline.com/learning-paths/learning-path-python/9781492025443/)

+ [Video+Code: "The pandas-scikit-learn data type divide" (30 mins)](https://www.safaribooksonline.com/oriole/the-pandas-scikit-learn-data-type-divide)

+ [Video+Code: Advanced Topic - "Explain Your Predictive Models to Business Stakeholders with LIME Using Python and H2O" (30 mins)](https://www.safaribooksonline.com/oriole/explain-your-predictive-models-to-business-stakeholders-w-lime-python-h2o)

#### Other Resources
For more information on this topic, check out the following resources:

- [Ben Lorica: Six reasons why I recommend scikit-learn](http://radar.oreilly.com/2013/12/six-reasons-why-i-recommend-scikit-learn.html)
- Scikit-learn examples for [Lasso](http://scikit-learn.org/stable/auto_examples/linear_model/plot_lasso_lars.html) and [Ridge](http://scikit-learn.org/stable/auto_examples/linear_model/plot_ridge_path.html) Regression
- Scikit-learn documentation for [Lasso](http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Lasso.html),  [Ridge](http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html), and [Elastic Net](http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.ElasticNet.html) Regression
- [Analytics Vidhya's Compilation of Linear Regression Blogs](https://www.analyticsvidhya.com/blog/tag/linear-regression/)
- [Data School's "Friendly Introduction to Linear Regression" using Python](http://www.dataschool.io/linear-regression-in-python/)
