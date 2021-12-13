## Stacks

## &ensp; Definition
&emsp;&ensp; A stack is a way of organizing data into a usable structure when programming. This data structure is a linear data structure, which means that it can only be worked with from one side of the structure. How a stack specifficly works is by a last in first out system, which can commenly be compared to pancake stacks to data stucture stacks. They are compared often because just like with pancakes you eat or grab, you do so from the top and not the bottom and the same happens with a stack data structure. With the stack the the last thing put into the stack is the first that can come off, it can be better visualized by the figure below. 

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;![image](https://user-images.githubusercontent.com/83718823/145653795-9025205f-38f0-4cab-aaf9-04cd1383034e.png)

## Example and Efficiencey 
&emsp;&emsp; When dealing with stacks there is 3 primary things to do with the stack, which are push, pop, peek. To start the push command allows us to add data to the stack and The new data will become the new top. The brings me to the next command, which is pop. The Pop function allows us to reamove things form the stack but when used it will remaove the top piece of data. When doing either of these things the data structure efficency is O(1) becasue they are generay simple commmands and dont require a lot of memory. Moving to the last command function is peek, this command is kinda a exception to how the stack functions because it allow you to look into the middle of teh stack and recieve its values. The efficency of that command is generally O(1) like the previous ones. the efficency can Be decreased if you search thorough a stack with a loop to find something in the stack. In the worst case when people use loop through stacks it's efficenacy will trun to O(n). See the example below of a example of this.
```python
if item_1 == 7:
    stack = Stack()
    for i in range(1, 11):
        stack.push(i)
    print(f"Stack: {stack}")
```
## Practice Problems
### Problem 1
&emsp;&ensp; For this probelm you want to figure out what left in the stack at the end with out running the code. 
```python 
stack = []
stack.append(3)
stack.append(9)
stack.append(4)
stack.pop()
stack.pop()
stack.append(65)
stack.append(85)
stack.pop()
stack.append(6)
stack.append(69)
stack.append(9)
stack.append(7)
stack.pop()
stack.pop()
stack.append(10)
stack.append(20)
stack.pop()
stack.pop()
stack.append(11)
stack.append(12)
stack.pop()
stack.pop()
stack.pop()
stack.append(7)
stack.append(17)
stack.append(30)
stack.append(19)
stack.pop()
stack.pop()
```
### Problem 2
&ensp;&emsp; 
```python
stack = stack()
 
# append() function to push
# element in the stack
stack.append('a')
stack.append('b')
stack.append('c')
def add2stack(item):
  # insert code here
  pass
  
#test
add2stack(d)
print (stack)
add2stack(e)
print (stack)

```
## Solutions
### Solution 1
```python
stack = []
stack.append(3)  #[3]
stack.append(9)  #[9]
stack.append(4)  #[3, 9, 4]
stack.pop()      
stack.pop()    
stack.append(65) #[3, 65]
stack.append(85) #[3, 65, 85]
stack.pop()
stack.append(6)  #[3, 65, 6]
stack.append(69) #[3, 6, 65, 69]
stack.append(9)  #[3, 6, 65, 69, 9]
stack.append(7)  #[3, 6, 65, 69, 9, 7]
stack.pop()
stack.pop()
stack.append(10) #[3, 6, 65, 69, 10]
stack.append(20) #[3, 6, 65, 69, 10, 20]
stack.pop()
stack.pop()
stack.append(11) #[3, 6, 65, 69, 11]
stack.append(12) #[3, 6, 65, 69, 11, 12]
stack.pop()
stack.pop()
stack.pop()
stack.append(7)  #[3, 6, 65, 7]
stack.append(17) #[3, 6, 65, 7, 17]
stack.append(30) #[3, 6, 65, 7, 17, 30]
stack.append(19) #[3, 6, 65, 7, 17, 30, 19]
stack.pop()
stack.pop()
stack.pop()
print(stack)     #[3, 6, 65, 7]
```
### Solution 2
```python 
stack = stack()
 
# append() function to push
# element in the stack
stack.append('a')
stack.append('b')
stack.append('c')
def add2stack(item):
    if item == stack: 
        append.stack(item)
        return
    else:pass
  
#test
add2stack(d)
print (stack)
add2stack(e)
print (stack)
ad2stack(c)
print
```
