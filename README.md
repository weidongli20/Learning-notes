# Learning-notes

* pandas hints

  - ``` > ix = (df.index >= '2018-01-01 00:00:00.500') & (df.index <='2018-01-01 00:00:01.200') df[ix] ```
  - ``` > df[np.logical_not(df['group'] == 'vegetable')] ```


* conda

  - ``` > conda env export --from-history -> py35.yml ```
  
    ``` > conda env create -f py35.yml ```
