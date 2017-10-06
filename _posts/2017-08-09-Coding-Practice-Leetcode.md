---
layout: post
title: Coding Practice Leetcode
categories: coding
---

Solutions to various leetcode problems for my refernce. In no particular order. Look at notes on the leetcode website. 

---

[226. Invert Binary Tree](https://leetcode.com/problems/invert-binary-tree/description/)

[566. Reshape the Matrix](https://leetcode.com/problems/reshape-the-matrix/description/)
	
	Create a list of lists based on a particular size:
	```python
	Input: [1,2,3,4,5,6]

	i=0
	new_list=[]
	while i<len(data_list):
		new_list.append(data_list[i:i+3])
		i+=3

	Output: [[1,2,3],[4,5,6]]
	```

[168. Excel Sheet Column Title](https://leetcode.com/problems/excel-sheet-column-title/description/)

[561. Array Partition I](https://leetcode.com/problems/array-partition-i/description/)

Have to find a way without sorting, but other solution works for now.

[485. Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/description/)

[136. Single Number](https://leetcode.com/problems/single-number/description/)

	Remember bit manipulation ```a XOR a = 0, a XOR b XOR a = b```. Can be used to find single element if all others repeating 2 times.

[575. Distribute Candies](https://leetcode.com/problems/distribute-candies/discuss/)
	
	Remember to use logic and reasoning as well, solutions can be made much easier.

[349. Intersection of Two Arrays](https://leetcode.com/problems/intersection-of-two-arrays/description/)

[448. Find All Numbers Disappeared in an Array](https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/description/)

[169. Majority Element](https://leetcode.com/problems/majority-element/description/)
	
	Used [moore voting algo](https://en.wikipedia.org/wiki/Boyer%E2%80%93Moore_majority_vote_algorithm)

[217. Contains Duplicate](https://leetcode.com/problems/contains-duplicate/description/)

[268. Missing Number](https://leetcode.com/problems/missing-number/description/)

[283. Move Zeroes](https://leetcode.com/problems/move-zeroes/description/)

[409. Longest Palindrome](https://leetcode.com/problems/longest-palindrome/description/)

[122. Best Time to Buy and Sell Stock II](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii/description/)

[496. Next Greater Element I](https://leetcode.com/problems/next-greater-element-i/discuss/)

[350. Intersection of Two Arrays II](https://leetcode.com/problems/intersection-of-two-arrays-ii/description/)

	```python
	(list((Counter(nums1) & Counter(nums2)).elements()))
	```
	
	This basically checks if each elemt exists in both hash maps, and if they exits, gives true. Intersection with duplicates.
	```&``` is bitwise, checks if a and b both True. ```and``` checks if a and b are logically true.


[645. Set Mismatch](https://leetcode.com/problems/set-mismatch/description/)

