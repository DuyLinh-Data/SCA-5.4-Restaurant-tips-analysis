# Session-5.4-Restaurant-tips-analysis
**1.The First Steps**
# Data import

import pandas as pd

import matplotlib as plt

# Load data from the link:

data = pd.read_csv("https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv")

# Look at the first 5 rows:   

data.head()

# Show the columns of the dataframe and their types:

data.info()
data.describe()

# Fix their types and make them string + Check info:

data = data.astype(str)

data.info()

data.describe()

**2.Tip value influencers**

# Create a new dataframe smokers_df containing only info about smokers:

smokers_df = data.query('smoker =="Yes"')

smokers_df.sample(5)

# Also create another one dataframe non_smokers_df containing only non-smokers:

non_smokers_df = data.query('smoker =="No"')

non_smokers_df.sample(5)

**Compare their measures of central tendency**

# Calculate them for the 'tip' column:

data['tip'] = pd.to_numeric(data['tip'], errors='coerce')

common_tip_min = data['tip'].min()

common_tip_max = data['tip'].max()

common_tip_mean = data['tip'].mean()

common_tip_median = data['tip'].median()

# Smokers

non_smokers_tip_min = pd.to_numeric(smokers_df['tip']).min()

non_smokers_tip_max = pd.to_numeric(smokers_df['tip']).max()

non_smokers_tip_mean = pd.to_numeric(smokers_df['tip']).mean()

non_smokers_tip_median = pd.to_numeric(smokers_df['tip']).median()

print(smokers_tip_min)

print(smokers_tip_max)

print(smokers_tip_mean)

print(smokers_tip_median)

# Non-smokers

non_smokers_tip_min = pd.to_numeric(non_smokers_df['tip']).min()

non_smokers_tip_max = pd.to_numeric(non_smokers_df['tip']).max()

non_smokers_tip_mean = pd.to_numeric(non_smokers_df['tip']).mean()

non_smokers_tip_median = pd.to_numeric(non_smokers_df['tip']).median()

print(non_smokers_tip_min)

print(non_smokers_tip_max)

print(non_smokers_tip_mean)

print(non_smokers_tip_median)

**Look at histograms**

# Plot the histogram

import matplotlib.pyplot as plt

plt.figure(figsize=(15, 5))

plt.hist(data.tip, bins = 5, color = '#74b9ff')

# Customize the plot

plt.xlabel('Tip value')

plt.ylabel('Frequency')

plt.title('Whole dataset tip values')

plt.grid(True)

# Show the plot

plt.show()

#**Smokers tips histogram**

import pandas as pd

import matplotlib.pyplot as plt

# Plot the histogram

plt.figure(figsize=(15, 5))

plt.hist(smokers_tips.tip, bins = 5, color = '#ff7675')

# Customize the plot

plt.xlabel('Tip value')

plt.ylabel('Frequency')

plt.title('Smokers tip values')

plt.grid(True)

# Show the plot
plt.show()

#**Non-smokers tips histogram**

import pandas as pd

import matplotlib.pyplot as plt

non_smokers_tips = pd.DataFrame({'tip': [1, 2, 3, 4, 5]})

# Plot the histogram

plt.figure(figsize=(15, 5))

plt.hist(non_smokers_tips['tip'], bins=5, color='#55efc4')

# Customize the plot

plt.xlabel('Tip value')

plt.ylabel('Frequency')

plt.title('Non-smokers tip values')

plt.grid(True)

# Show the plot
plt.show()
