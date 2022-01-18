## Sorting Out References

Python allows you to assign multiple values to multiple variables in one line by separating the variables and values with commas. What does the following program print out?

```python
first, second = 'Grace', 'Hopper'
third, fourth = second, first
print(third, fourth)
```

<details>
  <summary>
        Solution
  </summary>
  
**Output**
  <pre>
        Hopper Grace
</pre>
  </details>
