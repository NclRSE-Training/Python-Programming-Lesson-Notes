## Selection of Individual Values

Assume Pandas has been imported into your notebook and the Gapminder GDP data for Europe has been loaded:

**Python**

```python
import pandas as pd

df = pd.read_csv('data/gapminder_gdp_europe.csv', index_col='country')
```

Write an expression to find the Per Capita GDP of Serbia in 2007.

<details>
  <summary>
Solution
  </summary>

The selection can be done by using the labels for both the row (“Serbia”) and the column (“gdpPercap_2007”):

  <b>Python</b>
  <pre>
print(df.loc['Serbia', 'gdpPercap_2007'])
</pre>

  The output is
  
  <b>Output</b>
  
  <pre>
9786.534714
</pre>

</details>

[Expisode 2 Exercise 3](episode2_ex3.md)
