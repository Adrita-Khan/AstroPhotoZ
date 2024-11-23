**Metrics**

Here’s how each metric aligns with standard practices for evaluating machine learning models:

1. **MSE (Mean Squared Error)**: A standard loss function commonly used to evaluate prediction accuracy. It measures the average squared difference between predicted and actual values.

   $$\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$$

2. **MAE (Mean Absolute Error)**: Complementary to MSE, this metric measures the average absolute difference between predicted and actual values. It is less sensitive to outliers compared to MSE.

   $$\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} \left| y_i - \hat{y}_i \right|$$

3. **\( R^2 \) (Coefficient of Determination)**: Assesses how well the model explains the variance in the data. It is a critical metric for evaluating the goodness of fit.

   $$R^2 = 1 - \frac{\sum_{i=1}^{n} (y_i - \hat{y}_i )^2}{\sum_{i=1}^{n} (y_i - \bar{y})^2}$$

4. **Bias**: Reflects systematic errors in predictions. A lower bias indicates the model makes consistent predictions without systematic shifts.

   $$\text{Bias} = \frac{1}{n} \sum_{i=1}^{n} (\hat{y}_i - y_i)$$

5. **Precision**: In regression tasks, precision often refers to the variability in repeated predictions or the model's ability to tightly group results around the true values.

   $$\text{Precision} = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (\hat{y}_i - \bar{\hat{y}})^2}$$

6. **Catastrophic Outlier Fraction**: Measures the proportion of predictions that significantly deviate from the true values. This metric is especially important in astrophysics, where outliers can mislead scientific interpretations.

   $$\text{Catastrophic Outlier Fraction} = \frac{\text{Number of Outliers}}{n}$$

   *An outlier is typically defined as a prediction where the absolute difference between the predicted and true value exceeds a specified threshold.*
