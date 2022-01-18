## Reconstructing Data

Explain what each line in the following short program does: what is in ```first```, ```second```, etc.?

```python
first = pd.read_csv('data/gapminder_all.csv', index_col='country')
second = first[first['continent'] == 'Americas']
third = second.drop('Puerto Rico')
fourth = third.drop('continent', axis = 1)
fourth.to_csv('result.csv')
```

<details>
  <summary>
Solution
  </summary>
  
Let’s go through this piece of code line by line.

  <b>Python</b>
  <pre>
first = pd.read_csv('data/gapminder_all.csv', index_col='country')
</pre>

This line loads the dataset containing the GDP data from all countries into a dataframe called <code>first</code>. The <code>index_col='country'</code> parameter selects which column to use as the row labels in the dataframe.

  <b>Python</b>
  <pre>
second = first[first['continent'] == 'Americas']
</pre>

  This line makes a selection: only those rows of <code>first</code> for which the ‘continent’ column matches ‘Americas’ are extracted. Notice how the Boolean expression inside the brackets, <code>first['continent'] == 'Americas'</code>, is used to select only those rows where the expression is true. Try printing this expression! Can you print also its individual True/False elements? (hint: first assign the expression to a variable)

  <b>Python</b>
  <pre>
third = second.drop('Puerto Rico')
</pre>

As the syntax suggests, this line drops the row from second where the label is ‘Puerto Rico’. The resulting dataframe third has one row less than the original dataframe second.

  <b>Python</b>
  <pre>
fourth = third.drop('continent', axis = 1)
</pre>

Again we apply the drop function, but in this case we are dropping not a row but a whole column. To accomplish this, we need to specify also the axis parameter (we want to drop the second column which has index 1).

  <b>Python</b>
  <pre>
fourth.to_csv('result.csv')
</pre>
  
The final step is to write the data that we have been working on to a csv file. Pandas makes this easy with the <code>to_csv()</code> function. The only required argument to the function is the filename. Note that the file will be written in the directory from which you started the Jupyter or Python session.
  
  </details>
  
 [Episode 2 Exercise 5](episode2_ex5.md)

