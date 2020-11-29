# Object Oriented Programming

## **Object-Oriented Programming \(OOP\)**

**P**rocedural programming is about writing procedures or methods that perform operations on the data, while object-oriented programming is about creating objects that contain both data and methods.

Object-oriented programming has several advantages over procedural programming:

* OOP is faster and easier to execute
* OOP provides a clear structure for the programs
* OOP helps to keep the Java code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug
* OOP makes it possible to create full reusable applications with less code and shorter development time

## Class

a **class** is a blueprint for creating **objects** \(a particular data structure\), providing initial values for state \(member variables or attributes\), and implementations of behavior \(member functions or methods\).

The user-defined objects are created using the `class` keyword. The class is a blueprint that defines a nature of a future object. An **instance** is a specific object created from a particular class. Classes are used to create and manage new objects and support **inheritance**—a key ingredient in object-oriented programming and a mechanism of reusing code.

![Car Class and instances of Car](.gitbook/assets/python10.png)

The image above shows how a `Car` object can be the template for many other `Car` instances. In the image, there are three instances: `ford`, `toyota`, and `volkswagen`. Here, we will make a new class called `Car`, that will structure a `Car` object to contain information about the car’s model, the color, how many passengers it can hold, its speed, etc. A class can define types of operations, or methods, that can be performed on a `Car` object. For example, the `Car` class might specify an `accelerate` method, which would update the `speed`attribute of the car object.

{% embed url="https://repl.it/@mardavis/OOP-class-constructor" %}



