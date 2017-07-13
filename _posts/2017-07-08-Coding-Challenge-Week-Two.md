---
layout: post
title: Coding Challenge Week Two
categories: coding
---

Code everyday for atleast 4 hours doing questions from leet code, geek for geeks or algorithmic implementations. This will be a sort of personal blog writing my daily progress and if possible waka time images. Also, start another post for helpful python tips that I can refer later on.

**GOALS**
* 150 Leet code problems (42/150) 



---
### **Day 8** [07/08]

**Leetcode:** [198], [575]

198:

Similar to dynamic programming problem done yesterday. Need to study more DP.

**GeekforGeeks**:
* [permutations-of-a-given-string](http://practice.geeksforgeeks.org/problems/permutations-of-a-given-string/0)

Try to do this without itertools and use backtracking. [Refer this](http://www.geeksforgeeks.org/write-a-c-program-to-print-all-permutations-of-a-given-string/)

* [find-first-and-last-occurrence-of-x](http://practice.geeksforgeeks.org/problems/find-first-and-last-occurrence-of-x/0)

Good question , learnt a new way to find all indices of an element in list
```python

n = int(input())
indices = [i for i, x in enumerate(k) if x == n]    # n is the element whose indices are being found
```

* [k-largest-elements](http://practice.geeksforgeeks.org/problems/k-largest-elements/0)
* [rotate-array-by-n-elements](http://practice.geeksforgeeks.org/problems/rotate-array-by-n-elements/0)
* [value-equal-to-index-value](http://practice.geeksforgeeks.org/problems/value-equal-to-index-value/0)

Have to start doing CTCI and backtracking. Also, work on the linux script to send updates on the desktop automatically.

---
### **Day 9** [07/09]

Took a break from the normal competitve coding. Instead **made a python script / Mini project to download bing's image of the day and set it as my ubuntu wallpaper**. View the code repository [here.](https://github.com/khannasarthak/daily-wallpaper-ubuntu16.04)

Learnt a lot of new things reagrding making os calls fro python, json fetching and handling path/ creating directories. 

The script and the code repository can be accessed [**here.**](https://github.com/khannasarthak/daily-wallpaper-ubuntu16.04)

Still have to make it run in the background like a service or as an independent daemon on my ubuntu 16.04. 

Will get back to normal questing solving tomorrow and work on trying to make this script better.

---
### **Day 10** [07/10]

Played around with the script I made yesterday, was unable to run it on a virtual machine running ubuntu 16.04.2, will have to try and figure out why it wasn't working. 

**GeekforGeeks**:
* [number-of-occurrence](http://practice.geeksforgeeks.org/problems/number-of-occurrence/0)
* [reverse-sub-array](http://practice.geeksforgeeks.org/problems/reverse-sub-array/0)
* [remove-character](http://practice.geeksforgeeks.org/problems/remove-character/0)

Used the concept i had used in an earlier question to delete the element in place. 
```python
# have to delete characters in s2 from s1. All occurances
k = list(s1)	
n = list(s2)
for i in n:
	k[:] = ([x for x in k if x != i])	# Deletes in place
```
Decision to keep a note of important code snippets is proving to be helpful.

* [maximum-product-of-two-numbers](http://practice.geeksforgeeks.org/problems/maximum-product-of-two-numbers/0)

Have to try and solve it in O(n) time, currently it is O(nlogn) due to the sorting step. O(n) solution for reference can be found [**here**](http://www.geeksforgeeks.org/return-a-pair-with-maximum-product-in-array-of-integers/)

---
### **Day 11** [07/12]

Was busy travelling yesterday, couldn't code much. Did a few problems. 

**GeekforGeeks**:
* [find-first-set-bit](http://practice.geeksforgeeks.org/problems/find-first-set-bit/0)

Used python's string formating here to get binary representation of the number.
```python
k =  ((format((a),'b'))) # a is the decimal number , 'b' for binary
```	
Another way to do this is by using bit manipulation given [**here**](http://www.geeksforgeeks.org/position-of-rightmost-set-bit/)

* [minimum-difference-pair](http://practice.geeksforgeeks.org/problems/minimum-difference-pair/0)
* [bit-difference](http://practice.geeksforgeeks.org/problems/bit-difference/0)

String formatting again and then keeping a fixed value for the binary numbers. A good question.
```python
	a1 = str(format(a,'08b'))	# Converts to bainry number, if length > 8 then shows more characters anyways
	b1 = str(format(b,'08b'))

	a1 = a1.zfill(20)	# to make both of the numbers of same size
	b1 = b1.zfill(20)
	

	for i,j in zip(a1,b1): # to iterate and compare both lists
		if i!=j:
			c += 1
```

---
### **Day 12** [07/13]


**GeekforGeeks**:
* [keypad-typing](http://practice.geeksforgeeks.org/problems/keypad-typing/0)
* [count-total-set-bits](http://practice.geeksforgeeks.org/problems/count-total-set-bits/0)

Easy if implemented using inbuilt ```bin()``` function, however it can be doe by finding a pattern in the bits of odd numbers, solution can be found [**here.**](http://practice.geeksforgeeks.org/editorial.php?pid=500)

* [generate-binary-numbers](http://practice.geeksforgeeks.org/problems/generate-binary-numbers/0)

Another interesting way to do it is using queue, as shown [**here.**](http://www.geeksforgeeks.org/interesting-method-generate-binary-numbers-1-n/)

* [type-of-array](http://practice.geeksforgeeks.org/problems/type-of-array/0)

Used sort and did, time complexity is O(nlogn), however it can be done using recursion in O(n) the solution is [**here.**](http://www.geeksforgeeks.org/type-array-maximum-element/)

* [twice-counter](http://practice.geeksforgeeks.org/problems/twice-counter/0)
* [unique-numbers](http://practice.geeksforgeeks.org/problems/unique-numbers/0)






[198]: https://leetcode.com/problems/house-robber/#/description
[575]: https://leetcode.com/problems/distribute-candies/#/description