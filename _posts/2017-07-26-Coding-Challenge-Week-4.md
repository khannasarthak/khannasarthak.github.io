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
	
**Leetcode**:


