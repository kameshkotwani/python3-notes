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

tuple5 = 10,20 #will be created as a tuple
tuple6 = 10, #will be created as a tuple
```
---
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

### Extracting values from tuple seperately

```python
t1=10,20
v1,v2=t1 #v2=10,v2=20
```

### Swaping tuples

```python
t1=20,10,
t2=11,13,14,
print(f"t1={t1} t2={t2}") #t1=(20,10) t2=(11,13,14) 
t1,t2=t2,t1 # swapping two tuples
print(f"t1={t1} t2={t2}") #t2=(20,10) t1=(11,13,14) 
```

### Returning tuple from function
+ Multiple values from a function is returned as a tuple
```python
def math_operations(p1,p2):
	add = p1+p2
	sub = p1-p2
	div = p1/p2
	mul = p1*p2
	return add,sub,div,mul # Will return as a tuple
```


### Slicing in Tuples
```python
t1=10,20,30,40,50,60,70,80,90,100
	#slicing tuple
	t2 = t1[2:7]
	t3 = t1[6:]
	t4 = t1[:5]
	print(t2,t3,t4) #(30, 40, 50, 60, 70) (70, 80, 90, 100) (10, 20, 30, 40, 50)
```



