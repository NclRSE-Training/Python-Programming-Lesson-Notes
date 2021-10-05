## 5.5 Computing the Value of a Polynomial

The built-in function enumerate takes a sequence (e.g. a list) and generates a new sequence of the same length. Each element of the new sequence is a pair composed of the index (0, 1, 2,…) and the value from the original sequence:

```python
for idx, val in enumerate(a_list):
  # Do something using idx and val
  ```

The code above loops through ```a_list```, assigning the index to ```idx``` and the value to ```val```.

Suppose you have encoded a polynomial as a list of coefficients in the following way: the first element is the constant term, the second element is the coefficient of the linear term, the third is the coefficient of the quadratic term, etc.

```python
x = 5
coefs = [2, 4, 3]
y = coefs[0] * x**0 + coefs[1] * x**1 + coefs[2] * x**2
print(y)
```

```console
97
```

Write a loop using ```enumerate(coefs)``` which computes the value ```y``` of any polynomial, given ```x``` and ```coefs```.

<details>
  <summary>
Solution
  </summary>
    
  <pre>
y = 0
for idx, coef in enumerate(coefs):
y = y + coef * x**idx
</pre>
  
  </details>
  
  [Episode 6 exercise 1](episode6_ex1.md)
