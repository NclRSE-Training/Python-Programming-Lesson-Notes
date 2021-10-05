## 7.6 Counting Vowels

1. Write a loop that counts the number of vowels in a character string.
1. Test it on a few individual words and full sentences.
1. Once you are done, compare your solution to your neighbor’s. Did you make the same decisions about how to handle the letter ‘y’ (which some people think is a vowel, and some do not)?

<details>
  <summary>
Solution
  </summary>

<pre>
vowels = 'aeiouAEIOU'
sentence = 'Mary had a little lamb.'
count = 0
for char in sentence:
    if char in vowels:
        count += 1

print('The number of vowels in this string is ' + str(count))
</pre>
  
  </details>
  
[Episode 8 exercise 1](episode8_ex1.md)
