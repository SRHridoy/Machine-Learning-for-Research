# 📒 Data Science & Machine Learning Notebook Collection (English + বাংলা)

> For my own learning, in my own words, in my own way! | নিজের শেখার জন্য, নিজের ভাষায়, নিজের মতো করে!

---

## 📖 Table of Contents | সূচিপত্র

-   Quick Start | দ্রুত শুরু
-   How to Use | কিভাবে ব্যবহার করবেন
-   Expanded Notes by Folder | ফোল্ডারভিত্তিক বিস্তারিত নোট
-   Learning Tips | শেখার টিপস
-   FAQ & Resources | সাধারণ প্রশ্ন ও রিসোর্স

---

## Quick Start | দ্রুত শুরু

-   Python 3.7+
-   Jupyter Lab/Notebook
-   Libraries: pandas, matplotlib, seaborn, scikit-learn, pandas-profiling, gspread
-   পাইথন ৩.৭+, জুপিটার ল্যাব/নোটবুক, pandas, matplotlib, seaborn, scikit-learn, pandas-profiling, gspread

**Install | ইনস্টল করুন:**

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install pandas jupyterlab matplotlib seaborn scikit-learn pandas-profiling gspread
jupyter lab
```

---

## How to Use | কিভাবে ব্যবহার করবেন

-   Browse folders by topic (e.g., Pandas, Linear Regression, etc.) | টপিক অনুযায়ী ফোল্ডার দেখুন
-   Open any `.ipynb` notebook in Jupyter | যেকোনো `.ipynb` নোটবুক খুলুন
-   Each notebook has step-by-step code, explanation, and real datasets | প্রতিটি নোটবুকে ধাপে ধাপে কোড, ব্যাখ্যা ও ডেটাসেট আছে

---

## Expanded Notes by Folder | ফোল্ডারভিত্তিক বিস্তারিত নোট

### 01_pandas — Data Handling with Pandas

**Notebook Links | নোটবুক লিংক:**

-   [01_list to dataframe.ipynb](01_pandas/01_list%20to%20dataframe.ipynb)
-   [02_excel to df.ipynb](01_pandas/02_excel%20to%20df.ipynb)
-   [03_pandas profiling.ipynb](01_pandas/03_pandas%20profiling.ipynb)
-   [04_Importing Google Sheets using Python Pandas.ipynb](01_pandas/04_Importing%20Google%20Sheets%20using%20Python%20Pandas.ipynb)

**What is Pandas? | Pandas কী?**

-   English: Pandas is a powerful Python library for data manipulation and analysis. It lets you load, clean, transform, and analyze data efficiently.
-   বাংলা: Pandas হলো পাইথনের শক্তিশালী ডেটা ম্যানিপুলেশন ও অ্যানালাইসিস লাইব্রেরি। এটি দিয়ে সহজেই ডেটা লোড, ক্লিন, ট্রান্সফর্ম ও বিশ্লেষণ করা যায়।

**Key Concepts | মূল বিষয়:**

-   DataFrame creation from lists, dicts, CSV/Excel, Google Sheets
-   Data selection, filtering, sorting, grouping, aggregation
-   Data profiling for quick insights

**Basic Example | সহজ উদাহরণ:**

```python
import pandas as pd
# Load CSV | CSV ফাইল লোড করুন
df = pd.read_csv('Screen Time Data.csv')
print(df.head())  # Show first 5 rows | প্রথম ৫টি সারি দেখুন
```

**Advanced Example | একটু উন্নত উদাহরণ:**

```python
# Filter rows where 'Total Screen Time' > 100 | যেখানে 'Total Screen Time' ১০০-এর বেশি
filtered = df[df['Total Screen Time'] > 100]
print(filtered)

