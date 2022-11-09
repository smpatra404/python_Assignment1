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