## 8.1 Combining Strings

“Adding” two strings produces their concatenation: ```'a' + 'b'``` is ```'ab'```. Write a function called ```fence``` that takes two parameters called ```original``` and ```wrapper``` and returns a new string that has the wrapper character at the beginning and end of the original. A call to your function should look like this:

```python
print(fence('name', '*'))
```

```console
*name*
```

<details>
  <summary>
    Solution
  </summary>

<pre>
def fence(original, wrapper):
  return wrapper + original + wrapper
</pre>
 
</details>

[Episode 8 exercise 2](episode8_ex2.md)
