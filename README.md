# MYVIZHI Y (212224050022)
# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```py
class student():
    def __init__(self, name):
        self.name=name
        print("This is non parametrized constructor")
    def display(self):
        greetings="Hello"
        print(greetings, self.name)
name=input()
c=student(name)
c.display()
```

## Output
<img width="915" height="247" alt="{632B2585-EB37-4457-AD60-C8BC4FED5487}" src="https://github.com/user-attachments/assets/56480a8f-fa8c-4211-ab69-ad3e6145b87e" />

## Result
Thus,the program is executed successfully.

# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```py
class Demo:
    def live(self):
        print("Alive")
    def __del__(self):
        print("The object no longer exists")
obj=Demo()
obj.live()
del obj
```
        

## 🧪 Output
<img width="688" height="189" alt="{C7A10E35-81DB-4A73-9641-27C5DA27BAD3}" src="https://github.com/user-attachments/assets/be3e53b5-e8e3-43e5-bbd7-23face524c2e" />

## Result
Thus,the program is executed successfully.
# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```py
class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_basic(self):
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)


# Child class Employee
class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display(self):
        print("Employee Object")
        self.display_basic()
        print("Company: ", self.company)
        print("Department: ", self.department)
        print()


# Child class Doctor
class Doctor(Details):
    def __init__(self, id, name, gender, hospital, department):
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display(self):
        print("Doctor Object")
        self.display_basic()
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)


# ---- Input for Employee ----
id1 = int(input())
name1 = input()
gender1 = input()
company = input()
dept1 = input()

# ---- Input for Doctor ----
id2 = int(input())
name2 = input()
gender2 = input()
hospital = input()
dept2 = input()

# ---- Object Creation ----
emp = Employee(id1, name1, gender1, company, dept1)
doc = Doctor(id2, name2, gender2, hospital, dept2)

# ---- Display ----
emp.display()
doc.display()
```
## Sample Output
<img width="653" height="462" alt="{A50B0DF1-DED1-4927-820A-4A5CF82FE7BE}" src="https://github.com/user-attachments/assets/38efebb7-a5e5-4cbe-bd87-454056c443cc" />

## Result
Thus,the program is executed successfully.
# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```py
class name:
    def get_name(self):
        self.name=name
class age(name):
    def get_age(self):
        self.age=age
class Id(age):
    def get_id(self):
        self.id=id
    def display(self):
        print(name,age,id)
name=input()
age=int(input())
id=input()
c=Id()
c.get_name()
c.get_age()
c.get_id
c.display()
```

## Sample Output
<img width="685" height="215" alt="{D9AC1F81-A59E-4981-8027-382764F16555}" src="https://github.com/user-attachments/assets/5cb639d4-065e-4cc6-af86-d2bfbaf1298a" />

## Result
Thus,the program is executed successfully.
# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```py
class value:
    def __init__(self,a,b):
        self.a=a
        self.b=b
class division(value):
    def add(self):
        
        print(self.a+self.b)
    def sub(self):
        print(self.a - self.b)
    def div(self):
        print(self.a/self.b)
a=int(input())
b=int(input())
c=division(a,b)
c.add()
c.sub()
c.div()
```
## Output Example
<img width="413" height="207" alt="{E09AD96A-16DD-41B8-B579-7E284E78DF0D}" src="https://github.com/user-attachments/assets/96e992ab-fd73-400c-9ae1-2ac2a145d1be" />

## Result
Thus,the program is executed successfully.
