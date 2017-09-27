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

[https://leetcode.com/problems/excel-sheet-column-title/description/](https://leetcode.com/problems/excel-sheet-column-title/description/)

[561. Array Partition I](https://leetcode.com/problems/array-partition-i/description/)

Have to find a way without sorting, but other solution works for now.

[485. Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/description/)

[136. Single Number](https://leetcode.com/problems/single-number/description/)

	Remember bit manipulation ```a XOR a = 0, a XOR b XOR a = b```. Can be used to find single element if all others repeating 2 times.

[575. Distribute Candies](https://leetcode.com/problems/distribute-candies/discuss/)
	
	Remember to use logic and reasoning as well, solutions can be made much easier.
.




