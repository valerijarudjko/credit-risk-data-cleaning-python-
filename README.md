# Data Cleaning with Pandas - Fixing Messy Credit Data

- Data: [Credit Risk Customers](https://www.kaggle.com/datasets/ppb00x/credit-risk-customers)

 ## Create your environment
```bash
python3.11.1 -m venv my_env1    # <-- choose yoor python version and name of your environment
```



## Install the Kaggle CLI

1. Open your VS Code integrated terminal and run:
```bash
pip install kaggle
```
This gives you access to the kaggle command-line tool

2. Get your Kaggle API credentials

- Sign in at https://www.kaggle.com, click your user icon → Account, then hit Create API Token.
- A file named kaggle.json will download.
  
- Move it into your home Kaggle folder:
##### Mac/Linux: ~/.kaggle/kaggle.json
##### Windows: C:\Users\<YourUser>\.kaggle\kaggle.json
- Secure it (on Unix):
```bash
chmod 600 ~/.kaggle/kaggle.json
```
##### This lets the CLI authenticate.

# Download & unzip the dataset
- In VS Code terminal run:
```bash
kaggle datasets download \
  -d ppb00x/credit-risk-customers \
  -p data/credit-risk-customers \
  --unzip
```
-d specifies the dataset slug; -p sets the target directory; --unzip extracts the files in place

- Load the data in Python:
In your .py or Jupyter file, use pandas to read whichever CSV(s) you need.

- For example (adjust the filename to match what was unzipped):
```bash
df = pd.read_csv('data/credit-risk-customers.csv')
print(df.head())
```


## Importing libraries:
```bash
pip install pandas
pip install openpyxl
```
```python
import pandas as pd
```












#### Acknowledgments
- Data Source: Kaggle’s Credit Risk Customers
- Inspiration: @onurdatascience
