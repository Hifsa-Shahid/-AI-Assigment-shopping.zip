# 🛒 Shopping Revenue Prediction using KNN

##  Assignment Overview

This project is part of a Artificial Intelligence assignment that predicts whether an online shopping session will result in **revenue (purchase)** or **no revenue** using a **K-Nearest Neighbors (KNN)** classifier. The model is trained and evaluated using a **CSV shopping dataset** containing user behavior data.

---

##  Objective

To build a classification model that:

* Learns from historical online shopping behavior
* Predicts whether a user will make a purchase
* Evaluates performance using sensitivity and specificity

---

##  Dataset Description

The dataset is provided in **CSV format**, where each row represents a user session on an e-commerce website.

### Input Features

* Administrative pages visited and duration
* Informational pages visited and duration
* Product-related pages visited and duration
* Bounce rates and exit rates
* Page values and special day indicator
* Operating system, browser, region, traffic type
* Visitor type (Returning or New)
* Weekend (True/False)

###  Target Variable (Label)

* **Revenue**

  - `1` → Purchase made
  - `0` → No purchase

---

##  Data Preprocessing

* Categorical values are converted to numerical values
* Boolean fields are encoded as binary values (0 or 1)

This step is necessary because AI models require numerical input.

---

##  Artificial Intelligence Model

* **Algorithm:** K-Nearest Neighbors (KNN)
* **K value:** 1
* The model predicts the class of a test instance based on its closest training neighbor.

---

##  Train–Test Split

* **60%** of the data is used for training
* **40%** of the data is used for testing

This ensures that the model is evaluated on unseen data.

---

##  Evaluation Metrics

The model is evaluated using:

###  Sensitivity (True Positive Rate)

Measures how well the model identifies users who actually make purchases.

###  Specificity (True Negative Rate)

Measures how well the model identifies users who do not make purchases.

---

##  Results

```
Correct Predictions: 4063
Incorrect Predictions: 869
True Positive Rate (Sensitivity): 38.01%
True Negative Rate (Specificity): 90.50%
```

###  Interpretation

* The model performs well in identifying **non-buyers**
* Performance is weaker in detecting **buyers** due to data imbalance and low K value

---

## Conclusion

This assignment demonstrates the application of a KNN classifier on real-world e-commerce data. While the model achieves high specificity, improvements such as tuning the value of K or using other classifiers could enhance sensitivity and overall performance.



on script.

---

## Technologies Used

* Python
* scikit-learn
* CSV module

---

##  Author

**Hifsa Shahid**
Artificial Intelligence Assignment

