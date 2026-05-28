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

class Details(object): 
 
    def __init__(self, name, id): 
        self.name = name 
        self.id = id

    def Employee_Details(self): 
        return self.id , self.name

class Patient_details(Employee_details): 
  
    def Employee_check(self): 
        if self.id > 500000:
           return " Valid Employee "
        else:
           return " Invalid Employee "

id=int(input())
name=input()
Employee1 = Patient_details( name , id)  # parent class object
print( Employee1.Employee_Details() , Employee1.Employee_check() )
## Sample Output
<img width="811" height="229" alt="WhatsApp Image 2026-05-28 at 2 11 55 PM" src="https://github.com/user-attachments/assets/a96ba1fa-2238-41cb-bd81-b85eb1314507" />


