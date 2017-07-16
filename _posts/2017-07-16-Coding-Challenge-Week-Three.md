---
layout: post
title: Coding Challenge Week Three
categories: coding
---

Code everyday for atleast 4 hours doing questions from leet code, geek for geeks or algorithmic implementations. This will be a sort of personal blog writing my daily progress and if possible waka time images. Also, start another post for helpful python tips that I can refer later on.

**GOALS**
* 150 Leet code problems (42/150) 



---
### **Day 15** [07/16]

**GeekforGeeks**:
* [ways-to-tile-a-floor](http://practice.geeksforgeeks.org/problems/ways-to-tile-a-floor/00)

	Used fibonacci series, also learnt of a new method to non recursively calculate fib(n)
	```python
	fibo=[0,1]
	for i in range (n):
		fibo.append(fibo[-1]+fibo[-2])

	print (fibo) # gives the whole list, with the indexes acting like keys in a dictionary
	```