# Group by 'Week Day' and get average screen time | 'Week Day' অনুযায়ী গড় স্ক্রিন টাইম
avg_by_day = df.groupby('Week Day')['Total Screen Time'].mean()
print(avg_by_day)
```

**Tips | টিপস:**

-   Use `.info()`, `.describe()`, `.shape` to understand your data | ডেটা বোঝার জন্য এগুলো ব্যবহার করুন
-   Try `pandas_profiling` for a quick data report | দ্রুত রিপোর্টের জন্য `pandas_profiling` ব্যবহার করুন

---

### 02_types of var — Types of Variables in Data Science

**Notebook Link | নোটবুক লিংক:**

-   [01_Types of Variables in Data Science.ipynb](02_types%20of%20var/01_Types%20of%20Variables%20in%20Data%20Science.ipynb)

**Understanding Data: Key Dimensions | ডেটা বোঝার মূল দিক**

-   **Data Types | ডেটার ধরন:**
    -   Numerical (Discrete, Continuous) | সংখ্যাগত (ডিসক্রিট, কন্টিনিউয়াস)
    -   Categorical (Nominal, Ordinal, Binary) | ক্যাটাগরিক্যাল (নমিনাল, অর্ডিনাল, বাইনারি)
    -   Text, Date/Time | টেক্সট, তারিখ/সময়
-   **Measurement Scale | মাপার স্কেল:**
    -   Nominal, Ordinal, Interval, Ratio | নমিনাল, অর্ডিনাল, ইন্টারভ্যাল, রেশিও
-   **Role in Analysis | বিশ্লেষণে ভূমিকা:**
    -   Independent (Input), Dependent (Output) | ইনপুট, আউটপুট
-   **Distribution | ডিস্ট্রিবিউশন:**
    -   Normal, Skewed, Uniform, Bimodal | নরমাল, স্কিউড, ইউনিফর্ম, বাইমোডাল

**Why it matters? | কেন গুরুত্বপূর্ণ?**

-   Choosing the right statistical methods and visualizations depends on variable types.
-   সঠিক বিশ্লেষণ ও ভিজ্যুয়ালাইজেশনের জন্য ধরন জানা জরুরি।

**Example | উদাহরণ:**

```python
# Check data types | ডেটা টাইপ চেক করুন
print(df.dtypes)
```

---

### 03_linear regression — Linear Regression & Related Concepts

**Notebook Links | নোটবুক লিংক:**

-   [01_Regression Analysis.ipynb](03_linear%20regression/01_Regression%20Analysis.ipynb)
-   [02_Loss & Cost Functions in Linear Regression.ipynb](03_linear%20regression/02_Loss%20&%20Cost%20Functions%20in%20Linear%20Regression.ipynb)
-   [03_Coefficient of Determination(R-squared).ipynb](<03_linear%20regression/03_Coefficient%20of%20Determination(R-squared).ipynb>)
-   [04_Assignment 01 - Salary Prediction.ipynb](03_linear%20regression/04_Assignment%2001%20-%20Salary%20Prediction.ipynb)
-   [06\_ Linear Regression with Multiple Variables.ipynb](03_linear%20regression/06_%20Linear%20Regression%20with%20Multiple%20Variables.ipynb)
-   [08_Polynomial Regression.ipynb](03_linear%20regression/08_Polynomial%20Regression.ipynb)

**What is Linear Regression? | লিনিয়ার রিগ্রেশন কী?**

-   English: Linear Regression predicts a continuous value by fitting a straight line. Used for salary prediction, trend analysis, etc.
-   বাংলা: লিনিয়ার রিগ্রেশন একটি কন্টিনিউয়াস মান প্রেডিক্ট করতে সরল রেখা ফিট করে। যেমন: বেতন অনুমান, ট্রেন্ড বিশ্লেষণ।

**How does it work? | কিভাবে কাজ করে?**

-   Finds weights (w) so that `y = w0 + w1x1 + ... + wnxn` best fits the data.
-   ডেটার সাথে সবচেয়ে ভালো ফিট হয় এমন ওয়েট বের করে।

**Mathematical Formula | গাণিতিক সূত্র:**
\[
MSE = \frac{1}{N} \sum (y - \hat{y})^2
\]

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X, y)
print(model.predict([[5]]))  # Predict for 5 years experience | ৫ বছরের জন্য প্রেডিক্ট
```

