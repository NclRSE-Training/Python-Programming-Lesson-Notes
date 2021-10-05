## 7.5 In-Place Operators

Python (and most other languages in the C family) provides [in-place operators](https://swcarpentry.github.io/python-novice-inflammation/reference.html#in-place-operators) that work like this:

```python
x = 1  # original value
x += 1 # add one to x, assigning result back to x
x *= 3 # multiply x by 3
print(x)
```

```console
6
```

Write some code that sums the positive and negative numbers in a list separately, using in-place operators. Do you think the result is more or less readable than writing the same without in-place operators?

<details>
  <summary>
Solution
  </summary>

<pre>
positive_sum = 0
negative_sum = 0
test_list = [3, 4, 6, 1, -1, -5, 0, 7, -8]
for num in test_list:
    if num > 0:
        positive_sum += num
    elif num == 0:
        pass
    else:
        negative_sum += num
print(positive_sum, negative_sum)
</pre>

Here ```pass``` means “don’t do anything”. In this particular case, it’s not actually needed, since if ```num == 0``` neither sum needs to change, but it illustrates the use of ```elif``` and ```pass```.
</details>

[Episode 7 exercise 6](episode7_ex6.md)
