---
layout: post
title: Coding Challenge Week One
categories: coding
---

Code everyday for atleast 4 hours doing questions from leet code, geek for geeks or algorithmic implementations. This will be a sort of personal blog writing my daily progress and if possible waka time images. Also, start another post for helpful python tips that I can refer later on.

**GOALS**
* 150 Leet code problems (32/150) 



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

### **Day 2** [07/02]

* Leetcode [32] : 169, 520


Will keep updating it daily as things go on.