# Trees
## &ensp; Definition
&ensp;&emsp;  A lot like the linked list that was taught prior, a tree is a data structure that uses pointers and nodes to connect data together and organize it for later use. The prime difference is that trees unlike linked lists it can connect to multiple different nodes. There are 2 main tree data structures, which are binary tree and binary search tree. But a tree has more than just nodes, for example, there is the root which is the start of the tree. Then there are the parent and child nodes that appear in a tree when a node is connected to other nodes. The nodes that are at the bottom or end doing that don't have connected nodes are called leaves. If you look below you can find a more visual concept of these things. Trees can be super useful for storing data and reading through it to find things in relation like search bars and their filter are good examples of what trees are good for. Moving back to the binary tree, it is a tree that links no more than 2 nodes to the root or parent nodes. The binary search tree is similar to the binary tree in structural design being that they both can only have 2 nodes connected, but the binary search tree respects the values and rules of the data being put into the tree and keeps the tree balanced. Another thing that is important to know about trees is the height of the tree based on the root or parent node. This is calculated based on the count down of nodes from the starting node. Glancing at the diagram below its height is 4 from A.

&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;![image](https://user-images.githubusercontent.com/83718823/145931121-178fc454-7f66-4cda-a4b8-ceb0d1c14825.png)

## &ensp; Tree Efficency and Example
 &ensp;&emsp; The tree data structure tends to be one of the more effective data structures that we reviewed although they were used for slightly different reasons. This is thanks to how we search for information through this data structure. The principle we use is recursion, this is a method of looping through all of a data structure from left to right. This method allows tree data structure to be able to reach a constant O(log n), which the only big O notation that is better is o(1). Although there are exceptions to tree data structures that are not balanced.  This means the binary search trees are O(log n), but it is not the case for the binary trees. To clarify the binary are more effective but takes more to code, while the binary trees are a little less efficient but easier to implement.

![indirect1](https://user-images.githubusercontent.com/83718823/145931162-c52c6e51-b81b-440d-a636-a455b6c2a1f8.jpg)

### &ensp;&emsp; Code Example:
```python
class Node:
   def __init__(self, data):
      self.left = None
      self.right = None
      self.data = data
   def P_Tree(self):
      print(self.data)

root = Node(10)
root.P_Tree()
```
## Practice Problems
### &ensp; Problem 1
&ensp;&emsp; This problem will help you to understand how to insert values into the tree data strucrture.
```python
class binary_tree:

    def __init__(self, value):

        self.left = None
        self.right = None
        self.value = value

    def insert(self, value):
        #Insert values into the tree
        pass
    def print_tree(self):
        #traverse the tree and print it in order
        pass

root = binary_tree(100)
root.insert(50)
root.insert(55)
root.insert(60)
root.insert(20)
root.insert(52)


root.print_tree()
```
### &ensp; Problem 2
&ensp;&emsp; In this problem we will be continueing the code made early and traversing it to print them in order
```python
class binary_tree:

    def __init__(self, value):

        self.left = None
        self.right = None
        self.value = value

    def insert(self, value):

        if self.value:
            if value < self.value:
                if self.left is None:
                    self.left = binary_tree(value)
                else:
                    self.left.insert(value)
            elif value > self.value:
                if self.right is None:
                    self.right = binary_tree(value)
                else:
                    self.right.insert(value)
        else:
            self.value = value

    def print_tree(self):
        #traverse the tree and print it in order
        pass

root = binary_tree(100)
root.insert(50)
root.insert(55)
root.insert(60)
root.insert(20)
root.insert(52)
root.print_tree()

```
### &ensp; Solution 1
```python
class binary_tree:

    def __init__(self, value):

        self.left = None
        self.right = None
        self.value = value

    def insert(self, value):

        if self.value:
            if value < self.value:
                if self.left is None:
                    self.left = binary_tree(value)
                else:
                    self.left.insert(value)
            elif value > self.value:
                if self.right is None:
                    self.right = binary_tree(value)
                else:
                    self.right.insert(value)
        else:
            self.value = value

    def print_tree(self):
        #traverse the tree and print values in order
        pass

root = binary_tree(100)
root.insert(50)
root.insert(55)
root.insert(60)
root.insert(20)
root.insert(52)
root.print_tree()
```
### &ensp; Solution 2
```python 
class binary_tree:

    def __init__(self, value):

        self.left = None
        self.right = None
        self.value = value

    def insert(self, value):

        if self.value:
            if value < self.value:
                if self.left is None:
                    self.left = binary_tree(value)
                else:
                    self.left.insert(value)
            elif value > self.value:
                if self.right is None:
                    self.right = binary_tree(value)
                else:
                    self.right.insert(value)
        else:
            self.value = value

    def print_tree(self):
        if self.left:
            self.left.print_tree()
        print( self.value),
        if self.right:
            self.right.print_tree()

root = binary_tree(100)
root.insert(50)
root.insert(55)
root.insert(60)
root.insert(20)
root.insert(52)
root.print_tree()

```
