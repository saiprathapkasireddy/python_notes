# VARIABLES  

- Variables is a reserved memory location that stores and manipulates data.

- (=) is used to assign a value to a variable.

```python
# CRUD

x = 10
# CREATING value to a variable x

print(x)  
# By using print READING a value by using variable name

x = 5 
print(x)
# By changing or assigning different value to same variable UPDATING its value to 5.

del x 
# By using del keyword DELETING value and variable from memory location

print(x)
# It is name error x is not defined because we delete x.


```

### Static Initialization:

- Static Initialization refers to assign a value to a variable at declaration time. This value does'nt change when the execution of code.

```python
x = 10
language = "python"
y = 3.33 

# In the above we intialize variables statically because we assign values when a variable is declare.
```

### Dynamic Initialization:

- Dynamic Initialization refers to assign values to variables at the execution time. We can change the values as our preference.

```python
x = input("enter name:")
language = input("language is:")

# In the above we initialize variables dynamically we did'nt assign any values during declaration.
```

### Assigning Multiple Variables :

- We can assign values to multiple variables by using comma.
- We have to give same count for variables and values.

```python
a,b,c = 1,2,3
print(a) # 1
print(b) #2
print(c) #3

num,string,li = 2,"sai",[1,2,3]
print(num) # 2
print(string) # sai
print(li) # [1,2,3]
```



