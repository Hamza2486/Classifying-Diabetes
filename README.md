# Diabetes Classification Using Classical Methods

## Dataset Overview
The dataset, **diabetes.csv**, contains information from over 250,000 individuals sourced by the CDC. Each row corresponds to an individual's health and demographic details, with the following columns:

1) **Diabetes status**: `1` = diagnosed with diabetes, `0` = not diagnosed
2) **High blood pressure**: `1` = diagnosed with hypertension, `0` = not diagnosed
3) **High cholesterol**: `1` = diagnosed with high cholesterol, `0` = not diagnosed
4) **Body Mass Index (BMI)**: Calculated as weight divided by height squared
5) **Smoker**: `1` = has smoked over 100 cigarettes in their lifetime, `0` = has not
6) **Stroke**: `1` = has previously suffered a stroke, `0` = has not
7) **Myocardial issues**: `1` = has previously had a heart attack, `0` = has not
... and so forth up to:
22) **Zodiac sign**: `1` = Aries, `12` = Pisces, etc.

## Project Objectives and Methods
The primary objective of the analysis is to build a classification model to separate diabetics from non-diabetics. Further, from each analysis, the best predictor for diabetes is identified. The methods used are as follows:

### Implemented Models:
1. **Logistic Regression**: 
    
2. **Support Vector Machine (SVM)**:
    
3. **Decision Tree**:
    
4. **Random Forest**:
    
5. **AdaBoost**:

## Metrics
The following metrics were used to evaluate the models:
1. **Area Under the ROC Curve (AUC)**
3. **Training vs Testing Accuracy**
4. **Matthews Correlation Coefficient (MCC)**
- The classes in the dataset were imbalanced; therefore, the MCC was used since it takes into account true and false positives and negatives and is generally regarded as a balanced measure which can be used even if the classes are of very different sizes.
- **Formula:**
     $`\text{MCC} = \frac{(TP \times TN - FP \times FN)}{\sqrt{(TP + FP) \times (TP + FN) \times (TN + FP) \times (TN + FN)}}`$
     Where TP = True Positives, TN = True Negatives, FP = False Positives, FN = False Negatives.
6. **Precision**
- **Formula:** 
     $`\text{Precision} = \frac{TP}{TP + FP}`$
7. **Recall**
- **Formula:**
     $`\text{Recall} = \frac{TP}{TP + FN}`$

