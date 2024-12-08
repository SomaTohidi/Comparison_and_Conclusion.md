# Automobile Dataset Classification Project

## Comparison of Model Results

| Metric                  | Logistic Regression | MLP (Neural Network) | Best Random Forest |
|-------------------------|---------------------|----------------------|--------------------|
| **Accuracy**            | 49%                | 71%                 | 76%               |
| **Macro Avg F1-Score**  | 0.43               | 0.59                | 0.63              |
| **Weighted Avg F1-Score** | 0.47              | 0.70                | 0.74              |

### Observations:
1. **Logistic Regression**:
   - Baseline model with poor performance on all metrics.
   - Struggled with minority classes due to its linear nature.

2. **MLP (Neural Network)**:
   - Significant improvement in accuracy and F1-scores compared to Logistic Regression.
   - Captures non-linear relationships better but still struggles with minority classes.

3. **Best Random Forest**:
   - The best-performing model with the highest accuracy (76%) and balanced F1-scores.
   - Handles non-linearity and imbalanced data better than other models.

### Conclusion:
- Random Forest provides the most robust performance and sets the benchmark for this dataset.
- Further improvements can be achieved by addressing class imbalance and exploring advanced ensemble methods.

---

## Summary and Conclusion

### Key Findings:
1. **Preprocessing**:
   - Missing values were effectively managed using mean, median, and mode.
   - Outliers in features like `Horsepower` and `Price` were analyzed but not removed.

2. **Model Evaluation**:
   - Random Forest outperformed Logistic Regression and MLP in terms of accuracy and F1-scores.
   - Minority classes (e.g., Class 0) remain challenging due to data imbalance.

### Limitations:
1. **Data Imbalance**:
   - Classes with very few samples (e.g., Class 0) negatively impacted performance.
2. **Feature Engineering**:
   - Limited feature transformations were applied, which might have restricted model performance.

### Recommendations:
1. **Address Data Imbalance**:
   - Use SMOTE or similar techniques to generate synthetic samples for minority classes.
2. **Explore Advanced Models**:
   - Gradient Boosting or XGBoost could further enhance performance.
3. **Feature Engineering**:
   - Apply advanced transformations like PCA or feature selection to improve model performance.
