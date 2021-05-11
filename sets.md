# Sets and it's operations

+ Does not allow duplicate values
+ All set theory operations are valid
+ Values in Set are not ordered
+ Mutable, set can be changed

---
## Initializing a Set

```python 
set1= set() #empty set
set_2={10,20,10,40,50} #second way 
set_3= {} # this will be made as a dict NOT as SET
```

### Intersection of Sets
```python
s1 = {10,20,30,40}
s2 = {30,40,50,60}
print(s1.intersection(s2)) # {40,30}
```

### Union of Sets 
```python
s1 = {10,20,30,40}
s2 = {30,40,50,60}
print(s1.union(s2)) # {40, 10, 50, 20, 60, 30}
```

### Difference of Sets
```python
s1 = {10,20,30,40}
s2 = {30,40,50,60}
# S1 -S2 is different from S2-S1
print(s1.difference(s2)) # {10,20}
print(s2.difference(s1)) # {50,60}
```

### Converting a set into Immutable form
```python
s1 = {10,20,30,40} #mutable
s2=frozenset(s1) #immutable set
```