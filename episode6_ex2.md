## 6.2 Minimum File Size

Modify this program so that it prints the number of records in the file that has the fewest records.

```python
import glob
import pandas as pd
fewest = ____
for filename in glob.glob('data/*.csv'):
  dataframe = pd.____(filename)
  fewest = min(____, dataframe.shape[0])
print('smallest file has', fewest, 'records')
```

Note that the ```DataFrame.shape()``` method returns a tuple with the number of rows and columns of the data frame.

<details>
  <summary>
Solution
  </summary>
  
  <pre>
import glob
import pandas as pd
fewest = float('Inf')
for filename in glob.glob('data/*.csv'):
  dataframe = pd.read_csv(filename)
  fewest = min(fewest, dataframe.shape[0])
print('smallest file has', fewest, 'records')
</pre>
  
  </details>
  
  [Episode 6 exercise 3](episode6_ex3.md)
