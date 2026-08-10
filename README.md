
# SMS Spam Detection Using Machine Learning

## Project Overview

This project develops a machine learning system for automatically classifying SMS messages as either **spam** or **ham (legitimate)**.

The project was developed as part of an Artificial Intelligence (Machine Learning) group assignment. The SMS dataset was obtained from Kaggle and processed using Python and Scikit-learn.

## Dataset

The dataset contains SMS messages labelled as either:

* **Ham (0):** Legitimate SMS messages
* **Spam (1):** Unwanted or potentially fraudulent SMS messages

The original dataset contained 5,572 records and 5 columns. After removing unnecessary columns and 414 duplicate records, the final dataset contained **5,169 unique SMS messages**.

The final class distribution was:

* Ham: 4,516
* Spam: 653

## Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Scikit-learn
* Pickle
* CountVectorizer
* Multinomial Naive Bayes

## Methodology

The project followed these main steps:

1. Dataset collection
2. Data exploration
3. Data cleaning
4. Removal of duplicate records
5. Label encoding
6. Text feature extraction using CountVectorizer
7. Train-test splitting
8. Model training using Multinomial Naive Bayes
9. Model evaluation
10. Testing with new SMS messages
11. Saving the trained model using Pickle

## Model Performance

The trained model achieved:

| Metric         | Result |
| -------------- | -----: |
| Accuracy       | 98.26% |
| Spam Precision |   0.94 |
| Spam Recall    |   0.94 |
| Spam F1-Score  |   0.94 |

### Confusion Matrix

```text
[[880   9]
 [  9 136]]
```

The model correctly classified 880 ham messages and 136 spam messages in the test set.

## Project Files

* `SMS_Spam_Detection.ipynb` — Main Jupyter Notebook containing the complete implementation.
* `spam_model.pkl` — Saved trained Multinomial Naive Bayes model.
* `vectorizer.pkl` — Saved CountVectorizer used to transform SMS messages into numerical features.
* `README.md` — Project documentation.

## Group Members

AUGUSTUS APPIAH - UEB3519923
MUMUNI RAZACK ANONABALA- UEB3506823
ISHMEAL NARTEH - UEB3509223

## Future Improvements

Future work may include comparing additional machine learning algorithms, applying TF-IDF feature extraction, using advanced natural language processing techniques, and deploying the model as a web or mobile application.

## License

This project was developed for academic purposes.
