# 📒 আমার ডেটা সায়েন্স ও মেশিন লার্নিং নোটবুক কালেকশন

> "নিজের শেখার জন্য, নিজের ভাষায়, নিজের মতো করে!"

---

## 📖 সূচিপত্র (Table of Contents)

- [👋 সূচনা](#-সূচনা)
- [🚀 Quick Links](#-quick-links)
- [🛠️ How to Use](#-how-to-use)
- [📂 কালেকশন](#-কালেকশন)
  - [১. Pandas ও ডেটা হ্যান্ডলিং (`01_pandas`)](#১-pandas-ও-ডেটা-হ্যান্ডলিং-01_pandas)
  - [২. ভেরিয়েবল ও ডেটার ধরন (`02_types of var`)](#২-ভেরিয়েবল-ও-ডেটার-ধরন-02_types-of-var)
  - [৩. লিনিয়ার রিগ্রেশন (`03_linear regression`)](#৩-লিনিয়ার-রিগ্রেশন-03_linear-regression)
  - [৪. ফিচার ইঞ্জিনিয়ারিং (`04_Feature Enginerring`)](#৪-ফিচার-ইঞ্জিনিয়ারিং-04_feature-enginerring)
  - [৫. প্রজেক্ট: মাল্টিপল লিনিয়ার রিগ্রেশন (`05_project_multiple_linear_regression`)](#৫-প্রজেক্ট-মাল্টিপল-লিনিয়ার-রিগ্রেশন-05_project_multiple_linear_regression)
- [✨ আমার শেখার টিপস](#-আমার-শেখার-টিপস)
- [🏁 শেষ কথা](#-শেষ-কথা)

---

## 👋 সূচনা

এই রেপোটা আমার ডেটা সায়েন্স ও মেশিন লার্নিং শেখার জার্নির নোট, কোড, আর উদাহরণ দিয়ে সাজানো। সবকিছু বাংলায় লিখেছি যেন ভবিষ্যতে একবার দেখলেই সব মনে পড়ে যায়।

---

## 🚀 Quick Links

- **[বেসিক Pandas অপারেশন](01_pandas/02_excel%20to%20df.ipynb)**
- **[স্যালারি প্রেডিকশন প্রজেক্ট](03_linear%20regression/04_Assignment%2001%20-%20Salary%20Prediction.ipynb)**
- **[প্রফিট প্রেডিকশন প্রজেক্ট](05_project_multiple_linear_regression/01_Profit%20Prediction%20using%20Multiple%20Linear%20Regression.ipynb)**

---

## 🛠️ How to Use

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd your-repo-name
    ```
3.  **Install the required libraries:**
    ```bash
    pip install pandas jupyterlab matplotlib seaborn scikit-learn pandas-profiling gspread
    ```
4.  **Run Jupyter Lab:**
    ```bash
    jupyter lab
    ```

---

## 📂 কালেকশন

### ১. Pandas ও ডেটা হ্যান্ডলিং (`01_pandas`)

| ফাইল                                                              | বর্ণনা                                                                                             | টিপস                                                                                   |
| ----------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| **[01_list to dataframe.ipynb](01_pandas/01_list%20to%20dataframe.ipynb)** | Python list থেকে DataFrame বানানো, ইনডেক্স-কলাম কাস্টমাইজ, dict থেকে DataFrame — সব হাতে কলমে।      | `.shape`, `.info()`, `.columns` এগুলো দিয়ে ডেটার গঠন চেক করা যায়।                        |
| **[02_excel to df.ipynb](01_pandas/02_excel%20to%20df.ipynb)**         | CSV ফাইল থেকে ডেটা আনা, সাবসেটিং, সোর্টিং, বেসিক স্ট্যাটস, করেলেশন, হিটম্যাপ — সব এক জায়গায়। | `.read_csv()`, `.head()`, `.sort_values()`, `.describe()`, `.corr()` — এগুলো খুব কাজে লাগে। |
| **[03_pandas profiling.ipynb](01_pandas/03_pandas%20profiling.ipynb)** | ডেটার অটো রিপোর্ট — এক ক্লিকে পুরো ডেটার সারাংশ।                                                    | `pandas_profiling` দিয়ে ডেটার সমস্যা, missing value, outlier সব ধরা যায়।                |
| **[04_Importing Google Sheets...](01_pandas/04_Importing%20Google%20Sheets%20using%20Python%20Pandas.ipynb)** | Google Sheets থেকে ডেটা আনার সহজ উপায়, gspread দিয়ে।                                              | Google API credentials লাগবে, শিট শেয়ার করতে হবে সার্ভিস অ্যাকাউন্টে।                      |
| **Screen Time Data.csv**                                          | মোবাইল স্ক্রিন টাইমের ডেটাসেট, নিজের ডেটা এনালাইসিসের জন্য।                                         |                                                                                        |

### ২. ভেরিয়েবল ও ডেটার ধরন (`02_types of var`)

| ফাইল                                                                      | বর্ণনা                                                    | টিপস                                        |
| ------------------------------------------------------------------------- | --------------------------------------------------------- | ------------------------------------------- |
| **[01_Types of Variables...](02_types%20of%20var/01_Types%20of%20Variables%20in%20Data%20Science.ipynb)** | ভেরিয়েবলের ধরন, মেজারমেন্ট স্কেল, ডেটার role — সব বাংলায়। | ডেটার ধরন বুঝে এনালাইসিস করলে ভুল কম হয়। |

### ৩. লিনিয়ার রিগ্রেশন (`03_linear regression`)

| ফাইল                                                                                    | বর্ণনা                                                              | ডেটাসেট                                                                                             |
| --------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **[01_Regression Analysis.ipynb](03_linear%20regression/01_Regression%20Analysis.ipynb)** | লিনিয়ার রিগ্রেশন, ডেটা ভিজ্যুয়ালাইজেশন, মডেল ফিটিং, প্রেডিকশন।      | `linear_data.csv`                                                                                   |
| **[02_Loss & Cost Functions...](03_linear%20regression/02_Loss%20&%20Cost%20Functions%20in%20Linear%20Regression.ipynb)** | লস ফাংশন (MSE, MAE), মডেল ইভালুয়েশন।                               |                                                                                                     |
| **[03_Coefficient of Determination...](03_linear%20regression/03_Coefficient%20of%20Determination(R-squared).ipynb)** | R-squared মান, মডেলের পারফরম্যান্স।                                 |                                                                                                     |
| **[04_Assignment 01 - Salary Prediction.ipynb](03_linear%20regression/04_Assignment%2001%20-%20Salary%20Prediction.ipynb)** | বাস্তব ডেটা দিয়ে স্যালারি প্রেডিকশন।                                 | `Salary Data.csv`                                                                                   |
| **[05_Assignment_car_risk_analysis.ipynb](03_linear%20regression/05_Assignment_car_risk_analysis.ipynb)** | গাড়ি চালানোর রিস্ক এনালাইসিস।                                       | `car driving risk analysis.csv`                                                                     |
| **[06_ Linear Regression with Multiple Variables.ipynb](03_linear%20regression/06_%20Linear%20Regression%20with%20Multiple%20Variables.ipynb)** | মাল্টিপল ভেরিয়েবল নিয়ে রিগ্রেশন।                                     | `nasdaq100.csv`                                                                                     |
| **[07_pearson Correlation coefficient.ipynb](03_linear%20regression/07_pearson%20Correlation%20coefficient.ipynb)** | পিয়ারসন করেলেশন ক্যালকুলেশন।                                         |                                                                                                     |
| **[08_Polynomial Regression.ipynb](03_linear%20regression/08_Polynomial%20Regression.ipynb)** | নন-লিনিয়ার ডেটার জন্য পলিনোমিয়াল রিগ্রেশন।                           | `nonlinear_data.csv`                                                                                |

### ৪. ফিচার ইঞ্জিনিয়ারিং (`04_Feature Enginerring`)

| ফাইল                                                                                                | বর্ণনা                                                    | টিপস                                       |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------- | ------------------------------------------ |
| **[01_Label Encoder...](04_Feature%20Enginerring/01_Label%20Encoder%20in%20Machine%20Learning.ipynb)** | ক্যাটাগরিক্যাল ডেটাকে লেবেল এনকোডিং।                       | এনকোডিং আর স্কেলিং ছাড়া মডেলিং ঠিকমতো হয় না! |
| **[02_One-Hot Encoding...](04_Feature%20Enginerring/02_One-Hot%20Encoding%20in%20Machine%20Learning.ipynb)** | ওয়ান-হট এনকোডিং।                                          |                                            |
| **[03_ Binary Encoder...](04_Feature%20Enginerring/03_%20Binary%20Encoder%20Explained%20in%20Machine%20Learning.ipynb)** | বাইনারি এনকোডিং।                                          |                                            |
| **[04_Ordinal Encoder.ipynb](04_Feature%20Enginerring/04_Ordinal%20Encoder.ipynb)**                   | অর্ডিনাল ডেটার জন্য এনকোডিং।                               |                                            |
| **[05_ Min Max Normalization.ipynb](04_Feature%20Enginerring/05_%20Min%20Max%20Normalization.ipynb)** | ডেটা স্কেলিং (০-১)।                                       |                                            |
| **[06_Standardization Z-Score.ipynb](04_Feature%20Enginerring/06_Standardization%20Z-Score.ipynb)**   | ডেটা স্ট্যান্ডার্ডাইজেশন (মিন=০, SD=১)।                     |                                            |

### ৫. প্রজেক্ট: মাল্টিপল লিনিয়ার রিগ্রেশন (`05_project_multiple_linear_regression`)

| ফাইল                                                                                                                            | বর্ণনা                                                                                             | ডেটাসেট      |
| ------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | ------------ |
| **[01_Profit Prediction...](05_project_multiple_linear_regression/01_Profit%20Prediction%20using%20Multiple%20Linear%20Regression.ipynb)** | একাধিক ইনপুট (Marketing Spend, Administration, Transport, Area) থেকে Profit প্রেডিকশন। One-hot encoding, train-test split, মডেল ফিটিং, স্কোরিং, R-squared — সব এক জায়গায়। | `online.csv` |

---

## ✨ আমার শেখার টিপস

-   **প্র্যাকটিস:** কোড নিজে চালাও, নিজের ডেটা দিয়ে চেষ্টা করো।
-   **ভিজ্যুয়ালাইজেশন:** সবসময় গ্রাফ/চার্টে দেখো, চোখে পড়লে মনে থাকে।
-   **ডকুমেন্টেশন:** pandas, sklearn, matplotlib — অফিসিয়াল ডকুমেন্টেশন পড়ো।
-   **প্রশ্ন:** না বুঝলে গুগল/চ্যাটজিপিটি/স্ট্যাকওভারফ্লোতে প্রশ্ন করো।
-   **নোট:** শেখার সময় ছোট ছোট নোট রাখো, পরে কাজে লাগবে।

---

## 🏁 শেষ কথা

এই রেপোটা আমার শেখার সঙ্গী। সময় পেলে নতুন টপিক, প্রজেক্ট, উদাহরণ যোগ করবো।

**শুভকামনা!** 🚀