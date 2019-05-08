
## Printing statement


```python
print('hello world')
```

    hello world
    

## Variable Assignment


```python
var1 = 16
var2 = var1**var1
var3 = var1*var2
print(var2)
```

    18446744073709551616
    

## Count Digits in a number


```python
print(len(str(var2)))
```

    20
    

## Getting the datatype of a variable 


```python
type(var1)
```




    int




```python
type(var3)
```




    int




```python
type(var2)
type("Python")
```




    str



## String slicing


```python
str1='Python Programming'

str1[0] # Accessing the first character
```




    'P'




```python
str1[len(str1)-1] # Printing the last character
```




    'g'




```python
str1[0:6] # Printing first 6 characters
```




    'Python'




```python
str1[len(str1)-1::-1] # Reverse of a string
```




    'gnimmargorP nohtyP'




```python
str1[0:len(str1):2] # Alternate characters
```




    'Pto rgamn'




```python
str1[5::-2] # Reverse alternate characters
```




    'nhy'




```python
str1[7:]*10 # Repeating a string n times
```




    'ProgrammingProgrammingProgrammingProgrammingProgrammingProgrammingProgrammingProgrammingProgrammingProgramming'




```python
print(str1[7:],str1[7:])
```

    Programming Programming
    


```python
print(str1[7:],end='\n')
print(str1[7:],end='\n')
```

    Programming
    Programming
    

## Lists


```python
li = [123,345,'Python']
li
```




    [123, 345, 'Python']




```python
len(li) # Length of the list.It works for any iterable object.
```




    3




```python
li[1] # Accessing a single list element
```




    345




```python
li[len(li)-1] = 'Programming' # Replacing an element
li
```




    [123, 345, 'Programming']




```python
li.append('Python') # Adding a new element to a list only at the end
li
```




    [123, 345, 'Programming', 'Python']




```python
print(li)
```

    [123, 345, 'Programming', 'Python']
    


```python
li[2:] # Fetching Last two elements
```




    ['Programming', 'Python']




```python
li.pop() # Removes the last element
```




    'Python'




```python
li
```




    [123, 345, 'Programming']




```python
li.remove(123) # Removes the value
```


```python
li
```




    ['Programming']




```python
li.pop(0) # Removes the element at the given index
```




    'Programming'




```python
li
```




    []




```python
li.insert(0,123) # To insert an element anywhere in the list
```


```python
li
```




    [123]




```python
li.insert(1,567)
```


```python
li
```




    [123, 567, 567]




```python
li[1]
```




    567




```python
li
```




    [123, 567, 567]




```python
li.pop()
```




    567




```python
li
```




    [123, 567]




```python
li2=[[1,2,3],[4,5,6],[7,8,9]]
```


```python
li2
```




    [[1, 2, 3], [4, 5, 6], [7, 8, 9]]




```python
li2[0]
```




    [1, 2, 3]




```python
li2[0][1]
```




    2




```python
li2.insert(3,[10,11,12])
```


```python
li2
```




    [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]]




```python
li2.pop()
```




    [10, 11, 12]




```python
li2
```




    [[1, 2, 3], [4, 5, 6], [7, 8, 9]]




```python
li2[1].pop(2)
```




    6




```python
li2
```




    [[1, 2, 3], [4, 5], [7, 8, 9]]




```python
li2[1].insert(2,6)
```


```python
li2
```




    [[1, 2, 3], [4, 5, 6], [7, 8, 9]]




```python
for i in range(0,len(li2)):
    for j in range(0,len(li2[i])):
        print(li2[i][j],end=" ")
```

    1 2 3 4 5 6 7 8 9 


```python
for i in range(len(li2)-1,-1,-1):
    for j in range(len(li2[i])-1,-1,-1):
        print(li2[i][j],end=" ")
```

    9 8 7 6 5 4 3 2 1 


```python
li
```




    [123, 567]




```python
li.append(100)
```


```python
li.append(150)
```


```python
li.pop(4)
```




    150




```python
li
```




    [123, 567, 100, 150]




```python
li.sort()
li
```




    [100, 123, 150, 567]




```python
li.extend(20)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-156-0726698ec4d3> in <module>
    ----> 1 li.extend(20)
    

    TypeError: 'int' object is not iterable


## Tuples


```python
t1 = (123, 345, 567)
```


```python
t1
```




    (123, 345, 567)




```python
t1[2]+t1[1]
```




    912




```python
t1[2]
```




    567




```python
t1[(len(t1)-1)]
```




    567




```python
t1[1:3]
```




    (345, 567)




```python
t1[2::-1]
```




    (567, 345, 123)




```python
str(t1[0])[1] +" "+str(t1[1])[1]+" "+str(t1[2])[1]
```




    '2 4 6'




```python
t1[len(t1)-1::-1]
```




    (567, 345, 123)




```python
t1
```




    (123, 345, 567)




```python
str(t1[0])[2::-1] +" "+str(t1[1])[2::-1] +" "+str(t1[2])[2::-1] 
```




    '321 543 765'




```python
str(t1[2])[2::-1] +" "+str(t1[0])[2::-1] +" "+str(t1[1])[2::-1] 
```




    '765 321 543'



## Reading Input from a User


```python
str1=input("Enter a string = ")
```

    Enter a string = Good Afternoon Baby !
    

## Dictionaries 


```python
d1 = {'Procedural':'C','Scripting':'Python','Functional':'Haskel'}
```


```python
d1
```




    {'Procedural': 'C', 'Scripting': 'Python', 'Functional': 'Haskel'}




```python
d1['Scripting']
```




    'Python'




```python
d1.values()
```




    dict_values(['C', 'Python', 'Haskel'])




```python
d1.keys()
```




    dict_keys(['Procedural', 'Scripting', 'Functional'])




```python
d2 = {'Symbolic':'Mathematica','logic':'prolog'}
```


```python
d1.update(d2) # Merging of two dictionaries
```


```python
d1
```




    {'Procedural': 'C',
     'Scripting': 'Python',
     'Functional': 'Haskel',
     'Symbolic': 'Mathematica',
     'Object Oriented': 'Java',
     'logic': 'prolog'}




```python
d1['Object Oriented'] = 'Java' # Adding a new element to dictionaries
```


```python
d1
```




    {'Procedural': 'C',
     'Scripting': 'Python',
     'Functional': 'Haskel',
     'Symbolic': 'Mathematica',
     'Object Oriented': 'Java',
     'logic': 'prolog'}




```python
d1
```




    {'Procedural': 'C',
     'Scripting': 'Python',
     'Functional': 'Haskel',
     'Symbolic': 'Mathematica',
     'Object Oriented': 'Java',
     'logic': 'prolog'}




```python
d1['logic']
```




    'prolog'



### Problem 1:
#### Problem Statement :
For a given number, define a functiobn to check if it is divisible by 2 and 3 but not 4.


#### Constraints :
Given number will be in the range.[1,1000000000]

#### Test Cases
* Test Case 1 : checkDivisibility(6)-> True
* Test Case 2 : checkDivisibility(16)-> False
* Test Case 3 : checkDivisibility(20)-> False


```python
def checkDivisibility(n):
    if(n % 2 ==0 and n % 3== 0 and n % 4 != 0):
        return True
    else:
        return False
checkDivisibility(20)
```




    False




```python

```
