---
layout: post
title: Coding Challenge Week One
categories: coding
---

Code everyday for atleast 4 hours doing questions from leet code, geek for geeks or algorithmic implementations. This will be a sort of personal blog writing my daily progress and if possible waka time images. Also, start another post for helpful python tips that I can refer later on.

**GOALS**
* 150 Leet code problems (34/150) 



---
### **Day 0** [06/30]

* Leetcode [30] : 557, 500, 561, 506

The questions were good, learnt a few new tricks using dictionaries. Feels good to start coding again after a long break. 

506:
```python
new_dict = dict(zip(key,value))
print (list(map(dik.get, nums))) # where nums can be a list of keys, and this returns values  
```

500:
```python
new_list = list1 + list2 # not a deep copy.
```

---
### **Day 1** [07/01]

* Leetcode [32] : 169, 520

Spent a lot of time studying binary trees and their implementationsin pyhton, thats why wasnt able to do much of leet code. 

169:
```python
from collections import Counter
count = Counter(nums)
k= (count.most_common()[0])	# returns the 1st [0th] most common element in the list
```
Collections is a lot faster than making and dictionary and checking key value pairs explicitly. *most_common()* is a great way of finding out the most common (high frequency) elements in a pyhton list

---
### **Day 2** [07/02]

* Leetcode [34] : 263, 347

347:
```python
from collections import Counter
class Solution(object):
    def topKFrequent(self, nums, k):       
        count = Counter(nums)
        return ((zip(*count.most_common(k)))[0]) 
```
Without zip, the solution was getting timed out for 1 test case. Zip function could be used to extract the first item from the tuple. 
```
	Eg: nums = [1,1,1,2,2,2,3,3,3], k = 3
	count.most_common(k) gives [(1, 3), (2, 3), (3, 3)]
	list(zip(*count.most_common(k))) gives [(1, 2, 3), (3, 3, 3)], keys in first list and values in second list
	list(zip(*count.most_common(k)))[0] gives just the first list of keys, ie. (1,2,3)
```

Have to code more, and make the linux desktop library / tool as well.

