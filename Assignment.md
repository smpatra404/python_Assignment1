## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

Ans. Python needs to interprete the code into machine language in order to execute it, hence it is called a high-level language. We can use python in wide variety of use cases such as data science, data analysis, machine learning, web application, desktop application, IoT etc. Hence it is a general purpose language

Q2. Why is Python called a dynamically typed language?

Ans. Python doesn't determine the type of a variable during its declaration. It assigns the variable type during the run time, hence its called as a dynamically typed language.

Q3. List some pros and cons of Python programming language?

Ans. 

    Pro:
        1. Easier learning curve.
        2. Has a huge community and libraries for any kind of needs.
        3. Versatile and can be used for various type of requirements.

    Con:
        1. Comparatively slower in comparison to compiler based languages.
        2. Dynamically typed can be problematic in certain cases.
        3. Multi threading can be tricky.
        4. Consumes more memory.

Q4. In what all domains can we use Python?

Ans. Python can be used in creating web apps, desktop apps, cross platform apps, data science, machine learning, deep learning, data engineering, Iot use cases, Game development etc.

Q5. What are variable and how can we declare them?

Ans. A variable can be treated as a container which can store various type of values depending on what we are assigning to it. In python it can be decalared as var_name = 123 or var_name = 'john maximus'

Q6. How can we take an input from the user in Python?

Ans. We can use the inbuilt 'input()' function to take input from the terminal and can store it in a variable for using later. E.g. var_num = input('Enter your phone number : ')

Q7. What is the default datatype of the value that has been taken as an input using input() function?

Ans. String

Q8. What is type casting?

Ans. Type casting is a method using which we can convert the datatype of a variable to another. In order to successfully type cast the data needs to be in an apropriate format. E.g We can type cast '123' string to 123 int. But we can't cast 'Ab1' string to Ab1 int.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

Ans. Yes we can take multiple inputs from the user using a single input(). But the inputs needs to be separated using split function in order to get the different values entered by the user. 

Example: firstName, lastName = input('Enter First Name and Last Name : ').split()

Q10. What are keywords?

Ans. Keywords are the program reserved words for the classes, functions, references which can't be used as a user defined variable/function/class name.

Q11. Can we use keywords as a variable? Support your answer with reason.

Ans. No we can not use keywords as variable names as there are already inbuilt methods with those names.

Q12. What is indentation? What's the use of indentaion in Python?,

Ans. Indentation works the same way as curly braces in other languages. It defines the scope of a code block for methods, loops, condtions, switch cases, functions, classes etc.

Q13. How can we throw some output in Python?

Ans. We can use print() in order to display an output on the terminal.

Q14. What are operators in Python?

Ans. Operators are symbols used for various operarions like assignment, arithmatic, logical etc.

Q15. What is difference between / and // operators?

Ans. Both / and // does division. But // operator floors the output. Example 9/2 = 4.5 but 9//2 = 4

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Ans: 
``` 
print('iNeuron'*4)
```

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

Ans:
```
num = input('Enter a number : ')
if(num%2 == 0):
    print('Entered number is even')
else:
    print('Entered number is odd')
```
Q18. What are boolean operator?

Ans: Boolean operators are the operators that give a boolean value as an output. Example <, >, ==, <= etc. All of these will give True or False depending on the condition its used in.

Q19. What will the output of the following?
```
1 or 0 = 1

0 and 0 = 0

True and False and True = False

1 or 0 or 0 = 1
```

Q20. What are conditional statements in Python?

Ans: Conditional statements are the statements which are used when we need to execute certain part of the code only when it satisfies a certain condition. Example:
```
if(num > 0):
    print('Valid number entered')
else:
    print('Number must be greater than 0')
```

Q21. What is use of 'if', 'elif' and 'else' keywords?

Ans: If is used when there is a single condition to check against. elif can be used in repeatation if there are more than 2 conditions. else is generally used to handle the remaining all the scenarios. Example:
```
if(a > b):
    print('a is bigger')
elif(a < b):
    print('b is bigger')
else:
    print('a and b are equals to each other')
```

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

Ans:
```
age = input('Enter your age')
if(age >= 18):
    print('I can vote')
else:
    print('I can't vote')
```

Q23. Write a code that displays the sum of all the even numbers from the given list.

