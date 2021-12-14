# Trees
## &ensp; Definition
&ensp;&emsp; A lot like linked list that were taught prior, a tree is a data structure that uses pointers and nodes to connect data together and organize it for later use. The prime difference is that trees unlike linked list can connect to multiple different nodes. There are 2 main tree data structures, which are binary tree amd binary search tree. But a tree has more than just nodes, for example there is the root which is the start opf the tree. Then there is the parent and child nodes that apear in a tree when a node is connnected to other nodes. The nodes that are at th bottom or end doing that dont have connected nodes are called leaves. If you look below you can find a more visual concept of these things. Trees can be super usdeful for storing data amd reading through it to find things in relation slike search bars and their filter are a good example of what trees are good for. Moving back to the binary tree, it is a tree that links no more thatn 2 nodes to the root or parent nodes. The binary search tree is similar to the binary tree in structual design being that they both can only have 2 nodes connected, but the binary search tree respects the valuses and rules of the data being put into the tree and keeps the tree balanced. Another thing that is importatnt to know about trees is the hieght of the tre based on the root or parent node. This is calculated based on the count down of nodes from teh startiung node. Glancing at teh diagram below it's hight is 4 from A.

&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;&emsp;&ensp;![image](https://user-images.githubusercontent.com/83718823/145931121-178fc454-7f66-4cda-a4b8-ceb0d1c14825.png)

## &ensp; Tree Efficency and Example
 &ensp;&emsp; The tree data structure tends to be on of the more effective data structures taht we revieved although they were used for slightly different reasons. This is thanks to how we searsh for information through this datat structure. The principople we us is recursion, this is a methood of looping through all of a data structure from leaft to right. This method allows tree data structure to be able to reach a constant O(log n), which the only big O notation that is better is o(1). Although there are exceptions to tree data structures thatt are not balenced.  This means the binary search trees are O(log n), but it is not the case for the binary trees. To clarify teh binary are more effective but takes more to code, while the binary trees  are a little less effiecent but easier to implement.

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
##Practice Problems
### &ensp; Problem 1
&ensp;&emsp; This problem will help you to understand how to insert values into the tree data strucrture.
```python
class binary_tree:

    def __init__(self, value):

        self.left = None
        self.right = None
        self.value = value

    def insert(self, value):
        #insert value into the tree
        pass
    def print_tree(self):
        if self.left:
            self.left.print_tree()
        print( self.data),
        if self.right:
            self.right.print_tree()

root = binary_tree(100)
root.insert(50)
root.insert(55)
root.insert(60)
root.insert(20)
root.insert(52)
root.PrintTree()
```
### Problem 2
