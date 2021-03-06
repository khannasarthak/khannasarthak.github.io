---
layout: post
title: Coding Practice 4
categories: coding
published: false
---

Solutions and notes on various questions from geekforgeeks and leetcode. 

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

	Implement the ```collections.Counter``` function yourself tomorrow. **DONE**
	```python
	a = string with elements
	c = {}
	for i in a:
		if i in c.keys():
			c[i]+=1
		else:
			c[i]= 1
	print (c)
	```

---
### **Day 24** [07/29]

**GeekforGeeks**:
* [move-all-zeroes-to-end-of-array](http://practice.geeksforgeeks.org/problems/move-all-zeroes-to-end-of-array/0)
* [inversion-of-array](http://practice.geeksforgeeks.org/problems/inversion-of-array/0)

	Did this using 2 for loops, however a O(nlogn) solution also exists, have a look at it. [Editorial](http://www.geeksforgeeks.org/counting-inversions/)
* [majority-element](http://practice.geeksforgeeks.org/problems/majority-element/0)

	I solved using hashmap, there are other methods too , but time complexity doesn't reduce to less than hash maps O(n). [Editorial](http://www.geeksforgeeks.org/majority-element/)

* [second-most-repeated-string-in-a-sequence](second-most-repeated-string-in-a-sequence)

* [pythagorean-triplet](http://practice.geeksforgeeks.org/problems/pythagorean-triplet/0)

	Have a look at the [Editorial] for O(n^2) solution, my solution was trivial O(n^3)

* [finding-the-numbers](http://practice.geeksforgeeks.org/problems/finding-the-numbers/0)

	[Editorial](http://www.geeksforgeeks.org/find-two-non-repeating-elements-in-an-array-of-repeating-elements/) using XOR, ive used hashing and counter.

* [reverse-words-in-a-given-string](http://practice.geeksforgeeks.org/problems/reverse-words-in-a-given-string/0)

* [roman-number-to-integer](http://practice.geeksforgeeks.org/problems/roman-number-to-integer/0)
		
	Had done this question on leetcode, so the code was much cleaner and faster now.

* [possible-words-from-phone-digits](http://practice.geeksforgeeks.org/problems/possible-words-from-phone-digits/0)

	My method was effectively the same, but i used itertools. [Editorial](http://www.geeksforgeeks.org/find-possible-words-phone-digits/) [Python2 solu, without itertools](http://ide.geeksforgeeks.org/CIvvfx)

	Learnt how to find combinations of a list of lists.
	```python
	s = ['abc','def','ghi']

	for combination in itertools.product(*s):	# if no *, then it has to be passes list by list, * passes it as a list of lists.
		op.append((''.join(combination)))
	```

---
### **Day 25** [07/30]:

**GeekforGeeks**:
* [sum-of-middle-elements-of-two-sorted-arrays](http://practice.geeksforgeeks.org/problems/sum-of-middle-elements-of-two-sorted-arrays/0)

	Pythonic solution faster than normal O(n) implementation in all cases. 
	```python
	O(n)
	while a and b:
		if a[0]<b[0]:
			op.append(a.pop(0))
		else:
			op.append(b.pop(0))

	-- Pytonic --
	op = a+b
	op.sort()
	```

* [equilibrium-point](http://practice.geeksforgeeks.org/problems/equilibrium-point/0)

* [sum-of-two-numbers-represented-as-arrays](http://practice.geeksforgeeks.org/problems/sum-of-two-numbers-represented-as-arrays/0)

	My solution does not change the arrays, however, another implementation : [Editorial](http://practice.geeksforgeeks.org/editorial.php?pid=506)

* [kth-distance](http://practice.geeksforgeeks.org/problems/kth-distance/0)
	
	Implemented O(kn) solution, however O(n) is also possible, [Editorial](http://www.geeksforgeeks.org/check-given-array-contains-duplicate-elements-within-k-distance/)

* [does-robot-moves-circular](http://practice.geeksforgeeks.org/problems/does-robot-moves-circular/0)

	Good question, wasnt able to figure it out, had to look at [editorial](http://www.geeksforgeeks.org/check-if-a-given-sequence-of-moves-for-a-robot-is-circular-or-not/) for a clear solution


---
### **Day 26** [08/04]:

Hardisk crashed, took time to recover and install the OS again. back to coding now. Never, gonna take a break unless absolutely necessary, makes it much difficult to get back and code. 

**GeekforGeeks**:
* [product-array-puzzle](http://practice.geeksforgeeks.org/problems/product-array-puzzle/0)

	The [editorial](http://www.geeksforgeeks.org/a-product-array-puzzle/) is quite different, using a right and left array. Space complexity is higher in mine. 

* [finding-number](http://practice.geeksforgeeks.org/problems/finding-number/0)
	
	[Editorial](http://www.geeksforgeeks.org/search-an-element-in-a-sorted-and-pivoted-array/). I figured the solution out, but took quite some time. Need to note this for future use. *Modified Binary Search for Bitonic Array*

---
### **Day 27** [08/05]:

**GeekforGeeks**:
* [count-number-of-ways-to-cover-a-distance](http://www.geeksforgeeks.org/count-number-of-ways-to-cover-a-distance/)

	Can be solved using DP, however , the question becomes an extended fibonacci seq. [DP editorial](http://www.geeksforgeeks.org/count-number-of-ways-to-cover-a-distance/)

* [minimum-element-in-a-sorted-and-rotated-array](http://practice.geeksforgeeks.org/problems/minimum-element-in-a-sorted-and-rotated-array/0)

	Similar to the modified binary search for a bitonic array. [Editorial](http://www.geeksforgeeks.org/find-minimum-element-in-a-sorted-and-rotated-array/)

* [maximum-repeating-number](http://practice.geeksforgeeks.org/problems/maximum-repeating-number/0)

	Tough question, involves a trick if has to be completed in O(1) space complexity. [Editorial](http://www.geeksforgeeks.org/find-the-maximum-repeating-number-in-ok-time/)

* [numbers-with-same-first-and-last-digit](http://practice.geeksforgeeks.org/problems/numbers-with-same-first-and-last-digit/0)

	My solution takes a lot of time, but doesnt TLE. The [Editorial](http://www.geeksforgeeks.org/count-numbers-first-last-digits/) is quite tricky, hard to come at.

---
### **Day 28** [08/06]:

**GeekforGeeks**:
* [floor-in-a-sorted-array](http://practice.geeksforgeeks.org/problems/floor-in-a-sorted-array/0)

	Getting a hang of binary search now, can easily spot questions where it will be used. Still i take time to figure the complete solution if its not a straightforward application. [Editorial](http://www.geeksforgeeks.org/floor-in-a-sorted-array/)

* [jumping-numbers](http://practice.geeksforgeeks.org/problems/jumping-numbers/0)

	Brute force solution giving TLE. The editorial uses BFS as shown [here.](http://practice.geeksforgeeks.org/problems/jumping-numbers/0)

* [key-pair](http://practice.geeksforgeeks.org/problems/key-pair/0)

	[Editorial](http://www.geeksforgeeks.org/write-a-c-program-that-given-a-set-a-of-n-numbers-and-another-number-x-determines-whether-or-not-there-exist-two-elements-in-s-whose-sum-is-exactly-x/) using hashmap.

* [convert-array-into-zig-zag-fashion](http://practice.geeksforgeeks.org/problems/convert-array-into-zig-zag-fashion/0)

	Good question, used modified bubble sort.

* [maximum-of-all-subarrays-of-size-k](http://practice.geeksforgeeks.org/problems/maximum-of-all-subarrays-of-size-k/0)

	