**Advanced Example | উন্নত উদাহরণ:**

```python
# Polynomial Regression | পলিনোমিয়াল রিগ্রেশন
from sklearn.preprocessing import PolynomialFeatures
poly = PolynomialFeatures(degree=2)
X_poly = poly.fit_transform(X)
model.fit(X_poly, y)
```

**Tips | টিপস:**

-   Visualize your data and regression line | ডেটা ও রিগ্রেশন লাইন প্লট করুন
-   Use train-test split for evaluation | মডেল যাচাইয়ের জন্য train-test split ব্যবহার করুন

---

### 04_Feature Enginerring — Feature Engineering

**Notebook Links | নোটবুক লিংক:**

-   [01_Label Encoder in Machine Learning.ipynb](04_Feature%20Enginerring/01_Label%20Encoder%20in%20Machine%20Learning.ipynb)
-   [02_One-Hot Encoding in Machine Learning.ipynb](04_Feature%20Enginerring/02_One-Hot%20Encoding%20in%20Machine%20Learning.ipynb)
-   [03\_ Binary Encoder Explained in Machine Learning.ipynb](04_Feature%20Enginerring/03_%20Binary%20Encoder%20Explained%20in%20Machine%20Learning.ipynb)
-   [04_Ordinal Encoder.ipynb](04_Feature%20Enginerring/04_Ordinal%20Encoder.ipynb)
-   [05\_ Min Max Normalization.ipynb](04_Feature%20Enginerring/05_%20Min%20Max%20Normalization.ipynb)
-   [06_Standardization Z-Score.ipynb](04_Feature%20Enginerring/06_Standardization%20Z-Score.ipynb)

**What is Feature Engineering? | ফিচার ইঞ্জিনিয়ারিং কী?**

-   English: Transforming raw data into features for ML (encoding, scaling).
-   বাংলা: কাঁচা ডেটাকে মডেলিংয়ের জন্য ফিচারে রূপান্তর করা (এনকোডিং, স্কেলিং)।

**Key Techniques | মূল টেকনিক:**

-   Label, One-Hot, Binary, Ordinal encoding; Min-Max scaling; Standardization.

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
df['encoded'] = le.fit_transform(df['category'])  # ক্যাটাগরি এনকোডিং
```

**Advanced Example | উন্নত উদাহরণ:**

```python
# One-hot encoding | ওয়ান-হট এনকোডিং
import pandas as pd
dummies = pd.get_dummies(df['Area'], drop_first=True)
df = pd.concat([df, dummies], axis=1)
```

**Tips | টিপস:**

-   Always encode categorical variables before modeling | ক্যাটাগরিক্যাল ডেটা এনকোড করুন
-   Scale features for algorithms like KNN, SVM | KNN, SVM-এর জন্য ফিচার স্কেল করুন

---

### 05_project_multiple_linear_regression — Multiple Linear Regression Project

**Notebook Link | নোটবুক লিংক:**

-   [01_Profit Prediction using Multiple Linear Regression.ipynb](05_project_multiple_linear_regression/01_Profit%20Prediction%20using%20Multiple%20Linear%20Regression.ipynb)

**Project Overview | প্রজেক্ট ওভারভিউ:**

-   Predicting profit using multiple features (Marketing Spend, Administration, Transport, Area).
-   Data cleaning, one-hot encoding, train-test split, model fitting, scoring.

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
```

**Advanced Example | উন্নত উদাহরণ:**

```python
# One-hot encoding for categorical feature
city = pd.get_dummies(X['Area'], drop_first=True)
X = X.drop('Area', axis=1)
X = pd.concat([X, city], axis=1)
```

**Tips | টিপস:**

-   Always check for nulls or zeros in data before modeling | মডেল করার আগে ডেটা null বা 0 কিনা চেক করুন

---

### 06_Gradient Descent — Gradient Descent

**Notebook Link | নোটবুক লিংক:**

-   [01_gradient descent_linear regression.ipynb](06_Gradient%20Descent/01_gradient%20descent_linear%20regression.ipynb)

