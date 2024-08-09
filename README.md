# Session-5.4-Restaurant-tips-analysis
**1.The First Steps**
#Data import

import pandas as pd

import matplotlib as plt

#Then load data from the following link: https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv:

data = pd.read_csv("https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv")

#Let's take a look at the first 5 rows to be sure, that data is loaded properly:     

data.head()

#Show the columns of the dataframe and their types:

data.info()
data.describe()

#Fix their types and make them string + Check info:

data = data.astype(str)

data.info()

data.describe()

**2.Tip value influencers**

#Create a new dataframe smokers_df containing only info about smokers:

smokers_df = data.query('smoker =="Yes"')

smokers_df.sample(5)

#Also create another one dataframe non_smokers_df containing only non-smokers:

non_smokers_df = data.query('smoker =="No"')

non_smokers_df.sample(5)

**Compare their measures of central tendency**
