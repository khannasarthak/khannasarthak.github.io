---
layout: post
title: Coding Practice CTCI 
categories: coding
---

### Chapter 1: Arrays and Strings

Will be posting my solutions in python here and also and notes / comments.

---

**1.1 Is Unique:**

Implement an algorithm to determine if a string has all unique characters. What if you cannot use additional data structures?

```python
from collections import Counter

def isUnique(s):
	flag = False
	c = Counter(s)
	for i in c:
		if c[i]>1:
			flag =  False
		else:
			flag = True
	return flag
```


**1.2 Check Permutation:**

Given two strings, write a method to decide if one is a permutation of the other.

```python
def isPermu(a,b):
	if len(a)!=len(b):
		return False
	else:
		if len(a)==len(b):
			if list((set(a)-set(b))) ==[]:
				return True

```


**1.3 URLify:** 

Write a method to replace all spaces in a string with '%20'.

```python
def url(a):
	k = a.split()
	op = []
	for i in k:
		if i!=' ':
			op.append(i)
	return '%20'.join(op)

print ((url(a)))
```

Use ```split()``` to remove single spaces and extra whitespacing, then use ```join``` to join the string with space replaced with ```%20```.

**1.4 Palindrome Permutation:**: 

Given a string, write a function to check if it is a permutation of a palindrome.

```python
from collections import Counter

a = 'azAZ' # string to test on

def pp(s):
	s = s.lower()
	s = ''.join(s.split())
	c = Counter(s)
	f = False
	count = 0
	for i in c:
		if c[i]%2==1:
			count+=1
	if count==1 or count==0:
		f = True
	# print (count)
	return f

print (pp(a))
```

A good resource with all the implemented methods : [Leetcode Article](https://leetcode.com/articles/palindrome-permutation/#approach-2-using-hashmap-accepted)