**What is Gradient Descent? | গ্র্যাডিয়েন্ট ডিসেন্ট কী?**

-   English: Optimization algorithm to minimize cost functions.
-   বাংলা: কস্ট ফাংশন মিনিমাইজ করার অপ্টিমাইজেশন অ্যালগরিদম।

**Steps | ধাপসমূহ:**

1. Initialize parameters (e.g., m, c = 0)
2. Update using gradients
3. Repeat for set iterations

**Basic Example | সহজ উদাহরণ:**

```python
m, c = 0, 0
learning_rate = 0.001
for i in range(1000):
    y_pred = m*x + c
    md = -(2/n) * sum(x*(y-y_pred))
    cd = -(2/n) * sum(y-y_pred)
    m = m - learning_rate * md
    c = c - learning_rate * cd
```

**Tips | টিপস:**

-   Choose learning rate carefully | লার্নিং রেট ঠিকভাবে দিন

---

### 07_Decision Tree — Decision Tree

**Notebook Link | নোটবুক লিংক:**

-   [01_Classification- Decision Tree Construction in Machine Learning.ipynb](07_Decision%20Tree/01_Classification-%20Decision%20Tree%20Construction%20in%20Machine%20Learning.ipynb)

**What is a Decision Tree? | ডিসিশন ট্রি কী?**

-   English: Splits data into branches to make decisions.
-   বাংলা: ডেটাকে ভাগ করে সিদ্ধান্ত নেয়।

**Key Concepts | মূল বিষয়:**

-   Information gain, entropy, tree pruning.

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.tree import DecisionTreeClassifier
clf = DecisionTreeClassifier()
clf.fit(X, y)
```

**Tips | টিপস:**

-   Prune trees to avoid overfitting | ওভারফিটিং এড়াতে ট্রি ছোট করুন

---

### 08_Confusion Matrix — Confusion Matrix

**Notebook Link | নোটবুক লিংক:**

-   [01_Confusion Matrix with Python.ipynb](08_Confusion%20Matrix/01_Confusion%20Matrix%20with%20Python.ipynb)

**What is a Confusion Matrix? | কনফিউশন ম্যাট্রিক্স কী?**

-   Table to evaluate classification model performance.
-   ক্লাসিফিকেশন মডেলের পারফরম্যান্স যাচাইয়ের টেবিল।

**Metrics | মেট্রিক্স:**

-   Accuracy, Precision, Recall, F1-score

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.metrics import confusion_matrix
cm = confusion_matrix(y_true, y_pred)
```

**Tips | টিপস:**

-   Always check all metrics, not just accuracy | শুধু accuracy নয়, সব মেট্রিক দেখুন

---

### 09_K-Fold Cross Validation — K-Fold Cross Validation

**Notebook Link | নোটবুক লিংক:**

-   [01_XGBoost- Implementing K-Fold Cross Validation with Python & XGBoost Classifier.ipynb](09_K-Fold%20Cross%20Validation/01_XGBoost-%20Implementing%20K-Fold%20Cross%20Validation%20with%20Python%20&%20XGBoost%20Classifier.ipynb)

**What is K-Fold CV? | K-Fold ক্রস ভ্যালিডেশন কী?**

-   Splits data into k parts to validate model robustness.
-   ডেটাকে k ভাগে ভাগ করে মডেল যাচাই করা।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.model_selection import cross_val_score
scores = cross_val_score(model, X, y, cv=5)
```

**Tips | টিপস:**

-   Use cross-validation for robust evaluation | মডেল যাচাইয়ের জন্য cross-validation ব্যবহার করুন

---

### 10_Logistic Regression Classification — Logistic Regression

**Notebook Links | নোটবুক লিংক:**

-   [01_Logistic Regression in Machine Learning.ipynb](10_Logistic%20Regression%20Classification/01_Logistic%20Regression%20in%20Machine%20Learning.ipynb)
-   [customer_churn_prediction.ipynb](10_Logistic%20Regression%20Classification/customer_churn_prediction.ipynb)

**What is Logistic Regression? | লজিস্টিক রিগ্রেশন কী?**

-   Used for binary classification (yes/no, 0/1).
-   দুই ক্লাসের (হ্যাঁ/না, ০/১) প্রেডিকশনের জন্য ব্যবহৃত।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.linear_model import LogisticRegression
logreg = LogisticRegression()
logreg.fit(X, y)
print(logreg.predict([[2, 5000]]))  # উদাহরণ ইনপুট
```

**Tips | টিপস:**

-   Use for classification, not regression | ক্লাসিফিকেশনের জন্য ব্যবহার করুন
-   Scale features for better results | ফিচার স্কেল করুন

---

### 11\_ Support Vector Machine — SVM

**Notebook Link | নোটবুক লিংক:**

-   [SVM in Machine Learning.ipynb](11_%20Support%20Vector%20Machine/SVM%20in%20Machine%20Learning.ipynb)

**What is SVM? | SVM কী?**

-   Finds the best boundary (hyperplane) to separate classes.
-   ক্লাস আলাদা করতে সবচেয়ে ভালো বাউন্ডারি বের করে।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.svm import SVC
svm = SVC()
svm.fit(X, y)
```

**Tips | টিপস:**

-   Try different kernels | বিভিন্ন kernel ব্যবহার করুন

---

### 12_Predicting Heart Disease using Random Forest — Random Forest

**Notebook Link | নোটবুক লিংক:**

-   [Predicting Heart Disease using Random Forest.ipynb](12_Predicting%20Heart%20Disease%20using%20Random%20Forest/Predicting%20Heart%20Disease%20using%20Random%20Forest.ipynb)

**What is Random Forest? | র‍্যান্ডম ফরেস্ট কী?**

-   Ensemble of decision trees for better accuracy.
-   অনেক ডিসিশন ট্রির সমষ্টি।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.ensemble import RandomForestClassifier
rf = RandomForestClassifier()
rf.fit(X, y)
```

**Tips | টিপস:**

-   Good for tabular data | টেবিল ডেটার জন্য ভালো

---

### 13_Save ML Model Pickle vs Joblib — Model Saving

**Notebook Link | নোটবুক লিংক:**

-   [Save ML Model and Pickle vs Joblib.ipynb](13_Save%20ML%20Model%20Pickle%20vs%20Joblib/Save%20ML%20Model%20and%20Pickle%20vs%20Joblib.ipynb)

**What is Model Saving? | মডেল সংরক্ষণ কী?**

-   Save and load ML models for reuse.
-   মডেল সংরক্ষণ ও পুনরায় ব্যবহার।

**Basic Example | সহজ উদাহরণ:**

```python
import joblib
joblib.dump(model, 'model.joblib')
```

**Tips | টিপস:**

-   Use Joblib for large models | বড় মডেলের জন্য Joblib ব্যবহার করুন

---

### 14_K-Nearest Neighbors Algorithm in ML — KNN

**Notebook Links | নোটবুক লিংক:**

-   [01_K-nearest regreessor and removing outliers (gaussian distribution).ipynb](<14_K-Nearest%20Neighbors%20Algorithm%20in%20ML/01_K-nearest%20regreessor%20and%20removing%20outliers%20(gaussian%20distribution).ipynb>)
-   [02_Knn \_classifier.ipynb](14_K-Nearest%20Neighbors%20Algorithm%20in%20ML/02_Knn%20_classifier.ipynb)

**What is KNN? | KNN কী?**

-   Predicts by looking at the k closest data points.
-   কাছের k ডেটা পয়েন্ট দেখে প্রেডিক্ট করে।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.neighbors import KNeighborsClassifier
knn = KNeighborsClassifier(n_neighbors=3)
knn.fit(X, y)
```

**Tips | টিপস:**

-   Scale features for distance-based algorithms | ফিচার স্কেল করুন

---

### 15\_ What is CountVectorizer in Python & How CountVectorizer Work — CountVectorizer

**Notebook Link | নোটবুক লিংক:**

-   [1_CountVectorizer in Python.ipynb](15_%20What%20is%20CountVectorizer%20in%20Python%20&%20How%20CountVectorizer%20Work/1_CountVectorizer%20in%20Python.ipynb)

**What is CountVectorizer? | CountVectorizer কী?**

-   Converts text to numeric features for ML.
-   টেক্সটকে নিউমেরিক ফিচারে রূপান্তর।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()
X_vec = cv.fit_transform(text_data)
```

