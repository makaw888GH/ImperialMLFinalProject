# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

**Input:** Describe the inputs of your model
* 21 features and 1 label were used as input for model training and testing

**Output:** Describe the output(s) of your model
* The primary output of the model is the probability of credit card payment default
* Other output of the model as part of the exploratory data analysis includes: Information Value, Population Stability Index (Data Drift analysis), Weight of Evidence, and Feature Importance

**Model Architecture:** Describe the model architecture you’ve used
* Logistic Regression Model architecture

## Performance

Optimisation output and AUC graph shows each of the hyperparameters selected, optimal value and resulting model performance

![alt_text](https://github.com/makaw888GH/ImperialMLFinalProject/blob/main/PostTuningResults.png?raw=true)

Feature Inportance to provide model explainability

![alt_text](https://github.com/makaw888GH/ImperialMLFinalProject/blob/main/featureImportance.png?raw=true)

## Limitations

### Multicollinearity:
* Logistic regression requires moderate or no multicollinearity between independent variables. High correlation between predictors can lead to unstable model estimates. This issue has been mitigated by removing features which exceed correlation threshold
### Outperformed by More Complex Algorithms:
* While logistic regression is useful for simple datasets, more powerful algorithms like neural networks can often outperform it.
### Regularization for Overfitting:
In high-dimensional datasets, logistic regression may overfit. Regularization techniques (such as L1 or L2 regularization) can help mitigate this issue.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
