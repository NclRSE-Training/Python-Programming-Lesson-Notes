## Selecting Indices

Explain in simple terms what ```idxmin``` and ```idxmax``` do in the short program below. When would you use these methods?

```python
data = pd.read_csv('data/gapminder_gdp_europe.csv', index_col='country')
print(data.idxmin())
print(data.idxmax())
```

<details>
  <summary>
Solution
  </summary>

For each column in <code>data</code>, <code>idxmin</code> will return the index value corresponding to each column’s minimum; idxmax will do accordingly the same for each column’s maximum value.

You can use these functions whenever you want to get the row index of the minimum/maximum value and not the actual minimum/maximum value.

</details>

[Episode 2 Exercise 6](episode2_ex6.md)
