## Correlations

Modify the example in the notes to create a scatter plot showing the relationship between the minimum and maximum GDP per capita among the countries in Asia for each year in the data set. What relationship do you see (if any)?

## Solution 1

```python
data_asia = pd.read_csv('data/gapminder_gdp_asia.csv', index_col='country')
data_asia.describe().T.plot(kind='scatter', x='min', y='max')
```

![Correlations Solution 1](https://nclrse-training.github.io/python-novice/fig/9_correlations_solution1.svg)

No particular correlations can be seen between the minimum and maximum gdp values year on year. It seems the fortunes of asian countries do not rise and fall together.

***

You might note that the variability in the maximum is much higher than that of the minimum. Take a look at the maximum and the max indexes:

```python
data_asia = pd.read_csv('data/gapminder_gdp_asia.csv', index_col='country')
data_asia.max().plot()
print(data_asia.idxmax())
print(data_asia.idxmin())
```

## Solution 2

![Correlations Solution 2](https://nclrse-training.github.io/python-novice/fig/9_correlations_solution2.png)

Seems the variability in this value is due to a sharp drop after 1972. Some geopolitics at play perhaps? Given the dominance of oil producing countries, maybe the Brent crude index would make an interesting 

[Episode 3 Exercise 3](episode3_ex3.md)
