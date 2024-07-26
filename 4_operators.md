# Operators 

- Operators in Python are special symbols or keywords that facilitate operations on variables and values. 
- They allow you to manipulate data, perform mathematical calculations, compare values, logical operations, bitwise operations and control the flow of your program. 
- Python operators are divided into several types, each serves a distinct purpose.

-----------------------------------
               1. Arthematic Operator
               2. Logical Operator
               3. Comparison Opearator
               4. Membership Operator
               5. Identity Operator
               6. Assignment Operator
               7. Bitwise Operator

### Arithmetic Operators:

- Arithmetic operators are used for mathematical calculations.
			

```python

#Addition
a = 10
b = 5
sum_result = a + b
print("Sum:", sum_result)

#Subtraction
a = 10
b = 5
diff_result = a - b
print("Difference:", diff_result)

#Multiplication
a = 10
b = 5
prod_result = a * b
print("Product:", prod_result)

#Division
a = 10
b = 5
div_result = a / b
print("Quotient:", div_result)

#Modulus (remainder)
a = 10
b = 5
mod_result = a % b
print("Remainder:", mod_result)

#Exponentiation
a = 10
b = 5
exp_result = a ** b
print("Exponentiation:", exp_result)

#Floor Division
a = 10
b = 5
result = a // b
print("Floor Division:", result)
```            

### Comparison Operators:
- Comparison operators are used to compare values and returns boolean values
		
```python
#Equal to ( == )
x = 10
y = 5 
print(x == y)   

#Not equal to ( != )
x = 10
y = 5 
print(x != y)   

#Greater than ( > )
x = 10
y = 5 
print(x > y)

#Less than ( < )
x = 10
y = 5 
print(x < y)

#Greater than or equal to ( >= )
x = 10
y = 5 
print(x >= y)   True

#Less than or equal to ( <= )
x = 10
y = 5 
print(x <= y)
```            

### Logical Operators:
- Logical operators perform logical operations on boolean values.

```python
#Logical AND ( and )
p = True
q = False
print(p and q)   

#Logical OR ( or )
p = True
q = False
print(p or q)    

#Logical NOT ( not )
p = True
q = False
print(not p)

```

### Table:   

|   p   |   q   | p AND q | p OR q |
|-------|-------|---------|--------|
| True  | True  |  True   |  True  |
| True  | False |  False  |  True  |
| False | True  |  False  |  True  |
| False | False |  False  |  False |


### Membership Operators:
- Membership operators test for membership in a sequence.

```python
#In ( in )
my_list = [1, 2, 3, 4, 5]
print(3 in my_list)   #True

#Not in ( not in )
my_list = [1, 2, 3, 4, 5]
print(6 not in my_list)   #True
print(5 not in my_list)   #False
```            

### Assignment Operators:

- Assignment operators are used to assign values to variables.

```python
#Add and assign
x = 10
x += 5   # Equivalent to x = x + 5

#Subtract and assign
x = 5
x -= 3   # Equivalent to x = x - 3

#Multiply and assign
x = 4
x *= 2   # Equivalent to x = x * 2

#Divide and assign
x = 5
x /= 4   # Equivalent to x = x / 4
print(x) 
```              

### Identity Operators:

- Identity operators are used to compare the objects, not if they are equal, but if they are actually the same object.
- Checks if two variables are referring to the exact same object in the computer's memory, not just objects that happen to look the same. 
- The 'is' operator checks for the identity of the objects, not just their content or appearance.
		
```python
a = [1, 2, 3]
b = a

#is
print(a is b) 

#is not
print(a is not b) 
```         

### Bitwise Operators:

- Bitwise operators perform operations on binary representations of integers.

```python
#Bitwise AND ( & )

p = 5      #binary:  0101
q = 3      #binary:  0011
print(p&q) #binary:  0001 
# It prints 1

#For each corresponding pair of bits, if both are 1, the result is 1; otherwise, it's 0.

#Bitwise OR ( | )
p = 5           #binary: 0101
q = 3           #binary: 0011
print(p|q)      #binary: 0111
# It prints 7

#For each corresponding pair of bits, if at least one is 1, the result is 1.

# Bitwise XOR(^)
p = 5            #binary: 0101
q = 3            #binary: 0011
print(p^q)       #binary: 0110
#it prints 6

#For each corresponding pair of bits, the result is 1 if the bits are different; otherwise, it's 0.

#Bitwise NOT ( ~ )
print(~p)
#it prints -6
```

## Operator Precedence:

- Operator precedence determines the order in which operators are evaluated in an expression. 
- It defines the hierarchy of operators, ensuring that some operators are evaluated before others.



    |Operators|Precedence|Symbol|
    |---------|----------|-------|
	|Parentheses|1 |()|
	|Exponentiation |2                         | **|
	|Unary plus and minus|3|+x, -x|
	|Multiplication, division, and remainder| 4| *, /, //, %|
	|Addition and subtraction|5|  +, -|
	|Bitwise shifts                          |6|<<, >>|
	|Bitwise AND                             |7| &|
	|Bitwise XOR                             |8| ^|
	|Bitwise OR                              |9| \ |
	|Comparison operators                    |10|<, <=, >, >=, ==, !=|
	|Membership operators                    |11|in, not in|
	|Identity operators                      |12|is, is not|
	|Logical NOT                             |13|not|
	|Logical AND                             |14|and|
	|Logical OR                              |15|or|


		Example:
		--------
		
		result = 6 + 7 * 4 ** 2 - (8 % 3)

		Exponentiation : 4 ** 2 evaluates to 16.
		Multiplication : 7 * 16 evaluates to 112.
		Addition       : 6 + 112 evaluates to 118.
		Remainder      : 8 % 3 evaluates to 2.
		Parentheses    : (8 % 3) is now 2.
		Subtraction    : 118 - 2 evaluates to 116
               