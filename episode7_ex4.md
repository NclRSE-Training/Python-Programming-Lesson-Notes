## 7.4 Close Enough

Write some conditions that print True if the variable a is within 10% of the variable b and False otherwise. Compare your implementation with your partner’s: do you get the same answer for all possible pairs of numbers?

### Hint

There is a built-in function ```abs``` that returns the absolute value of a number:

```python
    print(abs(-12))
```

```console
    12
```

<details>
  <summary>
    Solution 1
  </summary>
    
<pre>
a = 5
b = 5.1

if abs(a - b) <= 0.1 * abs(b):
    print('True')
else:
    print('False')
</pre>
    
</details>
  
<details>
    <summary>
    Solution 2
    </summary>

<pre>
print(abs(a - b) <= 0.1 * abs(b))
</pre>

This works because the Booleans True and False have string representations which can be printed.
</details>
    
[Episode 7 exercise 5](episode7_ex5.md)
