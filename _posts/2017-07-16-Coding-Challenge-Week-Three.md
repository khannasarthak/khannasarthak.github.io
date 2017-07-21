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
### **Day 16** [07/19]

Missed a day due to travelling. Back at home now, can starting working properly again. 

My site started having loads of issues today, even though I didnt do any changes. Was able to fix the problems ( css not loading, and baseurl errors) by creating a new ```baseurl``` variable equivalent and using that every where instead. Took some time to figure it out. 

**GeekforGeeks**:
* [array-of-alternate-ve-and-ve-nos](http://practice.geeksforgeeks.org/problems/array-of-alternate-ve-and-ve-nos/0)
	
	Iterate through 2 lists, however the length of new list is dependent on the smaller list.
	
	```python
	for i,j in zip(pos,neg):
		new.append(i)
		new.append(j)
	```
	For example:
	```
	pos = [1,2,3]
	neg= [-2,-3]
	new = [1,2,-2,-3]
	```
	Therefore, use with caution and make sure to take the extra elements from longer list into account.

* [count-the-elements **DO AGAIN IN LESS TIME**](http://practice.geeksforgeeks.org/problems/count-the-elements/0)
	
	Solution needs a O(n) solution, however I could only come up with a O(n^2) solution as of now. Learnt a few new things:

	To create a list of keys with no values, where keys are from a list do the following:
	```python
	a = [1,2,3]
	op = {key: None for key in a}
	```

	And to get values from a dictionary as a list:
	```python
	k = list(dictname.values())
	```

	*DICTIONARIES ARE NOT ORDERED, IF YOU GET VALUES FROM THEM, THEY WILL BE IN RANDOM ORDER. DICTIONARY IS AS GOOD AS A HASH TABLE*

	Still have to attemp and do this question in O(n^2) as given [**here.**](http://practice.geeksforgeeks.org/editorial.php?pid=2087) 	


---
### **Day 17** [07/20]

**GeekforGeeks**:
* [check-if-a-number-can-be-expressed-as-xy](http://practice.geeksforgeeks.org/problems/check-if-a-number-can-be-expressed-as-xy/0)
	
	Easy questions, just need to take care of log in python for numbers like 27,243 and so on. *USE LOG10 for all purposes.*
	```
	k = math.log10(27)/math.log10(3)
	ans = 3
	AND NOT

	k = math.log(27)/math.log(3)
	ans = 2.9999
	```
	This leads to rounding problems.

* [pairs-of-prime-number](http://practice.geeksforgeeks.org/problems/pairs-of-prime-number/0)

	Tough question, still needs to be optimized. [Generate prime numbers till n](https://stackoverflow.com/questions/11619942/print-series-of-prime-numbers-in-python) :
	```python
	for num in range(1,n):
    if all(num%i!=0 for i in range(2,int((num**0.5))+1,2)):
       op.append(int(num))
	```
	[Editorial](http://www.geeksforgeeks.org/find-two-prime-numbers-with-given-sum/)

* [geek-and-coffee-shop](http://practice.geeksforgeeks.org/problems/geek-and-coffee-shop/0)
* [count-possible-triangles](http://practice.geeksforgeeks.org/problems/count-possible-triangles/0)
	
	First solved using simple brute force in O(n^3), however can be reduced to O(n^2) by a trick given [**here**](http://www.geeksforgeeks.org/find-number-of-triangles-possible/)

* [possible-groups](http://practice.geeksforgeeks.org/problems/possible-groups/0)
	
	Can be brute forced, but takes O(n^3), a smarter trick can get it done in O(n) using simple PnC ad dictionaries. [**Editorial**](http://www.geeksforgeeks.org/count-possible-groups-size-2-3-sum-multiple-3/)
	```
	using nC3 and nC2 to find the groups. i.e Combinations
	```
* [boolean-matrix-problem](http://practice.geeksforgeeks.org/problems/boolean-matrix-problem/0)

	Had to *convert a single list into a matrix*, code might be useful later. [Refernce](http://www.geeksforgeeks.org/a-boolean-matrix-question/) for later
	```python
	m = [1,2,3,4,5,6,7,8,9] # list

	r,c = 3,4 # row and column

	while m!= []:
		k.append(m[:c])
		m = m[c:] 

	print (k)	# k is a 2D array / matrix
	```
* [count-substrings](http://practice.geeksforgeeks.org/problems/count-substrings/0)
* [single-number](http://practice.geeksforgeeks.org/problems/single-number/0)
	Use XOR to find single number
	```
	a^a = 0
	a^b^a=b
	```
* [reverse-bits](http://practice.geeksforgeeks.org/problems/reverse-bits/0)
	To convert dec to bin :
	```python
	b = str(format(n,'b'))
	```
	To convert bin to dec:
	```python
	d - int(b,2)
	```
	*DONT FORGET ZFILL to padd extra 0's* ```binary.zfill(32)``` to convert to 32 bit.



---
### **Day 18** [07/21]

**GeekforGeeks**:
* [index-of-first-1-in-a-sorted-array-of-0s-and-1s](http://practice.geeksforgeeks.org/problems/index-of-first-1-in-a-sorted-array-of-0s-and-1s/0)


 [**Crypto Currency Desktop Notifier**](https://github.com/khannasarthak/python-cryptomoney)

	Created a mini project using python on ubuntu, used json , currency API's and used the unix scheduler **cron** to run the script repeatedly at a given time.

[**Wallpaper Changer**](https://github.com/khannasarthak/daily-wallpaper-ubuntu16.04)

	Updated the code and enabled the script to run on startup, was missing the permission changes ```chmod +x filename.py``` in the startup application in ubuntu. However, it only works if the file is on the desktop, still have to figure out why it doesnt work if kept inside folders even when all folders are made chmod +x.

Will study tree's do Leetcode, geekforgeeks questions on it tomorrow.