
## 4.3 Overloading

```+``` usually means addition, but when used on strings or lists, it means “concatenate”. Given that, what do you think the multiplication operator ```*``` does on lists? In particular, what will be the output of the following code?

```python
counts = [2, 4, 6, 8, 10]
repeats = counts * 2
print(repeats)
```

1. ```[2, 4, 6, 8, 10, 2, 4, 6, 8, 10]```
1. ```[4, 8, 12, 16, 20]```
1. ```[[2, 4, 6, 8, 10],[2, 4, 6, 8, 10]]```
1. ```[2, 4, 6, 8, 10, 4, 8, 12, 16, 20]```

The technical term for this is operator overloading: a single operator, like ```+``` or ```*```, can do different things depending on what it’s applied to.

<details>
<summary>
Solution
</summary>

The multiplication operator ```*``` used on a list replicates elements of the list and concatenates them together:
<br/>
<code>
[2, 4, 6, 8, 10, 2, 4, 6, 8, 10]
</code>
<br/>
It’s equivalent to:
<br/>
<code>
counts + counts
</code>
<details>

[Episode 5 exercise 1](episode5_ex1.md)
