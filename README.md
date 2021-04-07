# Basic-Understanding-of-SHAPASH-With-The-Aid-of-an-Use-case
Establishing an expectation for trust around AI technologies may soon become one of the most important skills provided by Data Scientists. Significant research investments are underway in this area, and new tools are being developed, such as Shapash, an open-source Python library that helps Data Scientists make machine learning models more transparent and understandable.

[Shapash](https://github.com/MAIF/shapash) by [MAIF](https://www.maif.fr/) is a Python Toolkit that facilitates the understanding of Machine Learning models to data scientists. It makes it easier to share and discuss the model interpretability with non-data specialists: business analysts, managers, and end-users.

Concretely, Shapash provides easy-to-read visualizations and a [web app](https://shapash-demo.ossbymaif.fr/). Shapash displays results with appropriate wording (preprocessing inverse/post-processing). Shapash is useful in an operational context as it enables data scientists to use explicability from exploration to production: You can easily deploy local explainability in production to complete each of your forecasts/recommendations with a summary of the local explainability.

### Elements of context
Interpretability and explicability of models are hot topics. There are many articles, publications, and open-source contributions about it. All these contributions do not deal with the same issues and challenges. Most data scientists use these techniques for many reasons: to better understand their models, to check that they are consistent and unbiased, as well as for debugging. 

However, there is more to it: "Intelligibility matters for pedagogic purposes. Intelligible Machine Learning models can be debated with people that are not data specialists: business analysts, final users"

Concretely, there are two steps in our Data Science projects that involve non-specialists:
1. Exploratory step & Model fitting
2. Deploying the model in a production environment

### Exploratory step & Model fitting
At this step, data scientists and business analysts discuss what is at stake and define the essential data they will integrate into the projects. It requires understanding the subject well and the main drivers of the problem we are modeling. To do this, data scientists study global explicability, features importance, and which role the model’s top features play. They can also locally look at some individuals, especially outliers. A Web App is interesting at this phase because they need to look at visualizations and graphics. Discussing these results with business analysts is interesting to challenge the approach and validate the model.

### Deploying the model in a production environment
That’s it! The model is validated, deployed, and gives predictions to the end-users. Local explicability can bring them a lot of value, only if there is a way to provide them with a good, useful, and understandable summary. It will be valuable to them for two reasons:
- Transparency brings trust: They will trust models if they understands them.
- Human stays in control: No model is 100% reliable. When they can understand the algorithm’s outputs, users can overturn the algorithm suggestions if they think they rest on incorrect data.


### Shapash key features
1. Easy-to-read visualizations, for everyone.
2. A web app: To understand how a model works, you have to look at multiple graphs, features importance, and global contribution of a feature to a model. A web app is a useful tool for this.
3. Several methods to show results with appropriate wording (preprocessing inverse, post-processing). You can easily add your data dictionaries, category-encodersobject, or sklearn ColumnTransformer for more explicit outputs.
4. Functions to easily save Picklefiles and to export results in tables.
5. Explainability summary: the summary is configurable to fit with your need and to focus on what matters for local explicability.
6. Ability to easily deploy in a production environment and to complete every prediction/recommendation with a local explicability summary for each operational apps (Batch or API)
7. Shapashis open to several ways of proceeding: It can be used to easily access results or to work on better wording. Very few arguments are required to display results. But the more you work with cleaning and documenting the dataset, the clearer the results will be for the end-user.


Shapash works for Regression, Binary Classification, or Multiclass problems. It is compatible with many models: Catboost, Xgboost, LightGBM, Sklearn Ensemble, Linear models, SVM.

Shapash is based on local contributions calculated with Shap (shapley values), Lime, or any technique which allows computing summable local contributions.
