---
layout: post
title: Coding Practice Leetcode
categories: coding
---

Solutions to various leetcode problems for my refernce. In no particular order. Look at notes on the leetcode website. 

*Italicised Questions are important*

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

[628. Maximum Product of Three Numbers](https://leetcode.com/problems/maximum-product-of-three-numbers/description/)

[167. Two Sum II - Input array is sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/description/)

[35. Search Insert Position](https://leetcode.com/problems/search-insert-position/description/)

[594. Longest Harmonious Subsequence](https://leetcode.com/problems/longest-harmonious-subsequence/description/)

[674. Longest Continuous Increasing Subsequence](https://leetcode.com/problems/longest-continuous-increasing-subsequence/description/)

[1. Two Sum](https://leetcode.com/problems/two-sum/description/)

[*26. Remove Duplicates from Sorted Array*](https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/)

[14. Longest Common Prefix](https://leetcode.com/problems/longest-common-prefix/description/)

[189. Rotate Array](https://leetcode.com/problems/rotate-array/description/)

[461. Hamming Distance](https://leetcode.com/problems/hamming-distance/description/)

[557. Reverse Words in a String III](https://leetcode.com/problems/reverse-words-in-a-string-iii/description/)

[500. Keyboard Row](https://leetcode.com/problems/keyboard-row/description/)

[657. Judge Route Circle](https://leetcode.com/problems/judge-route-circle/description/)

[476. Number Complement](https://leetcode.com/problems/number-complement/description/)

[412. Fizz Buzz](https://leetcode.com/problems/fizz-buzz/description/)

[682. Baseball Game](https://leetcode.com/problems/baseball-game/description/)

[693. Binary Number with Alternating Bits](https://leetcode.com/problems/binary-number-with-alternating-bits/description/)

[520. Detect Capital](https://leetcode.com/problems/detect-capital/description/)

[258. Add Digits](https://leetcode.com/problems/add-digits/description/)

[387. First Unique Character in a String](https://leetcode.com/problems/first-unique-character-in-a-string/description/)

[242. Valid Anagram](https://leetcode.com/problems/valid-anagram/description/)

[599. Minimum Index Sum of Two Lists](https://leetcode.com/problems/minimum-index-sum-of-two-lists/description/)

[551. Student Attendance Record I](https://leetcode.com/problems/student-attendance-record-i/description/)

[504. Base 7](https://leetcode.com/problems/base-7/discuss/)

[389. Find the Difference](https://leetcode.com/problems/find-the-difference/description/)

[342. Power of Four](https://leetcode.com/problems/power-of-four/description/)

[13. Roman to Integer](https://leetcode.com/problems/roman-to-integer/description/)

[70. Climbing Stairs](https://leetcode.com/problems/climbing-stairs/description/)

[231. Power of Two](https://leetcode.com/problems/power-of-two/description/)

[326. Power of Three](https://leetcode.com/problems/power-of-three/description/)

[434. Number of Segments in a String](https://leetcode.com/problems/number-of-segments-in-a-string/description/)

[263. Ugly Number](https://leetcode.com/problems/ugly-number/description/)

[643. Maximum Average Subarray I](https://leetcode.com/problems/maximum-average-subarray-i/description/)

[172. Factorial Trailing Zeroes](https://leetcode.com/problems/factorial-trailing-zeroes/description/)

[118. Pascal's Triangle](https://leetcode.com/problems/pascals-triangle/description/)

[119. Pascal's Triangle II](https://leetcode.com/problems/pascals-triangle-ii/description/)

[383. Ransom Note](https://leetcode.com/problems/ransom-note/discuss/)

[292. Nim Game](https://leetcode.com/problems/nim-game/description/)

[168. Excel Sheet Column Title](https://leetcode.com/problems/excel-sheet-column-title/discuss/)

[171. Excel Sheet Column Number](https://leetcode.com/problems/excel-sheet-column-number/discuss/)

[202. Happy Number](https://leetcode.com/problems/happy-number/description/)

[506. Relative Ranks](https://leetcode.com/problems/relative-ranks/description/)

[121. Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/description/)

[27. Remove Element](https://leetcode.com/problems/remove-element/description/)

[9. Palindrome Number](https://leetcode.com/problems/palindrome-number/description/)

[125. Valid Palindrome](https://leetcode.com/problems/valid-palindrome/description/)

[7. Reverse Integer](https://leetcode.com/problems/reverse-integer/description/)

[190. Reverse Bits](https://leetcode.com/problems/reverse-bits/description/)

[414. Third Maximum Number](https://leetcode.com/problems/third-maximum-number/description/)

[20. Valid Parentheses](https://leetcode.com/problems/valid-parentheses/discuss/)

[507. Perfect Number](https://leetcode.com/problems/perfect-number/description/)

[442. Find All Duplicates in an Array](https://leetcode.com/problems/find-all-duplicates-in-an-array/description/)

[540. Single Element in a Sorted Array](https://leetcode.com/problems/single-element-in-a-sorted-array/discuss/)

[495. Teemo Attacking](https://leetcode.com/problems/teemo-attacking/description/)

[347. Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements/discuss/)

[345. Reverse Vowels of a String](https://leetcode.com/problems/reverse-vowels-of-a-string/description/)

[58. Length of Last Word](https://leetcode.com/problems/length-of-last-word/description/)

[633. Sum of Square Numbers](https://leetcode.com/problems/sum-of-square-numbers/description/)

[717. 1-bit and 2-bit Characters](https://leetcode.com/problems/1-bit-and-2-bit-characters/description/)

[492. Construct the Rectangle](https://leetcode.com/problems/construct-the-rectangle/discuss/)

[581. Shortest Unsorted Continuous Subarray](https://leetcode.com/problems/shortest-unsorted-continuous-subarray/description/)

[686. Repeated String Match](https://leetcode.com/problems/repeated-string-match/description/)

[205. Isomorphic Strings](https://leetcode.com/problems/isomorphic-strings/description/)

[290. Word Pattern](https://leetcode.com/problems/word-pattern/description/)











