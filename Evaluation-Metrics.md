## Metrics

Each metric aligns with standard practices for evaluating machine learning models, providing a comprehensive analysis of performance:

1. **MSE (Mean Squared Error)**  
   Measures the average squared difference between predicted and actual values. A standard loss function to evaluate prediction accuracy.

2. **MAE (Mean Absolute Error)**  
   Calculates the average absolute difference between predicted and actual values. Less sensitive to outliers compared to MSE.

3. **\( R^2 \) (Coefficient of Determination)**  
   Evaluates how well the model explains the variance in the data. A critical metric for assessing the goodness of fit.

4. **Bias**  
   Indicates systematic errors in predictions. A lower bias suggests the model makes consistent predictions without significant systematic shifts.

5. **Precision**  
   In regression tasks, this refers to the model's ability to tightly group predictions around the true values, indicating low variability in repeated predictions.

6. **Catastrophic Outlier Fraction**  
   Represents the proportion of predictions that deviate significantly from the true values. Especially important in domains like astrophysics, where outliers can skew scientific interpretations.
