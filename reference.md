# References

Use this space to list any references such as books or websites you used to complete the assessment, such as links to documentation or forum posts (please link to the specific question). You do not need to list any materials provided as part of the NPP course.

If you used any Chat GPT sessions to help you, please link to the specific session (see https://help.openai.com/en/articles/7925741-chatgpt-shared-links-faq for details on how to do this).

If you used other AI tools (e.g. GitHub Copilot) then list the tool and explain how it helped you (e.g. "I asked GitHub Copilot to generate a function to calculate the aritmetic-geoemtric mean of a list of numbers, and then modified the code to be able to work on a pandas DataFrame").

### Websites
#### For open and concatenate file:
- [Stack Overflow: Import multiple CSV files into pandas and concatenate into one DataFrame] (https://stackoverflow.com/questions/20906474/import-multiple-csv-files-into-pandas-and-concatenate-into-one-dataframe#:~:text=If%20multiple%20CSV%20files%20are%20zipped,)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [DelfStack: How to Import Multiple CSV Files Into Pandas and Concatenate Into One DataFrame] (https://www.delftstack.com/howto/python/read-multiple-csv-files-in-python/#:~:text=This%20tutorial%20demonstrates%20how%20to%20import)

#### For mean wind direction function:
- [Sling Academy: Fixing NumPy IndexError: Index is out of bounds for axis 0 with size N] (https://www.slingacademy.com/article/fixing-numpy-indexerror-index-out-of-bounds/?utm_content=cmp-true)
- [Stack Overflow: Python Index Error - Out of Bounds for axis 0] (https://stackoverflow.com/questions/66627017/python-index-error-out-of-bounds-for-axis-0)

#### For plotting histogram:
- [Plotting Histogram in Python using Matplotlib] (https://www.geeksforgeeks.org/plotting-histogram-in-python-using-matplotlib/)
- [Python KeyError: How to fix and avoid key errors] (https://www.learndatasci.com/solutions/python-keyerror/)
- [Stack Overflow: AttributeError: 'module' object has no attribute 'hist'] (https://stackoverflow.com/questions/29045636/attributeerror-module-object-has-no-attribute-hist)
- [Stack Overflow: Proper way to use **kwargs in Python] (https://stackoverflow.com/questions/1098549/proper-way-to-use-kwargs-in-python)

#### For suspect data:
- [Stack Overflow: TypeError: __call__() takes from 1 to 2 positional arguments but 3 were given] (https://stackoverflow.com/questions/63828474/typeerror-call-takes-from-1-to-2-positional-arguments-but-3-were-given)

#### For calculate averages:
- [Arithmetic-Geometric Mean] (https://mathworld.wolfram.com/Arithmetic-GeometricMean.html)

#### For invalid data:
- [Stack Overflow: Create bool mask from filter results in Pandas [duplicate]] (https://stackoverflow.com/questions/38802675/create-bool-mask-from-filter-results-in-pandas)
- [Stack Overflow: How to mask a list using boolean values from another list] (https://stackoverflow.com/questions/53527850/how-to-mask-a-list-using-boolean-values-from-another-list)

#### For site data:
- [Stack Overflow: Get a list from Pandas DataFrame column headers] (https://stackoverflow.com/questions/19482970/get-a-list-from-pandas-dataframe-column-headers)
- [Stack Overflow: ISO time (ISO 8601) in Python] (https://stackoverflow.com/questions/2150739/iso-time-iso-8601-in-python)
- [Stack Overflow: Working with mixed datetime formats in pandas [duplicate]] (https://stackoverflow.com/questions/60390709/working-with-mixed-datetime-formats-in-pandas)
- [Python Land: Python Try Except: Examples And Best Practices] (https://python.land/deep-dives/python-try-except)

#### For answer the question 1 and 2
- [Medium: Floating points in deep learning: Understanding the basics] (https://medium.com/@krinaljoshi/floating-points-in-deep-learning-understanding-the-basics-93459f77a266)
- [Python Data Types] (https://www.w3schools.com/python/python_datatypes.asp)

### Books

### Videos

### Chat GPT Sessions
#### For open and concatenate file:
- https://chatgpt.com/share/6705a2c2-882c-800a-b7c2-f626788604af

#### For plot histogram
- https://chatgpt.com/share/6707d3cb-6b28-800a-ba18-c5e3b6c785b1
- https://chatgpt.com/share/6707dbed-4458-800a-8163-861cd635ac00

#### For suspect data:
- https://chatgpt.com/share/6706f2d8-2fa8-800a-ada2-7748048a75ee

#### For weather_summaries
- https://chatgpt.com/share/67091917-e8a8-800a-82db-d1be49488222
- https://chatgpt.com/share/67091917-e8a8-800a-82db-d1be49488222

### Other AI Tools
#### For suspect data:
- Microsoft Copilot AI 
I asked Micorsoft Copilot AI to solve this problems below and try to applied it to my code'
IndexingError                             Traceback (most recent call last)
Cell In[167], line 19
     16 data = pd.read_excel('/home/zt24/numerical-programming-in-python/npp-pandas-assessment-esemsc-zt24/raw/merged_df.xlsx')
     17 sampel_data = pd.DataFrame(data)
---> 19 suspect_data(sampel_data)

Cell In[167], line 10, in suspect_data(dataframe)
      7 df_dewPoint['delta_dew_point'] = abs(df_dewPoint['dewPoint'] - df_dewPoint['expected_dew_point'])
      9 #Identify suspect data
---> 10 df_dewPoint['SuspectDataApplicable'] = df.loc[df_dewPoint['delta_dew_point'] > 0.2, 'No', 'Yes']
     11 df_dewPoint = df_dewPoint.filter(items=['dewPoint', 'expected_dew_point', 'delta_dew_point', 'SuspectDataApplicable'])
     13 return df_dewPoint

File ~/downloads/bash/envs/npp2024/lib/python3.12/site-packages/pandas/core/indexing.py:1184, in _LocationIndexer.__getitem__(self, key)
   1182     if self._is_scalar_access(key):
   1183         return self.obj._get_value(*key, takeable=self._takeable)
-> 1184     return self._getitem_tuple(key)
   1185 else:
   1186     # we by definition only have the 0th axis
   1187     axis = self.axis or 0

File ~/downloads/bash/envs/npp2024/lib/python3.12/site-packages/pandas/core/indexing.py:1371, in _LocIndexer._getitem_tuple(self, tup)
   1368     return self._getitem_lowerdim(tup)
   1370 # no multi-index, so validate all of the indexers
-> 1371 tup = self._validate_tuple_indexer(tup)
   1373 # ugly hack for GH #836
   1374 if self._multi_take_opportunity(tup):

File ~/downloads/bash/envs/npp2024/lib/python3.12/site-packages/pandas/core/indexing.py:962, in _LocationIndexer._validate_tuple_indexer(self, key)
    957 @final
    958 def _validate_tuple_indexer(self, key: tuple) -> tuple:
    959     \"\"\"
    960     Check the key for valid keys across my indexer.
    961     \"\"\"
--> 962     key = self._validate_key_length(key)
    963     key = self._expand_ellipsis(key)
    964     for i, k in enumerate(key)

File ~/downloads/bash/envs/npp2024/lib/python3.12/site-packages/pandas/core/indexing.py:1001, in _LocationIndexer._validate_key_length(self, key)
    999             raise IndexingError(_one_ellipsis_message)
   1000         return self._validate_key_length(key)
-> 1001     raise IndexingError(\"Too many indexers\")
   1002 return key

IndexingError: Too many indexers"
}

- Micorosoft Copilot AI
I asked to modify the code to show the plot of Dover Site and modify it

-Microsoft Copilot AI
I asked about the data types, modify, and rephrase it
- Microsot Copilot AI
I asked to check the grammar of my answer for question 1 and question 2