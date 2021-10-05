## 7.1 How Many Paths?

Consider this code:

```python
if 4 > 5:
    print('A')
elif 4 == 5:
    print('B')
elif 4 < 5:
    print('C')
```

Which of the following would be printed if you were to run this code? Why did you pick this answer?

1. A
1. B
1. C
1. B and C

<details>
  <summary>
    Solution
  </summary>

  C gets printed because the first two conditions, <code>4 > 5</code> and <code>4 == 5</code>, are not true, but <code>4 < 5</code> is true.

  </details>
  
  [Episode 7 exercise 2](episode7_ex2.md)
