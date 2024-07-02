# UserRetention Analysis 

### Import Necessary Packages
```python
pip install pandas
pip install numpy
pip install datetime
```

### Import Data from Csv 
```python
df = pd.read_csv(Salinan_Online_Retail_Data.csv)
df
```

### Data Cleansing
- Convert date
- Clean all rows without data
- Make all data in lower case for product_name column
- make new columns for status whether delivered or cancelled
- Add filter to make ranking for product

### Create User Retention Cohort
  - Aggregate transaction data into total summary of transaction/order of each user per month
  - Create column as cohort for usert that buy for the first time
  - Calculate the length bbetween months of transaction with first month of transaction ( Make the index 0 as 1, so month 0 (first month)
  - Make Pivot Table
  - Calculate how many users in each of the cohorts
  - Retention rate
    ![output](https://github.com/wildanzzam/User-Retention-Analysis/assets/141975092/bb5b2931-c7f9-47c2-903d-e5598ed612d9)
