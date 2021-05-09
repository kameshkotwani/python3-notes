# Lists and operations on List

 ## Lists: 
+ Dynamic 
+ Allows mutiple types of values
+ Indexing starts from 0
+ Has reverse indexing example, list[-1],list[-2]
+ Mutable


----------------
## Initializing a list
```python 
l= [] #one way
l = list() #second way
```

## Example of list
```python
l = [10,20,30,40,50]
l2=['apple','banana','grapes']
print(l) # output [10,20,30,40,50] # using array type indexing
print(l[3]) # output 40
print(l[-1]) # output 50 'reverse indexing'
print(l2[-3]) # output apple
```

# Operations on list

### ```list.append(value)```
+ Appends the passed value at the end
+ It takes O(1) time to append in the end
```python
list_e = [10,20,30,40,50]
l.append(30) # will append 30 at last
print(l) # [10,20,30,40,50,30]
```

### ```list.insert(index, value)```
+ Inserts the given value at a given index
```python
l = [10,20,30,40,50]
l.insert(3,77) # will insert 77 at index 3.
print(l) # [10,20,30,77,40,50]
```

### ```in (operator)```
+ Checks if some element is present in dataset or not
+ Returns `bool` value
```python
l = [10,20,30,40,50]
print(20 in l) # will return True if value found
print(69 in l) # False (as 69 is not in list)
```


### ```list.count(value)```
+ Will return the number of times given value occured
```python
l = [10,10,20,30,40,60,60,50,10]
l.count(10) #output -> 3
l.count(60) #output -> 2
```

### ```list.index(element)```
+ Will return the index of the first occurence of passed value
+ Will throw an error if element is not in the list
```python
l = [10,10,20,30,40,60,60,50,10]
l.index(10) #output -> 0
l.index(60) #output -> 5
```

### ```list.index(element,lower_index(inclusive), upper_index(exclusive))```
+ Will return the index of first occurence the element if present in the range provided
+ Will throw an error if element is not in the list (to be checked)
```python
l = [10,10,20,30,40,60,60,50,10]
l.index(10,0,3) #output -> 0
l.index(60,4,7) #output -> 5
```


### ```list.remove(element)```
+ Removes the passed element
+ Value error is raised if element not present
```python
l = [10,20,30,40,60,60,50]
l.remove(10) #output -> [20,30,40,60,60,50]
```

### ```list.pop() , list.pop(index)```
+ Removes the last element of the list
+ ```pop()``` function returns the value popped from the list
+ Time Complexity O(1)
```python
l = [10,20,30,40,60,60,50]
l.pop() #output -> [20,30,40,60,60]
l.pop(3) # [10,20,40,60,60,50]
```

### ```del```
+ General purpose keyword can be used in others as well
```python
l = [10,20,50]
del l[1] # [10,50] (removes the value at the provided index)
del l[0:2] # [50]
```
### ```max(list)```
+ Returns max value present in list
```python
l = [10,20,50]
print(max(l)) # output 50
l2=['banana','apple','cherry']
print(max(l2)) # gives lexographically highest string
```

### ```min(list)```
+ Returns min value present in list

```python
l = [10,20,50]
print(min(l)) # output 10
l2=['banana','apple','cherry']
print(min(l2)) # gives lexographically smallest string
```

### ```sum(list)```
+ Returns sum of values present in list [int]
+ If we typecast each str of int value to int, it adds.
+ Throws error if different types of values present
```python
l = [10,20,50]
print(sum(l)) # output 80
l2=[10,'apple'] # throws error
l3 = [int('10'),int('30')] #output 40
l4 = ['int(apple)', int('banana')] #invalid literal
```

### ```list.reverse()```
+ Reverses the list 
```python
l1=[10,20,30]
l1.reverse() # [30,20,10]
```

### ```list.sort()```
+ Sorts the list in increasing order 
+ sort function only works
```python
l1=[60,10,30]
l1.sort() # [10,30,60]
l2=['banana','apple','cherry']
l2.sort() # ['apple','banana','cherry'] # will sort lexographically
```

---------------
# Important Points
+ **The upper bound is always exclusive**
	1. ```[0:2]``` will range from 0,1 not 2
	2. ```range(1,10)``` will return values 1 to 9, not 10.
+ `max()` , `min()` , `sum()` , `sort()` only work in same data types.
+ `reverse()` will work in different data types as it only reverses the values, does not check them.

## Advantages:
+ Random Access.
+ Cache Friendlinesss

## Diadvantages:
+ Insertion, deletions, search(**not sorted**) are slow O(n). 


