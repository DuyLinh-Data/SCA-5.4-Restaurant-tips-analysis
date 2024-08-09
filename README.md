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

#Calculate them for the 'tip' column:

data['tip'] = pd.to_numeric(data['tip'], errors='coerce')

common_tip_min = data['tip'].min()

common_tip_max = data['tip'].max()

common_tip_mean = data['tip'].mean()

common_tip_median = data['tip'].median()

#Smokers

non_smokers_tip_min = pd.to_numeric(smokers_df['tip']).min()
non_smokers_tip_max = pd.to_numeric(smokers_df['tip']).max()
non_smokers_tip_mean = pd.to_numeric(smokers_df['tip']).mean()
non_smokers_tip_median = pd.to_numeric(smokers_df['tip']).median()