Ans:
```
numbers = [12, 75, 150, 180, 145, 525, 50]
sum = 0
for num in numbers:
    if(num%2 == 0):
        sum += num
print(sum)
```

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

Ans:
```
num1, num2, num3 = input('Enter the 3 numbers : ').split()
if(num1 > num2 and num1 > num3):
    print(num1+' is the largest')
elif(num2 > num1 and num2 > num3):
    print(num2+' is the largest')
elif(num3 > num1 and num3 > num2):
    print(num3+' is the largest')
else:
    print('All numbers are equal')
```

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop

Ans:
```
numbers = [12, 75, 150, 180, 145, 525, 50]
for num in numbers:
    if(num > 500):
        break
    elif(num%5 == 0 and num != 150):
        print(num)
```
Q26. What is a string? How can we declare string in Python?

Ans: Python string is a datatype which can store text values. We can declare string as,
```
strVar = "Hellow World!"
``` 

Q27. How can we access the string using its index?

Ans:
```
strVar = "John Doe"
print(strVar[2]) //This will return "h"
```

Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
Ans:
```
desired_output = string.split()[2]
```
Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
Ans:
```
desired_output = string.split()[2][::-1]
```

Q30. Reverse the string given in the above question.

Ans:
```
desired_output = string.split()[2][::-1]
```

Q31. How can you delete entire string at once?

Ans:

```
del(strVar)
```

Q32. What is escape sequence?

