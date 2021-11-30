# Big O Notation
## &ensp; Definition 
&emsp;&ensp; Big O notaion is a mathimatical notation that we use to helps us determine how effecient different lines of code are. Effecient meaning more how much space it takes up and how fast or slow the run time is when the amount of inputs increase rather thenathe actual amount of code written. Big O notation's formula is f(n) = O(g(n)), with this we are able to get the notations which vary depends on the code.

## &ensp; Implementing
&emsp;&ensp; While using Big O notation we can examine code and be able to bentch mark it essentially. It allows us to look at code and deterimin its run speed and space it takes. The measure meants that are used to elvaluate the code or base off the formula given previously, which are O(n!), O(2^n), O(nlog n), O(n), O(log n), and O(1). These were in order from worst performence to highest with n representing the possible inputs. There is a chart below that helps organize them into performence ability

![image](https://user-images.githubusercontent.com/83718823/143959106-35a59e06-605f-418d-ab7d-7b87f4cb33d0.png)

## &ensp; Examples
&emsp;&ensp;
def find_Jerry(list_names):
	for name in list_names:
		if name == "Jerry":
			return True
	return False 
 
&emsp;&ensp; This would be O(n) because if you look at the loop that goes through the list list_names, its performance depends on if Jerry is in the list. So if we put n to represent the list. In the worst case, bob is not on the list making the big O O(n)

def loops(x):
	for i in range(x):
		print(i)
	for f in range(x):
		print(i**2)
   
&emsp;&ensp; For this example, each loop is performing at a O(n)in the function. This seems like it would be the same as the previous example but since both are performing at O(n), it will look more like O(n^2) which is twice as inefficient as O(n)
