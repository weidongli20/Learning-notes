# Learning-notes

* pandas hints

  - ``` > ix = (df.index >= '2018-01-01 00:00:00.500') & (df.index <='2018-01-01 00:00:01.200') df[ix] ```
  - ``` > df[np.logical_not(df['group'] == 'vegetable')] ```
  - ``` > time_index = pd._to_datetime(date_str) + ser_int.astype('timedelta64[h]') - pd.Timedelta('1h') ```
  - ``` > df2 = df.rename({'a': 'X', 'b': 'Y'}, axis=1)  # new method
df2 = df.rename({'a': 'X', 'b': 'Y'}, axis='columns')
df2 = df.rename(columns={'a': 'X', 'b': 'Y'})  # old method  ```

| Alias  |  Description |
| ------ |:-------------:| 
| B      |    business day frequency |
| C      |   custom business day frequency |
| D      |   calendar day frequency |
| W      |     weekly frequency |
| M      |    month end frequency |
| SM     |     semi-month end frequency (15th and end of month) |
| BM     |    business month end frequency |
| CBM    |    custom business month end frequency |
| MS     |    month start frequency |
| SMS    |    semi-month start frequency (1st and 15th) |
| BMS    |    business month start frequency |
| CBMS   |    custom business month start frequency |
| Q      |    quarter end frequency |
| BQ     |    business quarter end frequency |
| QS     |    quarter start frequency |
| BQS    |    business quarter start frequency |
| A, Y   |    year end frequency |
| BA, BY |    business year end frequency |
| AS, YS |    year start frequency |
| BAS, BYS  |  business year start frequency |
| BH     |    business hour frequency |
| H      |    hourly frequency |
| T, min |    minutely frequency |
| S      |    secondly frequency |
| L, ms  |    milliseconds |
| U, us  |    microseconds |
| N      |    nanoseconds |

https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases

* conda

  - ``` > conda env export --from-history -> py35.yml ```
  
    ``` > conda env create -f py35.yml ```
