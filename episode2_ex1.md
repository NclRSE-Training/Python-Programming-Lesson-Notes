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

What is ```element[-1]```? What is ```element[-2]```?

<details>
  <summary>
Solution
  </summary>
  <b>Output</b>
  
  <pre>
n
e
</pre>
</details>  

Given those answers, explain what ```element[1:-1]``` does.
<details>
  <summary>
Solution
  </summary>

  <pre>
Creates a substring from index 1 up to (not including) the final index, effectively removing the first and last letters from ‘oxygen’
</pre>
  </details>
  
  
How can we rewrite the slice for getting the last three characters of ```element```, so that it works even if we assign a different string to ```element```? Test your solution with the following strings: ```carpentry```, ```clone```, ```hi```.

<details>
  <summary>
Solution
  </summary>

  <b>Python</b>
  <pre>
element = 'oxygen'
print('last three characters:', element[-3:])
element = 'carpentry'
print('last three characters:', element[-3:])
element = 'clone'
print('last three characters:', element[-3:])
element = 'hi'
print('last three characters:', element[-3:])
</pre>
  
  <b>Output</b>
  </pre>
last three characters: gen
last three characters: try
last three characters: one
last three characters: hi
</pre>
</details>



[Episode 2 Exercise 2](episode2_ex2.md)
