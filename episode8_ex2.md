## 8.2 Return versus print

Note that ```return``` and ```print``` are not interchangeable. ```print``` is a Python function that prints data to the screen. It enables us, users, see the data. ```return``` statement, on the other hand, makes data visible to the program. Let’s have a look at the following function:

```python
def add(a, b):
    print(a + b)
```

**Question:** What will we see if we execute the following commands?

```python
A = add(7, 3)
print(A)
```

<details>
  <summary>
    Solution
  </summary>

Python will first execute the function <code>add</code> with <code>a = 7</code> and <code>b = 3</code>, and, therefore, print <code>10</code>. However, because function <code>add</code> does not have a line that starts with <code>return</code> (no <code>return</code> “statement”), it will, by default, return nothing which, in Python world, is called <code>None</code>. Therefore, <code>A</code> will be assigned to <code>None</code> and the last line <code>(print(A))</code> will print <code>None</code>. As a result, we will see:

<pre>
10
None
</pre>
  
  </details>
  
  [Episode 8 exercise 3](episode8_ex3.md)
