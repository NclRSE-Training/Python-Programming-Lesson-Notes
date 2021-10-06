## 6.3 Comparing Data

Write a program that reads in the regional data sets and plots the average GDP per capita for each region over time in a single chart.

<details>
  <summary>
    Solution
  </summary>

  This solution builds a useful legend by using the string <code>split</code> method to extract the <code>region</code> from the path ‘data/gapminder_gdp_a_specific_region.csv’.

  <pre>
import glob
import pandas as pd
import matplotlib.pyplot as plt
fig, ax = plt.subplots(1,1)
for filename in glob.glob('data/gapminder_gdp*.csv'):
    dataframe = pd.read_csv(filename)
    # extract {region} from the filename, expected to be in the format 'data/gapminder_gdp_{region}.csv'.
    # we will split the string using the split method and `_` as our separator,
    # retrieve the last string in the list that split returns (`{region}.csv`), 
    # and then remove the `.csv` extension from that string.
    region = filename.split('_')[-1][:-4] 
    dataframe.mean().plot(ax=ax, label=region)
plt.legend()
plt.show()
</pre>

</details>

[Episode 7 exercise 1](episode7_ex1.md)
