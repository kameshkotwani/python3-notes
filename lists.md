# Lists and operations on List

 ## Lists: 
+ Dynamic 
+ Allows mutiple types of values
+ Indexing starts from 0
----------------
### Initializing a list
```python 
list1= [] #one way
list1 = list() #second way
```
### Example of list
```python
l = [10,20,30,40,50]
print(l) # output [10,20,30,40,50]
print(l[3]) # output 40
print(l[-1]) # output 50 'reverse indexing'
print(l[-3]) # output 30
```
### Operations on list

### ```list.append(value)```
```python
l = [10,20,30,40,50]
l.append(30) # will append 30 at last
print(l) # [10,20,30,40,50,30]
```

#### ```l.insert(index, value)```
```python
l = [10,20,30,40,50]
l.insert(3,77) # will insert 77 at index 3.
print(l) # [10,20,30,77,40,50]
```

#### ```in (operator)```
```python
l = [10,20,30,40,50]
print(20 in l) # will return True if value found
print(69 in l) # False (as 69 is not in list)
```


#### ```l.count(value)```
+ Will return the number of times given value occured
```python
l = [10,10,20,30,40,60,60,50,10]
l.count(10) #output -> 3
l.count(60) #output -> 2
```

#### ```l.index(element)```
+ Will return the index of the first occurence of passed value
+ Will throw an error if element is not in the list
```python
l = [10,10,20,30,40,60,60,50,10]
l.index(10) #output -> 0
l.index(60) #output -> 5
```

#### ```l.index(element,lower_index(inclusive), upper_index(exclusive))```
+ Will return the index of first occurence the element if present in the range provided
+ Will throw an error if element is not in the list (to be checked)
```python
l = [10,10,20,30,40,60,60,50,10]
l.index(10,0,3) #output -> 0
l.index(60,4,7) #output -> 5
```


#### ```l.remove(element)```
+ Removes the passed element
+ Value error is raised if element not present
```python
l = [10,20,30,40,60,60,50]
l.remove(10) #output -> [20,30,40,60,60,50]
```

#### ```l.pop() , l.pop(index)```
+ Removes the last element of the list
+ ```pop()``` function returns the value popped from the list
```python
l = [10,20,30,40,60,60,50]
l.pop() #output -> [20,30,40,60,60]
l.pop(3) # [10,20,40,60,60,50]
```

#### ```del```
+ General purpose keyword can be used in others as well
+ ```del``` 
```python
l = [10,20,50]
del l[1] # [10,50] (removes the value at the provided index)
del l[0:2] # [50]
```

# Important Points
 + The upper bound is always exclusive
    * ```[0:2]``` will range from 0,1 not 2
    * ```range(1,10)``` will return values 1 to 9, not 10.