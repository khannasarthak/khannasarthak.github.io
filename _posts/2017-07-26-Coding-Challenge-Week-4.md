---
layout: post
title: Coding Challenge Week 4
categories: coding
---

Code everyday for atleast 4 hours doing questions from leet code, geek for geeks or algorithmic implementations. This will be a sort of personal blog writing my daily progress and if possible waka time images. Also, start another post for helpful python tips that I can refer later on.

**GOALS**
* 150 Leet code problems (42/150) 



---
### **Day 22** [07/26]

**GeekforGeeks**:
* [greater-on-right-side](http://practice.geeksforgeeks.org/problems/greater-on-right-side/0)

	Quicker [solution](http://www.geeksforgeeks.org/replace-every-element-with-the-greatest-on-right-side/). However, the runtime's are comparable, as my initial solution used max.
	
* [maximum-value-in-a-bitonic-array](http://practice.geeksforgeeks.org/problems/maximum-value-in-a-bitonic-array/0)

	Used Modified Binary search. [Editorial](http://www.geeksforgeeks.org/find-the-maximum-element-in-an-array-which-is-first-increasing-and-then-decreasing/)
		
* [magic-number](http://practice.geeksforgeeks.org/problems/magic-number/0)

	Involvede a trick of sorts, given [here](http://www.geeksforgeeks.org/find-nth-magic-number/)

* [element-that-appears-once-where-every-element-occurs-twice](http://practice.geeksforgeeks.org/problems/element-that-appears-once-where-every-element-occurs-twice/0)
		
	Nice question, used ```eval``` and join to do XOR of all. 
	```python
	a = '4^5^4'
	b = '2+2'

	Use eval to execute the string
	print (eval(a)) --> 5
	print (eval(b)) --> 4
	```

* [finding-position](http://practice.geeksforgeeks.org/problems/finding-position/0)

	No need to use recursion, the actual will be the highest power of 2 lower than n. Took time to figure this out.
	

---
### **Day 23** [07/27]

**GeekforGeeks**:
* [facing-the-sun](http://practice.geeksforgeeks.org/problems/facing-the-sun/0)

* [save-knights](http://practice.geeksforgeeks.org/problems/save-knights/0)

	Involves a trick. from n>=3 the chess board looks like:
	```
	3X3
	K - K
	- K -
	K - K

	4X4
	K - K -
	- K - K
	K - K -
	- K - K
	```
	And this pattern continues.

* [next-sparse-binary-number](http://practice.geeksforgeeks.org/problems/next-sparse-binary-number/0)

	My solution was O(nlogn), however a O(n) solution also exists. [Editorial](http://www.geeksforgeeks.org/given-a-number-find-next-sparse-number/)

* [extract-maximum](http://practice.geeksforgeeks.org/problems/extract-maximum/0)

	Used Regex. NOTE: While using regex in python, use ```re.findall``` and not ```re.matches```, the first one gives direct answer, whereas matches gives a matched group, which have to be accessed using ```groups()```

* [k-anagrams-1](http://practice.geeksforgeeks.org/problems/k-anagrams-1/0)

	Created a dictionary, also, if we sort a word then its arranged in increasing order so we can compare if 2 anagrams of the same word are actually anagrams or not. [Reference: Ans2 ](https://stackoverflow.com/questions/8286554/using-python-find-anagrams-for-a-list-of-words)

	Adding new vallue for a particular key in a dictionary.
	```python
	d[key]=(w.count(key))
	```
	Getting all values in a dictionary
	```python
	d.values()
	```

* [reverse-each-word-in-a-given-string](http://practice.geeksforgeeks.org/problems/reverse-each-word-in-a-given-string/0)
* [number-of-groups](http://practice.geeksforgeeks.org/problems/number-of-groups/0)

	Had already done this question earlier, so it was easier to implement. Used Combinations and modulus. [Editorial](http://www.geeksforgeeks.org/number-groups-sizes-two-three-divisible-3/)

* [non-repeating-character](http://practice.geeksforgeeks.org/problems/non-repeating-character/0)

	Implement the ```collections.Counter``` function yourself tomorrow.

---
### **Day 24** [07/29]

**GeekforGeeks**:
* [move-all-zeroes-to-end-of-array](http://practice.geeksforgeeks.org/problems/move-all-zeroes-to-end-of-array/0)
* [inversion-of-array](http://practice.geeksforgeeks.org/problems/inversion-of-array/0)

	Did this using 2 for loops, however a O(nlogn) solution also exists, have a look at it. [Editorial](http://www.geeksforgeeks.org/counting-inversions/)
* [majority-element](http://practice.geeksforgeeks.org/problems/majority-element/0)

	I solved using hashmap, there are other methods too , but time complexity doesn't reduce to less than hash maps O(n). [Editorial](http://www.geeksforgeeks.org/majority-element/)

* []()