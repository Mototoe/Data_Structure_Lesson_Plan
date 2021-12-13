# Linkined Lists 
## &ensp; Definition
&emsp;&emsp; A linked list is a more complicated data structure then the previous reviewed data structure. This data structure consit of linking nodes of data to each other. we are able to do this becasue a node consist of 2 things, which are data and a address to direct teh data. This means that it not only contains data but directs it too. There are 2 versioinas of this data structure, there is a singly linked list and doublt linked list. The big difference betwwen the two is that one has 2 address on it so it allows for the data to be sent forward and backwards. To do that we take avntage of the next and prev terms. The figure below will provide the concept behind a linked list. Linked lists can be used to help maintain directorys of names and can impitate a stack and queue when its more covientent 
![image](https://user-images.githubusercontent.com/83718823/145895618-77932b3f-4ad7-4047-a031-9081a4d04202.png)
## &ensp; Singly Effectivnes and Example 
&ensp;&emsp; A benifit of useing singly linked list is that is it can be a little more efficent since the nodes only have one pointer. That also means a lot less code. Its effectivness is O(1) when editing and O(n) in the worst case when searhing through it. To navigate, add, or substract from the singly linked list you use the next to impplemnt the address fo teh nod and were you are connecting it moving forward. A good example of this the diagram below.
![image](https://user-images.githubusercontent.com/83718823/145897433-64a725af-d757-457c-9763-701997c5a5bd.png)
### &ensp;&emsp; Code Example:
```python
def _init_(self, value=none, next_node=None):
        self.value = value
        self.next_node = next_node
```

## &ensp; Doubly Effectivness and Example 
&ensp;&emsp; The doubly linked list has many benifits that are not possible with singly. One big advantage is being able to insert in the middle of a link list. The doubly linked lis is more flexible and usble becasue it allows the nodes to have 2 addressess to assign. This allows for data to be passed back and forth, but because of this extra address potential it uses up a little more memory. With that to add on to one of the sides it is O(1) but if you need to insert in the middle it goes to O(n). It is also O(n) whne searching through the douply linked list. Continuing with singly linked list you only really need the next pointe, with doubly you next and prev pointer sto be able to successfully create it. A good example of these pointers are shown in th first diagram in the lesson. TO help understand the doubly linked list oyu can think of a train becasue with each cart you have to attach or deatach both locks between the carts.
![DpkR1M8WwAEGRsw](https://user-images.githubusercontent.com/83718823/145902956-f66ca997-5cf5-47ce-93a0-1a45b866e000.jpg)
### &ensp;&emsp; Code Example:
```python
'''Node class represents
a node of the list'''
class Node:
        def _iit_
(self, value) :
self. value
= value
self.next = None
CircularLinkedList class represents the circular linked list'
class CircularLinkedList:
def
-
init
(self):
self.tail = None
"'Returns True if the list is empty (so self.tail = None)
Otherwise, returns False'
def list is empty(self):
return not self.tail
if
name
==
main
1•
-
my_list = circularLinkedList()
print(f"My list is Empty? {my_list.list is empty()}")
# Mv list is Empty? True
```
