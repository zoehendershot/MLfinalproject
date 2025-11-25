# Q: How do biological information and lifestyle choices impact a person's obesity level?

### Methodology: Classification Decision Tree with 4 levels: Insufficient Weight, Normal Weight, Overweight, Obese
- cleaned and preprocessed the Obesity dataset
- collapsed labels into 4 target classes
- encoded categorical features
- implemented a baseline Decision Tree pipeline
- performed hyperparameter tuning (grid search over max_depth)
- stratified 80/10/10 train/tune/test splits
- generated evaluation reports, confusion matrices, and feature importances

### Tools: Python, pandas, scikit-learn, matplotlib, Graphviz.

**Background**

_https://www.cdc.gov/obesity/risk-factors/risk-factors.html_

The CDC cites physical activity, eating patterns, sleep quality and quantity, and electronic use as risk factors for obesity.
Our dataset, which we found in the class data folder, contains many of these risk factors as features. Our goal is to explore 
a decision tree classifier for obesity level to see how well these lifestyle choices, as well as some biological traits, impact obesity level. 
We also explore how much each risk factor contributes to obesity. 

This exploration has potential application in the field of public health; it would be most beneficial to pour resources into prevention through the most important risk factors. 

--------------------------------------------
- Results summary: produced an interpretable Decision Tree baseline and identified the top predictive features via feature importance. Full evaluation metrics (precision, F1, balanced accuracy) are recorded in `basemodel.ipynb` under the Tune/Test evaluation cells.
- Impact: the analysis surfaces the most influential risk factors for obesity in this dataset and provides a reproducible workflow for experimenting with stronger models and handling class imbalance.
