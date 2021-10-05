
## 4.1 Slicing From the End

Use slicing to access only the last four characters of a string or entries of a list.

```python
string_for_slicing = 'Observation date: 02-Feb-2013'
list_for_slicing =  [['fluorine', 'F'],
                    ['chlorine', 'Cl'],
                    ['bromine', 'Br'],
                    ['iodine', 'I'],
                    ['astatine', 'At']]
```

```console
'2013'
[['chlorine', 'Cl'], ['bromine', 'Br'], ['iodine', 'I'], ['astatine', 'At']]
```

Would your solution work regardless of whether you knew beforehand the length of the string or list (e.g. if you wanted to apply the solution to a set of lists of different lengths)? If not, try to change your approach to make it more robust.

Hint: Remember that indices can be negative as well as positive

<details>
  <summary>
Solution
  </summary>

Use negative indices to count elements from the end of a container (such as list or string):

  <code>
string_for_slicing[-4:]
list_for_slicing[-4:]
  </code>
</details>

[Episode 4 exercise 2](episode4_ex2.md)
