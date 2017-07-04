---
layout: post
title: Coding Challenge Week One
categories: coding
---

Code everyday for atleast 4 hours doing questions from leet code, geek for geeks or algorithmic implementations. This will be a sort of personal blog writing my daily progress and if possible waka time images. Also, start another post for helpful python tips that I can refer later on.

**GOALS**
* 150 Leet code problems (42/150) 



---
### **Day 0** [06/30]

* Leetcode [30] : [557], [500], [561], [506]

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

* Leetcode [32] : [169], [520]

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

* Leetcode [34] : [263], [347]

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


---
### **Day 3** [07/03]

* Leetcode [39] : [268], [326], [35], [551], [70]

326:
```python
if n==0:
    return False
else:
    while n!=1:
        if n%3==0:
            n = n//3
        else:
            return False
            break
    return (True)
```
Another solution without using loops / recursion:
```python
return (n > 0 == 3**19 % n)
```
The explanations [stackoverflow](https://stackoverflow.com/questions/1804311/how-to-check-if-an-integer-is-a-power-of-3/24274850#24274850) and [leetcode](https://leetcode.com/articles/power-of-three/)

The positive divisors of 3^19 are exactly the powers of 3 from 3^0 to 3^19. That's all powers of 3 in the possible range here (signed 32-bit integer). So just check whether the number is positive and whether it divides 3^19.

551:
```python
a_count = s.count('A')
# print (a_count)
lll_count = s.count('LLL')
if a_count >1 or lll_count>0:
    return False
else:
    return True
```
Have to try this problem with regular expressions.

---
### **Day 4** [07/03]

* Leetcode [42] : [264(TLE)], [27], [593]

264:
The algorithm is correct, but the question time complexity needs to be reduced by using Dynamic Programming, which I havent done much yet. Will try it again once ive dont some questions of dynamic.








[557]: https://leetcode.com/problems/reverse-words-in-a-string-iii/#/description
[500]: https://leetcode.com/problems/keyboard-row/#/description
[561]: https://leetcode.com/problems/array-partition-i/#/description
[506]: https://leetcode.com/problems/relative-ranks/#/description
[169]: https://leetcode.com/problems/majority-element/#/description
[520]: https://leetcode.com/problems/detect-capital/#/description
[263]: https://leetcode.com/problems/ugly-number/#/description
[347]: https://leetcode.com/problems/top-k-frequent-elements/#/description
[268]: https://leetcode.com/problems/missing-number/#/description
[326]: https://leetcode.com/problems/power-of-three/#/description
[35]: https://leetcode.com/problems/search-insert-position/#/description
[551]: https://leetcode.com/problems/student-attendance-record-i/#/description
[70]: https://leetcode.com/problems/climbing-stairs/#/description
[264(TLE)]: https://leetcode.com/problems/ugly-number-ii
[27]: https://leetcode.com/problems/remove-element/#/description
[593]:https://leetcode.com/problems/valid-square/#/description


