---
layout: post
title: Binary Trees
categories: coding
---

My learning progress on trees. Will upgrade with code snippets and how they are implemented in code.

---

* Create a basic binary tree

```python
class Node:
	def __init__(self,key):	# Initialises instance of class or object
		self.left = None	# Left child
		self.right = None	# Right child
		self.val = key 		# Value
```
[Stackoverflow answer for what __init__ does.](https://stackoverflow.com/questions/8609153/why-do-we-use-init-in-python-classes)

Now, each node can have more nodes below it, called children.

```python
root = Node(1)			# Root node
root.left = Node(2)		# Left child with value 2
root.right = Node(3)	# Right child with value 3
# Tree formed :
#	1
#  / \
# 2   3
```
This is just the creation of binary trees, the next main part is the traversal, which can be done in multiple ways, namely, DFS and BFS.

---
* Depth First Search (DFS)




---


Will keep updating it daily as things go on.