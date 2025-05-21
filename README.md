# 19CS301-Module- 6
EX: 6.1   POLYMORPHISM

### AIM: 

To Create two specific classes- Beans and Mango. Along with that, create a generic function that tells us the type and color of the object we pass. Mind you, since we have passed only “obj” through it, this obj can be any object.


### ALGORITHM:
Step1: create class Beans and def a function type and color

Step 2: create a class Mango and def a function type and color

Step3: def a function func

Step 4: call the objects and execute the program

### PROGRAM:
```
class Beans ():
    def type(self):   
          print("Vegetable")
    def color(self):
          print("Green")
class Mango:
   def type(self):
          print("Fruit")
   def color(self):
         print("Yellow")
   def func(obj):
         obj.type()
         obj.color()
         obj_beans = Beans()
         obj_mango = Mango()
         func(obj_beans)
         func(obj_mango)
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/b41a3e12-896b-4f6c-a9b2-19045a5088f9)


### RESULT: 

Thus, the program has been successfully executed.

EXP.No: 6.b OPERATOR OVERLOADING

### AIM: 

write a python program to overload less than operator


###ALGORITHM:
Step1 :create class A and def init	 

Step2: def it	with a condition if self.a < o.a 

Step 3: call the function and execute the program.


### PROGRAM:
```
class A :
     def     init (self,a):
             self.a=a
     def     lt (self,o):
              if self.a < o.a :
                   return "ob1 is less than ob2"
              else:
                   return "ob2 is less than ob1"
ob1 = A(2)
ob2 = A(3)
print(ob1<ob2)
```
###OUTPUT:


![image](https://github.com/user-attachments/assets/dae03d17-1004-424e-a179-ef62fd2681bd)



###RESULT: 

Thus, the program has been successfully executed.


EX: 6.3 ABSTRACT CLASS METHOD

### AIM: 

To create an abstract method feed() in an abstract class Animal and implement it in subclasses Lion, Panda, and Snake.

### ALGORITHM:

Step 1: Import the ABC and abstractmethod from the abc module.

Step 2: Define the abstract class Animal with an abstract method feed().

Step 3: Create the subclasses Lion, Panda, and Snake, each implementing the feed() method.

Step 4: Create objects for each subclass.

Step 5: Call the feed() method using each object.

Step 6: Execute the program.

### PROGRAM:


```from abc import ABC
from abc import ABC, abstractmethod
class Animal(ABC): # Inherit from ABC(Abstract base class)
    @abstractmethod  # Decorator to define an abstract method
    def feed(self):
        pass
class Lion(Animal):
    #Add abstract methos implementation
    def feed(self):
        print("Feeding a lion with raw meat!")

class Panda(Animal): 
    def feed(self): 
        print("Feeding a panda with some tasty bamboo!") 

class Snake(Animal): 
    def feed(self): 
        print("Feeding a snake with mice!")
zoo = [Lion(), Panda(), Snake()]

for animal in zoo:
    animal.feed()
```
### OUTPUT:

![image](https://github.com/user-attachments/assets/29bc86a1-d46f-44e1-b01e-0ac8dd835e0e)



### RESULT: 

Thus, the program has been successfully executed.

EXP.No: 6.4     ENCAPSULATION


### AIM:

To implement encapsulation using private members in a class Class1Students with private variables name and age, and to access/modify them using getter and setter methods.

###ALGORITHM: 

Step 1: Define the class Class1Students with private variables __name and __age.

Step 2: Define the constructor __init__ to initialize name and age.

Step 3: Create the speak() method to print the values.

Step 4: Define getter methods get_name() and get_age() to access private variables.

Step 5: Define setter methods set_name() and set_age() to modify private variables.

Step 6: Create an object and use the speak() method to display original values.

Step 7: Use setter methods to modify the values and invoke speak() again to show updated values.

Step 8: End the program.

###PROGRAM:
```
class Class1Students:
    name="Michael"
    age=40
    def __init__(self,name,age):
        self.name=name
        self.age=age
    def speak(self):
        print(f"my name is {self.name}, and I am {self.age} years old.")
    def set_nameage(self,x,y):
        self.name=x
        self.age=y
s1=Class1Students("Michael",40)
s2=Class1Students("John",25)
s2.name="John"
s1.speak()
s2.set_nameage=("John",25)
s2.speak()
```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/360bb4d5-6d33-499f-9bb8-ed716ad57d09)

 

### RESULT: 

Thus, the program has been successfully executed




