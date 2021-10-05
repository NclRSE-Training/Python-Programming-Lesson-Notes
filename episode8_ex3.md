## 8.3 Selecting Characters From Strings

If the variable ```s``` refers to a string, then ```s[0]``` is the string’s first character and ```s[-1]``` is its last. Write a function called ```outer``` that returns a string made up of just the first and last characters of its input. A call to your function should look like this:

```python
print(outer('helium'))
```

```console
hm
```

<details>
  <summary>
    Solution
  </summary>

<pre>
def outer(input_string):
    return input_string[0] + input_string[-1]
</pre>
  
  </details>
  
[Episode 8 exercise 4](episode8_ex4.md)
