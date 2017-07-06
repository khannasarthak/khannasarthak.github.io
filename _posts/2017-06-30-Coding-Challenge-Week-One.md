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
### **Day 4** [07/04]

* Leetcode [42] : [264(TLE)], [27], [593]

264:

The algorithm is correct, but the question time complexity needs to be reduced by using Dynamic Programming, which I havent done much yet. Will try it again once ive dont some questions of dynamic.

27:
```python
class Solution(object):
    def removeElement(self, nums, val):
        nums[:] = ([x for x in nums if x != val])   # Deletes in place and replaces all instances of nums
        return (len(nums))
```
Use this to delete elements in place, nums is the list and val has to be deleted. 
If we use nums instead of nums[:], then the previous instances wont get updated. See example below. [Reference.](https://stackoverflow.com/questions/2186656/how-can-i-remove-all-instances-of-an-element-from-a-list-in-python)
```
just a
a = [1]; b = a;
 now a = [2]; b == [1];
with a[:]  
a = [1]; b = a; 
a[:] = [2]; b == [2], b also gets updated
```

593:

NEVER USE under root for distance, just keep everything in square. 2^(0.5) makes things very very difficult with the extra precision. ALWAYS DRAW THE FIGURE AND DESGIN THE ALGORITHM. [Reference](http://www.geeksforgeeks.org/check-given-four-points-form-square/)

Try to solve this using itertools and combinations: 
```python
class Solution(object):
def validSquare(self, p1, p2, p3, p4):
    def D((P, Q)):
        return (P[0] - Q[0]) ** 2 + (P[1] - Q[1]) ** 2
    S = set(map(D, itertools.combinations((p1, p2, p3, p4), 2)))
    return len(S) == 2 and 0 not in S
```

Need to buck up and increase the pace at which im solving, by A LOT!

---
### **Day 5** [07/05]

Didn't do leet code, instead started with geekforgeeks amazon company questions, will mix these two up. Did 4 questions and learnt a new method to slice list into various ways.

Geekforgeeks: 
* [maximum-money:](http://practice.geeksforgeeks.org/problems/maximum-money/0)
* [check-if-given-four-points-form-a-square:](http://practice.geeksforgeeks.org/problems/check-if-given-four-points-form-a-square/0)
* [equal-to-product:](http://practice.geeksforgeeks.org/problems/equal-to-product/0)

Have to try and do this in less than n^2 complexity, using binary search would make it nlogn, is there anything better?

* [student-record:](http://practice.geeksforgeeks.org/problems/student-record/0):

The code used here is very useful and can be reused in various questions.
```python
names  =  [x for x in a if x.isalpha()] # creates a list out of a which just gives names. a is the original list here

scores = [x for x in a if x.isalpha()==False]

k = [scores[i:i+3] for i in range(0, len(scores), 3)] #VERY IMP, creates a new list k containing elements as sublist from the original list

#EG:
list = [1,2,3,4,5,6,7,8,9]
k = [list[i:i+3] for i in range(0, len(list), 3)]
k = [[1,2,3],[4,5,6],[7,8,9]]
```

Will code from g4g and leetcode both tomorrow, and also have to start reading CTCI!

---
### **Day 6** [07/06]

Did quite a lot of coding today. Have to keep increasing my pace.

Leetcode: [58], [66]

Have to read about split() function properly, need to understand how and what does it do. 

Geekforgeeks:
* [check-set-bits](http://practice.geeksforgeeks.org/problems/check-set-bits/0)
* [uncommon-characters](http://practice.geeksforgeeks.org/problems/uncommon-characters/0)

How to find that some element from list bexists in list a or not.
```python
k1 = [item for item in b if item not in a]
```

* [check-if-string-is-rotated-by-two-places](http://practice.geeksforgeeks.org/problems/check-if-string-is-rotated-by-two-places/0)

Rotating a string:
```python
a[i:]+a[:i]
i is positive for right shift and negative for left shift
```

* [overlapping-rectangles](http://practice.geeksforgeeks.org/problems/overlapping-rectangles/0)

A very good question, difficult to solve without knowledge of the concept. Readings: [First Source](https://stackoverflow.com/questions/13390333/two-rectangles-intersection) , [Second Source](https://stackoverflow.com/questions/306316/determine-if-two-rectangles-overlap-each-other)

* [immediate-smaller-element](http://practice.geeksforgeeks.org/problems/immediate-smaller-element/0)
* [replace-all-0-with-5-in-an-input-integer](http://practice.geeksforgeeks.org/problems/replace-all-0-with-5-in-an-input-integer/1)

How to replace an element with another in a list:
```python
myl = list(str(n))

new_items = [x if (x != '0') else '5' for x in myl] 

# [x if (condition) else <New Value> for x in list]

k = int(''.join(map(str,new_items)))  # convert a str list to string

```

Today was quite productive, have to keep working harder!




















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
[58]: https://leetcode.com/problems/length-of-last-word/#/description
[66]: https://leetcode.com/problems/plus-one/#/description