**Tips | টিপস:**

-   Try on your own text data | নিজের টেক্সট ডেটায় চেষ্টা করুন

---

### 16_Naive Bayes Algorithm with Python — Naive Bayes

**Notebook Link | নোটবুক লিংক:**

-   [1.Naive Bayes Algorithm with Python.ipynb](16_Naive%20Bayes%20Algorithm%20with%20Python/1.Naive%20Bayes%20Algorithm%20with%20Python.ipynb)

**What is Naive Bayes? | নায়েভ বেইজ কী?**

-   Probabilistic classifier based on Bayes' theorem.
-   Bayes' theorem ভিত্তিক সম্ভাব্যতাভিত্তিক ক্লাসিফায়ার।

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.naive_bayes import GaussianNB
nb = GaussianNB()
nb.fit(X, y)
```

**Tips | টিপস:**

-   Good for text data | টেক্সট ডেটার জন্য ভালো

---

### 17*NLP Project* Spam eMail Detection with Naive Bayes Classifiers — NLP Spam Detection

**Notebook Link | নোটবুক লিংক:**

-   [01_Spam eMail Detection with Naive Bayes Classifiers.ipynb](17_NLP%20Project_%20Spam%20eMail%20Detection%20with%20Naive%20Bayes%20Classifiers/01_Spam%20eMail%20Detection%20with%20Naive%20Bayes%20Classifiers.ipynb)

**What is NLP Spam Detection? | NLP স্প্যাম ডিটেকশন কী?**

-   Detects spam emails using NLP and Naive Bayes.
-   NLP ও Naive Bayes দিয়ে স্প্যাম ইমেইল শনাক্তকরণ।

**Key Steps | ধাপসমূহ:**

-   Data cleaning, feature extraction (CountVectorizer), model training, evaluation.

**Basic Example | সহজ উদাহরণ:**

```python
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
cv = CountVectorizer()
X_vec = cv.fit_transform(text_data)
model = MultinomialNB()
model.fit(X_vec, y)
```

**Tips | টিপস:**

-   Always preprocess text data | টেক্সট ডেটা প্রিপ্রসেস করুন

---

## Learning Tips | শেখার টিপস

-   Practice by running code | কোড চালিয়ে প্র্যাকটিস করুন
-   Visualize data and results | ডেটা ও রেজাল্ট ভিজ্যুয়ালাইজ করুন
-   Read documentation | ডকুমেন্টেশন পড়ুন
-   Take notes | নোট নিন

---

## FAQ & Resources | সাধারণ প্রশ্ন ও রিসোর্স

-   **ModuleNotFoundError?** Install all libraries: `pip install ...` | সব লাইব্রেরি ইনস্টল করুন
-   **Jupyter won’t start?** Try `jupyter notebook` | চালু না হলে `jupyter notebook` ব্যবহার করুন
-   **Data file not found?** Run from project root | প্রজেক্ট রুট থেকে চালান
-   **Google Sheets import?** See [Google Sheets notebook](01_pandas/04_Importing%20Google%20Sheets%20using%20Python%20Pandas.ipynb)

**Resources | রিসোর্স:**

-   [Pandas Docs](https://pandas.pydata.org/docs/)
-   [Scikit-learn Docs](https://scikit-learn.org/stable/documentation.html)
-   [Matplotlib Docs](https://matplotlib.org/stable/users/index.html)
-   [Kaggle Datasets](https://www.kaggle.com/datasets)
-   [Google Colab](https://colab.research.google.com/)

---

**Happy Learning! | শুভকামনা! 🚀**
