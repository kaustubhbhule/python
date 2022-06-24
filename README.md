
# Python Programs

## Important

Reverse Number

```python
Program:

rev=0
num = 12345
while num > 0:
    rem = num % 10
    rev = (rev * 10) + rem
    num = num // 10
print("Reversed Number:", rev)

```

```
Output:

Reversed Number: 54321

```
#

Palindrome Number

```python
Program:

rev=0
num = 151
temp = num
while num > 0:
    rem = num % 10
    rev = (rev * 10) + rem
    num = num // 10

if rev == temp:
    print(temp, "is palindrome")
else:
    print(temp, "is not palindrome")

```

```
Output:

151 is palindrome

```
#

Armstrong Number

```python
Program:

sum=0
num = 153
temp = num
while num > 0:
    rem = num % 10
    sum = sum + rem**3
    num = num // 10

if sum == temp:
    print(temp, "is armstrong")
else:
    print(temp, "is not armstrong")

```

```
Output:

153 is armstrong

```
#

Prime number

```python
Program:

num = 5
count = 0
for i in range(1,num+1):
    if num%i==0:
        count+=1
if count <= 2:
    print(num, "is prime")
else:
    print(num, "is not prime")
```

```
Output:

5 is prime

```

#

## Practicals

Develop minimum 2 programs using Arithmetic Operators, exhibiting data type
conversion.

```python
Program:

# Arithmetic Operations
a = 10
b = 5
print("Sum is",a+b)
print("Difference is",a-b)
print("Product is",a*b)
print("Divison is",a/b)

# Data type conversion
c = 10
print(type(c))
c = float(c)
print(type(c))
```

```
Output:

Sum is 15
Difference is 5
Product is 50
Divison is 2.0
<class 'int'>
<class 'float'>
```
#

Develop programs using different data types (numbers, string, tuple, list, dictionary

```python
Program:

# Numbers
a = 5+9j
print(type(a))

# String
b = "Hello, World!"
print(type(b))

# Tuple
c = (1,2,3,4,5)
print(type(c))

# List
d = [1,2,3,4,5]
print(type(d))

# Dictinory
e = {'name':'Joe'}
print(type(e))

```

```
Output:

<class 'complex'>
<class 'str'>
<class 'tuple'>
<class 'list'>
<class 'dict'>
```
#

Calculate the Average of numbers in a given List.

```python
Program:

sum=0
lst = [10,20,30,40,50]
for i in lst:
    sum+=i
print("Average is",sum/len(lst))

```

```
Output:

Average is 30.0

```
#

Exchange the Values of Two Numbers without Using a Temporary Variable.

```python
Program:

a = 5
b = 7
print(a,b)

a = a * b
b = a // b
a = a // b
print(a,b)

```

```
Output:

5 7
7 5

```
#

Write simple programs to calculate the area and perimeter of
the Square, and the volume & perimeter of the cone.

```python
Program:

side = 5
print("Area of square is", side*side)
print("Perimeter of square is", side*4)

r = 5
h = 5
print("Volume of cone is",3.14*r*r*h/3)

```

```
Output:

Area of square is 25
Perimeter of square is 20
Volume of cone is 130.83333333333334

```
#

Read Height in Centimeters and then convert the Height to Feet and Inches

```python
Program:

cm = float(input("Enter height (in cm): "))
print("Height in Feet is", round(cm/30.48,3))
print("Height in Inches is", round(cm/2.54,3))

```

```
Output:

Enter height(in cm): 160
Height in Feet is 5.249
Height in Inches is 62.992

```
#

Find the Sum of Digits in a number.

```python
Program:

num = 12345
sum = 0
while num > 0:
    rem = num % 10
    sum = sum + rem
    num = (num-rem) // 10
print("Sum of digits is", sum)

```

```
Output:

Sum of digits is 15

```
#

Print all Numbers in a Range Divisible by a Given Number

```python
Program:

n = 8
for i in range(1,100):
    if i%n== 0:
        print(i, end=" ")

```

```
Output:

8 16 24 32 40 48 56 64 72 80 88 96

```
#

Write a programs to:  
(i) Create a list, add element to list, delete element from the list. 
(ii) Sort the list, reverse the list and
counting elements in a list.

```python
Program:

lst = [1,2,2,3,4,5]
print("List: Created: ",lst)
lst.append(6)
print("Item Added:",lst)
lst.remove(6)
print("Item Removed:",lst)

lst.sort()
print("Sorted List:", lst)
lst.reverse()
print("Reversed List:", lst)
count = lst.count(2)

```

```
Output:

List: Created:  [1, 2, 2, 3, 4, 5]
Item Added: [1, 2, 2, 3, 4, 5, 6]
Item Removed: [1, 2, 2, 3, 4, 5]
Sorted List: [1, 2, 2, 3, 4, 5]
Reversed List: [5, 4, 3, 2, 2, 1]

```
#

Merge Two Lists and Sort it.

```python
Program:

lst1 = [1,2,3,4,5]
lst2 = [5,1,2,3,4]
for i in lst2:
    lst1.append(i)
lst1.sort()
print("Merged and Sorted List:", lst1)

```

```
Output:

Merged and Sorted List: [1, 1, 2, 2, 3, 3, 4, 4, 5, 5]

```
#

Remove the Duplicate Items from a List

```python
Program:

lst = [1,2,2,3,3,4,5]
nlst = list(dict.fromkeys(lst))
print("Original List:", lst)
print("After Removing Duplicates:", lst)

```

```
Output:

Original List: [1, 2, 2, 3, 3, 4, 5]
After Removing Duplicates: [1, 2, 2, 3, 3, 4, 5]

```
#

Create dictionary, add element to dictionary, delete element from the dictionary.

```python
Program:

dict = {'1': 'Mango', '2': 'Apple', '3': 'Banana'}
print("Dictinory Created:",dict)

dict.update({'4': 'Pineapple'})
print("Item Added:",dict)

dict.pop('4')
print("Item Deleted:",dict)

```

```
Output:

Dictinory Created: {'1': 'Mango', '2': 'Apple', '3': 'Banana'}
Item Added: {'1': 'Mango', '2': 'Apple', '3': 'Banana', '4': 'Pineapple'}
Item Deleted: {'1': 'Mango', '2': 'Apple', '3': 'Banana'}

```
#

Write a program to: \
(i) To print all prime numbers from 1 to N.

```python
Program:

upper = int(input("Enter upper range: "))
print("Result:", end=" ")
for i in range (1, upper+1):
    if i > 1:
        for j in range(2, i):
            if i%j==0:
                break
        else:
            print(i, end=" ")

```

``` 
Output:

Enter upper range: 10
Result: 2 3 5 7

```
