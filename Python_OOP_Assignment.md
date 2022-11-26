## Python OOP Assignment

Q1. What is the purpose of Python&#39;s OOP?

Ans: The purpose is to create custom classes, methods, use concepts like inheritance, polymorphism, global, static methods etc to solve complex business problems and improve coding complexity, reusability.

Q2. Where does an inheritance search look for an attribute?

Ans: An inheritance searchs the attribute first in the instance object, then in the parent class of the instance, then in all higher superclasses.

Q3. How do you distinguish between a class object and an instance object?

Ans: Classes are the parent component from which instances are created from. We can overload the classes, inherit the classes.

Q4. What makes the first argument in a class’s method function special?

Ans : It always receives the instance object that is the implied subject of the method call.

Q5. What is the purpose of the **init** method?

Ans: **init** basically works like a constructor. Whenever we create instance of the class it invokes the **init** method automatically.

Q6. What is the process for creating a class instance?

Ans : instA = ParentClass()

Q7. What is the process for creating a class?

Ans :

```class DemoClass():
        def __init__(self, name, age):
            self.name = name
            self.age = age
```

Q8. How would you define the superclasses of a class?

Ans :

```
class Square(Rectangle):
    def __init__(self, length):
        super().__init__(length, length)
```

Q9. What is the relationship between classes and modules?

Ans : The difference between a class and a module in python is that a class is used to define a blueprint for a given object, whereas a module is used to reuse a given piece of code inside another program.

Q10. How do you make instances and classes?

Ans :

```
class DemoClass():
        def __init__(self, name, age):
            self.name = name
            self.age = age
demoInstance = DemoClass('John Doe', 26)
```

Q11. Where and how should be class attributes created?

Ans : These are defined directly inside of a class.

```
class MyClass
    attr1 = 'hello'        #class attributes
    attr2 = 'world'

x = MyClass()
print(x.attr1, x.attr2) # This will print 'hello world'
```

Q12. Where and how are instance attributes created?

Ans : These are defined inside a constructor using the self parameter.

```
class Student:
    def __init__(self, name):
        self.name = name # this is instance attribute
```

Q13. What does the term &quot;self&quot; in a Python class mean?

Ans : Self represents the instance of the class. By using the “self” we can access the attributes and methods of the class in python. It binds the attributes with the given arguments.

Q14. How does a Python class handle operator overloading?

Q15. When do you consider allowing operator overloading of your classes?

Q16. What is the most popular form of operator overloading?

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?

Q18. Describe three applications for exception processing.

Ans : 1. To catch known exceptions like null reference/divided by zero. 2. To catch known business exception 3. To catch unknown exceptions and perform some additional steps in order not to let our program stop abruptly

Q19. What happens if you don&#39;t do something extra to treat an exception?

Ans : If the exception is not handled than the program will stop executing from the line of exception.

Q20. What are your options for recovering from an exception in your script?

Ans: We can use Try Except block to handle exception scenarios.

Q21. Describe two methods for triggering exceptions in your script.

Ans : We can use raise keyword to throw user defined/predefined exceptions. Or we can try to acess a file that doesn't exist or Devide a number by zero

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of
whether or not an exception exists.

Ans: We can use the finally block or put our code outside of the try except block

Q23. What is the purpose of the try statement?

Ans : Try block generally consists of the business logic in which there is a potential of error to occur.

Q24. What are the two most popular try statement variations?

Ans : Try/Except/Finally and Try/Except/Finally

Q25. What is the purpose of the raise statement?

Ans : We can use raise keyword to throw user defined/predefined exceptions

Q26. What does the assert statement do, and what other statement is it like?

Ans : The assert statement is used to continue the execute if the given condition evaluates to True. If the assert condition evaluates to False, then it raises the AssertionError exception with the specified error message.

Q27. What is the purpose of the with/as argument, and what other statement is it like?

Ans : With statement is used in exception handling to make the code cleaner and much more readable.

Q28. What are \*args, \*\*kwargs?

Ans : The arguments sent to a function using \**kwargs are stored in a dictionary structure. *args sends a list of arguments to a function.

Q29. How can I pass optional or keyword parameters from one function to another?

Ans : To pass, collect the arguments using the _ and \*\* in the function’s parameter list. Through this, you will get the positional arguments as a tuple and the keyword arguments as a dictionary. Pass these arguments when calling another function by using _ and \*\*

Q30. What are Lambda Functions?

Ans : Python Lambda Functions are anonymous function means that the function is without a name.

Q31. Explain Inheritance in Python with an example?

Ans : Inheritance allows us to define a class that inherits all the methods and properties from another class

```
class Person:
  def __init__(self, fname, lname):
    self.firstname = fname
    self.lastname = lname

class Student(Person):
  pass

x = Student("Mike", "Olsen")
x.printname()
```

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?

Ans : Class A funcc() will be invoked as its passed at first.

Q33. Which methods/functions do we use to determine the type of instance and inheritance?

Ans : The isinstance() method checks whether an object is an instance of a class whereas issubclass() method asks whether one class is a subclass of another class

Q34.Explain the use of the 'nonlocal' keyword in Python.

Ans : Python nonlocal keyword is used to reference a variable in the nearest scope

Q35. What is the global keyword?

Ans : global keyword is a keyword that allows a user to modify a variable outside the current scope.
