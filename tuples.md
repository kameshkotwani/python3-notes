# Tuples

+ Immutable collection
+ Read only collection
+ Also holds different values
+ Tuple with single item, python degrades the item to a passed variable `int` , `str` ,`bool`

+ Slicing, negative indexing, range() can be used on tuples as well

+ Functions which modify the values, do not work in tuple
------

## Initialization

```python
tuple1=(10,20,30,40,50) #one way

tuple2=tuple([10,20,30,40,50]) #second way

tuple3= (10) # will be a int not a tuple
print(type(tuple3)) # int


tuple4=('India', ) # tuple with single item
print(type(tuple3)) # tuple

```

## Operations on Tuples


### ```tuple.index(value)```
```python
tuple1=(10,20,30,40,50)
	print(tuple1.index(30)) # 2
```

### ```tuple.count(value)```
```python
tuple1=(30,10,20,30,30,40,50)
	print(tuple1.count(30)) # 3
```

### ```len(object)```
```python
tuple1=(30,10,20,30,30,40,50)
	print(len(tuple1)) # 7
```