Ans: An escape sequence is a sequence of characters that is used inside a character or string, which gets converted into another character or series of characters like new line, or adding (') in a string . Example:

```
print('first line \n second line') // '\n' will create a new line
```

Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```
Ans:
```
print(iNeuron\'s Big Data Course)
```

Q34. What is a list in Python?

Ans: List is a collection type variable which can store multiple type of values in it. Example,
```
listVar = ['a', 1, 'b', c, False]
```

Q35. How can you create a list in Python?

Ans:
```
listVar = ['a', 1, 'b', c, False]
```

Q36. How can we access the elements in a list?

Ans: We can access the elemnts in a list using the index. Example:
```
print(listVar[3])
```

Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 
Ans:
```
print(lst[4][2])
```

Q38. Take a list as an input from the user and find the length of the list.

Ans:
```
input_string = input("Enter list elements separated by space")
lst  = input_string.split()
print(len(lst))
```

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```
Ans:
```
lst.insert(3, "Big")
```
Q40. What is a tuple? How is it different from list?

Ans: Tuples are very identical to list. The major differences being the values are stored in an ordered format and we can not Insert/Delete/Update the values of a tuple once its declared.

Q41. How can you create a tuple in Python?

Ans:
```
tupleVar = (1,10,2,6,"Abc")
```

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

Ans: We can not add any values to a tuple once its declared. The reason being, Tuples can not be modified once its declared.

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

Ans: Append method is not available for Tuples. However we can concatinate them using (+) operator and create a new tuple for the combined result. Example :
```
tup1 = (1, 2, 3)
tup2 = (4, 5, 6)

tupFinal = tup1 + tup2
```

Q44. Take a tuple as an input and print the count of elements in it.

Ans: 
```
input_string = input("Enter elements separated by space")
inputTuple  = tuple(input_string.split())
```

Q45. What are sets in Python?

Ans: Sets are collection objects same as list. Differentiating factor being set items are unordered, unchangeable, and do not allow duplicate values. Although we can not update the values, we can insert/delete elements from it.

Q46. How can you create a set?

Ans: 
```
lst = {1, 2, 3, 3}
```

Q47. Create a set and add "iNeuron" in your set.

```
lst = {1, 2, 3, 3}
lst.add('iNeuron')
```

Q48. Try to add multiple values using add() function.

Ans: add() takes only one value. We can not pass multiple strings in it.

Q49. How is update() different from add()?

Ans: update() method can insert multiple values into the set. But add() can only add 1 element at a time.

Q50. What is clear() in sets?

Ans: clear() method removes all the elemnets of the given set.

Q51. What is frozen set?

Ans: frozenset() Method creates an immutable Set object from a given collection object

Q52. How is frozen set different from set?

Ans: We can not add or delete any elements in frozen set like we do in normal set

Q53. What is union() in sets? Explain via code.

Ans: union() combines the given sets and returns a new set. All the duplicate values will be removed and only uinque values from both of the sets will be displayed

Q54. What is intersection() in sets? Explain via code.

Ans: intersection() gives us the uique items those are common in the given sets.

Q55. What is dictionary in Python?

Ans: Dictionary is a key value pair object. Where the details are stored in unique keys.

Q56. How is dictionary different from all other data structures.

Ans: In dictionary we can access the values using the unique keys instead of index.

Q57. How can we delare a dictionary in Python?

Ans:
```
empDict = {
  "name": "Subham",
  "sex": "Male",
  "age": 26
}
```

Q58. What will the output of the following?
```
var = {}
print(type(var))
```
Ans: dict

Q59. How can we add an element in a dictionary?

Ans: We can either add an element by stating testDict['newKey'] = 'New Value' or using uodate method which will update if the given key already exists or it will ad it as a new key-value pair testDict.update({"newKey": "New Value"})

Q60. Create a dictionary and access all the values in that dictionary.

Ans:
```
empDict = {
  "name": "Subham",
  "sex": "Male",
  "age": 26
}

for key in empDict.keys():
    print(empDict[key])
```

Q61. Create a nested dictionary and access all the element in the inner dictionary.

Ans:
```
empDict = {
    "id" : 1,
    "emp1": {
        "name" : "Subham",
        "sex": "Male",
        "age": 26
    }
}

for key in empDict['emp1'].keys():
    print(empDict['emp1'][key])

```

Q62. What is the use of get() function?

Ans: get() method returns the value of the item associated with the given key.

Q63. What is the use of items() function?

Ans: items() method returns a view of the called object. It ontains the key-value pairs of the dictionary as tuples in a list.

Q64. What is the use of pop() function?

Ans: pop() function removes element from the mentioned index of a list.

Q65. What is the use of popitems() function?

Ans: opitem() function removes the item that was last inserted into the dictionary.

Q66. What is the use of keys() function?

Ans: keys() function will give us a list of key names of the provided dictionary.

Q67. What is the use of values() function?

Ans: values() function returns a view object containing the values of the dictionary as a list.

Q68. What are loops in Python?

Ans: Loops are the methods which iterates a set of code untill the exit condition is satisfied.

Q69. How many type of loop are there in Python?

Ans: 2 types of looks are there i.e. for, while

Q70. What is the difference between for and while loops?

Ans: For loops is used when we know how many times we need the iteration needs to be. For the unkown or dynamic count of iteration we can use while loop.

Q71. What is the use of continue statement?

Ans: The continue keyword is used to end the current iteration in a loop and continues to the next onem.

Q72. What is the use of break statement?

Ans: break is used to get out of the loop instead of moving to the next iteration.

Q73. What is the use of pass statement?

Ans: Generally pass is used inside of a loop as a placeholder which can be later filled with some code.

Q74. What is the use of range() function?

Ans: range() will return a list of values in the mentioned range of values, like all values between 1 and 10.

Q75. How can you loop over a dictionary?

Ans: We can get the dictionary keys using keys() method and loop over those to access values of each keys.


### Coding problems
Q76. Write a Python program to find the factorial of a given number.

Ans:
```
num = int(input("Enter a number : "))
fact = 1
for i in range(1, num+1):
    fact = fact * i
print("Factorial is :",fact)
```

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100

Ans:
```
principal = int(input("Enter pricipal : "))
time = int(input("Enter time period : "))
interest = int(input("Enter rate of interest : "))

simpleInterest = (principal * time * interest) / 100

print("Total interest is ", simpleInterest)
```

Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.

Ans:
```
principal = int(input("Enter pricipal : "))
time = int(input("Enter time period : "))
interest = int(input("Enter rate of interest : "))

compInterest = principal * (pow((1 + interest / 100), time))

print("Total interest is ", compInterest)
```

Q79. Write a Python program to check if a number is prime or not.

Ans:
```
num = int(input("Enter the number : "))

if num > 1:
    for i in range(2, int(num/2)+1):
        if (num % i) == 0:
            print("Not a prime number")
            break
    else:
        print("Prime number")
else:
    print("Not a prime number")
```

Q80. Write a Python program to check Armstrong Number.

Ans:
```
num = int(input("Enter a number : "))
sum = 0
temp = num

while temp > 0:
   digit = temp % 10
   sum = sum + (digit ** 3)
   temp = temp // 10

if num == sum:
   print("Armstrong number")
else:
   print("Not an Armstrong number")
```

Q81. Write a Python program to find the n-th Fibonacci Number.

Ans:
```
def fibSeries(num):
   if num <= 2:
      return num - 1
   else:
      return fibSeries(num - 1) + fibSeries(num - 2)

num = int(input("Enter the nth number : "))
print("nth Element of the Fibonacci Series :", fibSeries(num))
```

Q82. Write a Python program to interchange the first and last element in a list.

Ans:
```
lis = [1,2,3,4,5]
temp = lis[0]
lis[0] = lis[-1]
lis[-1] = temp

print(lis)
```

Q83. Write a Python program to swap two elements in a list.
```
lis = [1,2,3,4,5]
elementIndex = 2
swapIndex = 4

temp = lis[elementIndex]
lis[elementIndex] = lis[swapIndex]
lis[swapIndex] = temp

print(lis)
```

Q84. Write a Python program to find N largest element from a list.

Ans:
```
lis = [20,28,39,10,21,-5,80]
n = int(input("Enter the N value : "))
lis.sort()

print(lis[-n:])
```

Q85. Write a Python program to find cumulative sum of a list.

Ans:
```
lis = [1,2,3,4,5]
sm = 0
clist = []
for i in lis:
    sm = sm + i
    clist.append(sm)

print(clist)
```
Q86. Write a Python program to check if a string is palindrome or not.

Ans:
```
inStr = input("Enter string : ")
if(inStr == inStr[::-1]):
    print("Pallindrome")
else:
    print("Not pallindrome")
```

Q87. Write a Python program to remove i'th element from a string.

Ans:
```
inStr = input("Enter string : ")
idx = int(input("Enter the index you want to remove : "))
new_str = inStr[:idx-1] + inStr[idx:]

print("New value after removal :", new_str)
```
Q88. Write a Python program to check if a substring is present in a given string.

Ans:
```
inStr = input("Enter string : ")
subStr = input("Enter the substring : ")
if(subStr in inStr):
    print("Substring found")
else:
    print("Not found")
```

Q89. Write a Python program to find words which are greater than given length k.

Ans:
```
inStr = input("Enter string : ")
length = int(input("Enter the length : "))
print("Words beyond the provided legth is :",inStr[length :: ])
```

Q90. Write a Python program to extract unquie dictionary values.

Ans:
```
testDic = {
    "a" : 1,
    "b" : 2,
    "c" : 2,
    "d" : 3,
    "e": 3,
    "f": 4
}
lis = []

for k in testDic.keys():
    lis.append(testDic[k])
print(set(lis))
```

Q91. Write a Python program to merge two dictionary.

Ans:
```
dict1 = {'a': 1, 'b': 2, 'c': 3}
dict2 = {'d': 4, 'e': 2}

print({**dict1, **dict2})
```

Q92. Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
Ans:
```
Input = [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
resDict = {}
for tup in Input:
    resDict[tup[0]] = tup[1]
print(resDict)
```
Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```
Ans:
```
lis = [9, 5, 6]
resLis = []
for i in lis:
    resLis.append((i, pow(i, 3)))
print(resLis)
```
Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
Ans:
```
test_tuple1 = (7, 2)
test_tuple2 = (7, 8)
resLis = []

for i in test_tuple1:
    for j in test_tuple2:
        resLis.append((i,j))
        resLis.append((j,i))
print(resLis)
```
Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```
Ans:
```
Input = [('for', 24), ('Geeks', 8), ('Geeks', 30)] 

print(sorted(Input, key = lambda x: x[1]))
```
Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
Ans:
```
count = 1
while count <= 5:
    print("*"*count)
    count += 1
```
Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
Ans:
```
count = 1
while count <= 5:
    print(" "*(5-count)+"*"*count)
    count += 1
```
Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
Ans:
```
row_count = 5
count = row_count - 1

for i in range(0, row_count):
    for j in range(0, count):
        print(end=" ")
    count = count - 1
    for j in range(0, i+1):
        print("* ", end="")
    
    print("\r")
```
Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
Ans:
```
row_count = 5
num = 1

for i in range(0, row_count):
    num = 1
    for j in range(0, i+1):
        print(num, end=" ")
        num = num + 1
    print("\r")
```
Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
Ans:
```
asci_number = 65
row_count = 5

for i in range(0, row_count):
    for j in range(0, i+1):
        ch = chr(asci_number)
        print(ch, end=" ")
    asci_number = asci_number + 1
    print("\r")
```