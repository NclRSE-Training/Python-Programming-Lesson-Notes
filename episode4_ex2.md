## 4.2 Non-Continuous Slices

So far we’ve seen how to use slicing to take single blocks of successive entries from a sequence. But what if we want to take a subset of entries that aren’t next to each other in the sequence?

You can achieve this by providing a third argument to the range within the brackets, called the step size. The example below shows how you can take every third entry in a list:

```python
primes = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37]
subset = primes[0:12:3]
print('subset', subset)
```

```console
subset [2, 7, 17, 29]
```

Notice that the slice taken begins with the first entry in the range, followed by entries taken at equally-spaced intervals (the steps) thereafter. If you wanted to begin the subset with the third entry, you would need to specify that as the starting point of the sliced range:

```python
primes = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37]
subset = primes[2:12:3]
print('subset', subset)
```

```console
subset [5, 13, 23, 37]
```

Use the step size argument to create a new string that contains only every other character in the string “In an octopus’s garden in the shade”. Start with creating a variable to hold the string:

```python
beatles = "In an octopus's garden in the shade"
```

What slice of beatles will produce the following output (i.e., the first character, third character, and every other character through the end of the string)?

```console
I notpssgre ntesae
```

<details>
  <summary>
Solution
  </summary>

To obtain every other character you need to provide a slice with the step size of 2:

beatles[0:35:2]

You can also leave out the beginning and end of the slice to take the whole string and provide only the step argument to go every second element:

beatles[::2]

If you want to take a slice from the beginning of a sequence, you can omit the first index in the range:

date = 'Monday 4 January 2016'
day = date[0:6]
print('Using 0 to begin range:', day)
day = date[:6]
print('Omitting beginning index:', day)

Using 0 to begin range: Monday
Omitting beginning index: Monday

And similarly, you can omit the ending index in the range to take a slice to the very end of the sequence:

months = ['jan', 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov', 'dec']
sond = months[8:12]
print('With known last position:', sond)
sond = months[8:len(months)]
print('Using len() to get last entry:', sond)
sond = months[8:]
print('Omitting ending index:', sond)

With known last position: ['sep', 'oct', 'nov', 'dec']
Using len() to get last entry: ['sep', 'oct', 'nov', 'dec']
Omitting ending index: ['sep', 'oct', 'nov', 'dec']

  
  </details>
  
  [Episode 4 exercise 3](episode4_ex3.md)
