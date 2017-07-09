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

Took a break from the normal competitve coding. Instead made a python script / Mini project to download bing's image of the day and set it as my ubuntu wallpaper. View the code repository [here.](https://github.com/khannasarthak/daily-wallpaper-ubuntu16.04)

Learnt a lot of new things reagrding making os calls fro python, json fetching and handling path/ creating directories. 

The script and the code repository can be accessed [**here.**](https://github.com/khannasarthak/daily-wallpaper-ubuntu16.04)

Still have to make it run in the background like a service or as an independent daemon on my ubuntu 16.04. 

Will get back to normal questing solving tomorrow and work on trying to make this script better.


[198]: https://leetcode.com/problems/house-robber/#/description
[575]: https://leetcode.com/problems/distribute-candies/#/description