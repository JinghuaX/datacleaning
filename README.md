# datacleaning in python 
import pandas as pd
import numpy as np

#read in data 
sample_data=pd.read_csv()
# set seed for reproducibility
np.random.seed(0) 

#look at the data to see if I see any missing values, which will be reprsented with `NaN` or `None`.
sample_data.sample(10)

# See how many missing data points we have
# get the number of missing data points per column
missing_values_count = sample_data.isnull().sum()
# look at the # of missing points in the first ten columns
missing_values_count[0:10]

# how many total missing values do we have?
total_cells = np.product(data.shape)
total_missing = missing_values_count.sum()

# percent of data that is missing
(total_missing/total_cells) * 100

 
