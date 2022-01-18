## Slicing Strings

A section of an array is called a ```slice```. We can take slices of character strings as well:

```python
element = 'oxygen'
print('first three characters:', element[0:3])
print('last three characters:', element[3:6])
```

**Output**
```output
first three characters: oxy
last three characters: gen
```

What is the value of ```element[:4]```? What about ```element[4:]```? Or ```element[:]```?

<details>
  <summary>
    Solution
  </summary>

  <b>Output</b>
  <pre>
oxyg
en
oxygen
</pre>

</details>

[Episode 2 Exercise 2](episode2_ex2.md)
