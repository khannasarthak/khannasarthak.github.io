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
* [number-of-paths](http://practice.geeksforgeeks.org/problems/number-of-paths/0)
	
	**Dynamic problem or recursion**, kinda tough to understand , need to do more of such kinds. 

	Reference: [One](http://algorithms.tutorialhorizon.com/dynamic-programming-count-all-paths-from-top-left-to-bottom-right-of-a-mxn-matrix/)
	, [Two](http://www.geeksforgeeks.org/count-possible-paths-top-left-bottom-right-nxm-matrix/), [Three](http://algorithms.tutorialhorizon.com/print-all-paths-from-top-left-to-bottom-right-in-two-dimensional-array/)

* [count-zero](http://practice.geeksforgeeks.org/problems/count-zero/0)	

	Dont always think about CS, use simple concepts of PnC, like in this question. Read question and try if you can use PnC, makes the question easier to solve

---
### **Day 16** [07/18]

Missed a day due to travelling. Back at home now, can starting working properly again. 

My site started having loads of issues today, even though I didnt do any changes. Was able to fix the problems ( css not loading, and baseurl errors) by creating a new ```baseurl``` variable equivalent and using that every where instead. Took some time to figure it out. 
