## 5.1 From 1 to N

Python has a built-in function called ```range``` that generates a sequence of numbers. ```range``` can accept 1, 2, or 3 parameters.

If one parameter is given, ```range``` generates a sequence of that length, starting at zero and incrementing by 1. For example, ```range(3)``` produces the numbers ```0, 1, 2```.
If two parameters are given, ```range``` starts at the first and ends just before the second, incrementing by one. For example, ```range(2, 5)``` produces ```2, 3, 4```.
If ```range``` is given 3 parameters, it starts at the first one, ends just before the second one, and increments by the third one. For example, ```range(3, 10, 2)``` produces ```3, 5, 7, 9```.

Using ```range```, write a loop that uses ```range``` to print the first 3 natural numbers:

```python
1
2
3
```

<details>
<summary>
Solution
</summary>

<pre>
for number in range(1, 4):
  print(number)
</pre>

</details>

[Episode 5 exercise 2](episode5_ex2.md)
