# Calculate-Maximum-Text-Value
You are given a text of single- space separated words, consisting of small and capital Latin letters.    Value of the word is number of capital letters in the word.  Value of the text is maximum volume of all words in the text.    Calculate the Value of the given text.

n = int(input())
text = input()
words = text.split()
max_count = 0
for word in words:
    count = sum(1 for char in word if char.isupper())
    max_count = max(max_count, count)
print(max_count)
