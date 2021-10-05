
## 5.3 Computing Powers With Loops

Exponentiation is built into Python:

```python
print(5 ** 3)
```

```console
125
```

Write a loop that calculates the same result as ```5 ** 3``` using multiplication (and without exponentiation).

<details>
  <summary>
Solution
  </summary>

<pre>
result = 1
for number in range(0, 3):
  result = result * 5
print(result)
</pre>
  
</details>

[Episode 5 exercise 4](episode5_ex4.md)
