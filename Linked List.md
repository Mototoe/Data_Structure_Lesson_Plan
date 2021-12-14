# Linked Lists 
## &ensp; Definition
&emsp;&emsp; A linked list is a more complicated data structure than the previously reviewed data structure. This data structure consists of linking nodes of data to each other. we are able to do this because a node consists of 2 things, which are data and an address to direct the data. This means that it not only contains data but directs it too. There are 2 versions of this data structure, there is a singly linked list and a doubly linked list. The big difference between the two is that one has 2 addresses on it so it allows for the data to be sent forward and backward. To do that we take advantage of the next and prev terms. The figure below will provide the concept behind a linked list. Linked lists can be used to help maintain directories of names and can implicate a stack and queue when its more convenient 
![image](https://user-images.githubusercontent.com/83718823/145895618-77932b3f-4ad7-4047-a031-9081a4d04202.png)
## &ensp; Singly Effectivnes and Example 
&ensp;&emsp; A benefit of using a singly linked list is that is it can be a little more efficient since the nodes only have one pointer. That also means a lot less code. Its effectiveness is O(1) when editing an O(n) in the worst case when searching through it. To navigate, add, or subtract from the singly linked list you use the next to implement the address for the nod and where you are connecting it moving forward. A good example of this is the diagram below.
![image](https://user-images.githubusercontent.com/83718823/145897433-64a725af-d757-457c-9763-701997c5a5bd.png)
### &ensp;&emsp; Code Example:
```python
def _init_(self, value=none, next_node=None):
        self.value = value
        self.next_node = next_node
```

## &ensp; Doubly Effectivness and Example 
&ensp;&emsp; The doubly linked list has many benefits that are not possible singly. One big advantage is being able to insert in the middle of a link list. The doubly linked list is more flexible and usable because it allows the nodes to have 2 addresses to assign. This allows for data to be passed back and forth, but because of this extra address potential, it uses up a little more memory. With that to add on to one of the sides, it is O(1) but if you need to insert it in the middle it goes to O(n). It is also O(n) when searching through the doubly linked list. Continuing with the singly linked list you only really need the next pointer, with doubly you need the next and prev pointer to be able to successfully create it. A good example of these pointers is shown in the first diagram in the lesson. TO help understand the doubly linked list you can think of a train because with each cart you have to attach or detach both sides between the carts.
![DpkR1M8WwAEGRsw](https://user-images.githubusercontent.com/83718823/145902956-f66ca997-5cf5-47ce-93a0-1a45b866e000.jpg)
### &ensp;&emsp; Code Example:
```python

class Node:
        def _init_(self, value):
                self.value = value
                self.next = None

class CircularLinkedList:
        def_init(self):
                self.tail = None

def list is empty(self):
        return not self.tail
        
if _name_=='_main_':
        my_list = circularLinkedList()
        print(f"My list is Empty? {my_list.list is empty()}")

```
## Practice Problems
### &ensp; Problem 1
&ensp;emsp; In this problem try to add a node to the linked list.
```python
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None
class linked_list:
    def __init__(self):
        # Createe an empty list
        self.head = None
        self.tail = None
        self.count = 0
    def iterate_item(self):
        # Iterate the list.
        current_item = self.head
        while current_item:
            val = current_item.data
            current_item = current_item.next
            yield val
    def append_item(self, data):
        #Append items on the list
        pass
items = linked_list()
items.append_items('a')
items.append_items('b')
items.append_items('c')
items.append_items('d')
items.append_items('c')
for val in items.iterate_item():
    print(val)
print("\nhead.data: ",items.head.data)
print("tail.data: ",items.tail.data)
```
### &ensp; Problem 2
&ensp;emsp; For this problem the goal is to read and print the linked list reversed.
```python
class Node(object):
    
    def __init__(self, data=None, next=None, prev=None):
        self.data = data
        self.next = next
        self.prev = prev

class doubly_linked_list(object):
    def __init__(self):
        self.head = None
        self.tail = None
        self.count = 0

    def append_items(self, data):
        # Append an item 
        new_item = Node(data, None, None)
        if self.head is None:
            self.head = new_item
            self.tail = self.head
        else:
            new_item.prev = self.tail
            self.tail.next = new_item
            self.tail = new_item
        self.count += 1
    
    def iter(self):
        # Iterate the list
        current = self.head
        while current:
            item_val = current.data
            current = current.next
            yield item_val

    def print_foward(self):
        for node in self.iter():
            print(node)   
        
    def reverse(self):
        #Reverse the linked list
        

items = doubly_linked_list()
items.append_items('a')
items.append_items('b')
items.append_items('c')
items.append_items('d')
items.append_items('e')
items.append_items('f')

print("Reverse list ")
items.reverse()
items.print_foward()
```
### &ensp; Solution 1
```python
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None
        
class linked_list:
    def __init__(self):
        # Createe an empty list
        self.head = None
        self.tail = None
        self.count = 0
        
    def iterate_item(self):
        # Iterate the list.
        current_item = self.head
        while current_item:
            val = current_item.data
            current_item = current_item.next
            yield val
    def append_item(self, data):
        #Append items on the list
        node = Node(data)
        if self.tail:
            self.tail.next = node
            self.tail = node
        else:
            self.head = node
            self.tail = node
        self.count += 1
items = linked_list()
items.append_items('a')
items.append_items('b')
items.append_items('c')
items.append_items('d')
items.append_items('c')
for val in items.iterate_item():
    print(val)
print("\nhead.data: ",items.head.data)
print("tail.data: ",items.tail.data)
```
### &ensp; Solution 2
```python
class Node(object):
    
    def __init__(self, data=None, next=None, prev=None):
        self.data = data
        self.next = next
        self.prev = prev

class doubly_linked_list(object):
    def __init__(self):
        self.head = None
        self.tail = None
        self.count = 0

    def append_items(self, data):
        # Append an item 
        new_item = Node(data, None, None)
        if self.head is None:
            self.head = new_item
            self.tail = self.head
        else:
            new_item.prev = self.tail
            self.tail.next = new_item
            self.tail = new_item
        self.count += 1
    
    def iter(self):
        # Iterate the list
        current = self.head
        while current:
            item_val = current.data
            current = current.next
            yield item_val

    def print_foward(self):
        for node in self.iter():
            print(node)   
        
    def reverse(self):
        ''' Reverse linked list. '''
        current = self.head
        while current:
            temp = current.next
            current.next = current.prev
            current.prev = temp
            current = current.prev
        temp = self.head
        self.head = self.tail
        self.tail = temp

items = doubly_linked_list()
items.append_items('a')
items.append_items('b')
items.append_items('c')
items.append_items('d')
items.append_items('e')
items.append_items('f')

print("Reverse list ")
items.reverse()
items.print_foward()
```
