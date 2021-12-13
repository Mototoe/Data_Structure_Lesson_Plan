# Linkined Lists 
## &ensp; Definition
&emsp;&emsp; A linked list is a more complicated data structure then the previous reviewed data structure. This data structure consit of linking nodes of data to each other. we are able to do this becasue a node consist of 2 things, which are data and a address to direct teh data. This means that it not only contains data but directs it too. There are 2 versioinas of this data structure, there is a singly linked list and doublt linked list. The big difference betwwen the two is that one has 2 address on it so it allows for the data to be sent forward and backwards. To do that we take avntage of the next and prev terms. The figure below will provide the concept behind a linked list. Linked lists can be used to help maintain directorys of names.
![image](https://user-images.githubusercontent.com/83718823/145895618-77932b3f-4ad7-4047-a031-9081a4d04202.png)
## &ensp; Singly Effectivnes and Example 
&ensp;&emsp; A benifit of useing singly linked list is that is it can be a little more efficent since the nodes only have one pointer. That also means a lot less code. Its effectivness is O(1) when editing and O(n) in the worst case when searhing through it. To navigate, add, or substract from the singly linked list you use the next to impplemnt the address fo teh nod and were you are connecting it moving forward. A good example of this the diagram below.
![image](https://user-images.githubusercontent.com/83718823/145897433-64a725af-d757-457c-9763-701997c5a5bd.png)
### &ensp;&emsp; Code Example:
```python
def _init_(self, value=none, xt_node=None):
        self.value = value
        self.next_node = next_node
```

## &ensp; Doubly Effectivness and Example 
![145900335-c141a7db-e35a-44ab-a84f-82adb2d1f5bc](https://user-images.githubusercontent.com/83718823/145900343-80090889-2364-4486-a355-bee2d980c706.png)
