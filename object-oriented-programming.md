# Object Oriented Programming

## **Object-Oriented Programming \(OOP\)**

**P**rocedural programming is about writing procedures or methods that perform operations on the data, while object-oriented programming is about creating objects that contain both data and methods.

Object-oriented programming has several advantages over procedural programming:

* OOP is faster and easier to execute
* OOP provides a clear structure for the programs
* OOP helps to keep the Java code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug
* OOP makes it possible to create full reusable applications with less code and shorter development time

A **class** is a blueprint for creating **objects** \(a particular data structure\), providing initial values for state \(member variables or attributes\), and implementations of behavior \(member functions or methods\).

The user-defined objects are created using the `class` keyword. The class is a blueprint that defines a nature of a future object. An **instance** is a specific object created from a particular class. Classes are used to create and manage new objects and support **inheritance**—a key ingredient in object-oriented programming and a mechanism of reusing code.

![Car Class and instances of Car](.gitbook/assets/python10.png)

The image above shows how a `Car` object can be the template for many other `Car` instances. In the image, there are three instances: `ford`, `toyota`, and `volkswagen`. Here, we will make a new class called `Car`, that will structure a `Car` object to contain information about the car’s model, the color, how many passengers it can hold, its speed, etc. A class can define types of operations, or methods, that can be performed on a `Car` object. For example, the `Car` class might specify an `accelerate` method, which would update the `speed`attribute of the car object.

{% embed url="https://repl.it/@mardavis/OOP-class-constructor" %}

A class is a way of organizing information about a type of data so a programmer can reuse elements when making multiple instances of that data type—for example, if a programmer wanted to make three instances of `Car`, maybe a BMW, a Ferrari, and a Ford instance. The `Car` class would allow the programmer to store similar information that is unique to each car \(they are different models, and maybe different colors, etc.\) and associate the appropriate information with each car.

## Classes

### Creating A Class

In Javascript, classes are declared by the keyword `class` followed by the class name. A `class` statement defines a new class just as a `def` statement defines a new function.

The following example will define a simple class that defines a person.

```javascript
class Person {

```

### **The Constructor Method**

After declaring the class name, a programmer must define a **constructor** method. In **Javascript**, this is denoted `constructor`. The `constructor` function takes any number of arguments as desired by the programmer. For this example that describes a person, the programmer wants to know each persons name, age, gender and interests. 

The name `constructor()` is used for the "constructor method" for the class. While a class is a blueprint for a new data type, the programmer still needs to create values of this data type in order to have something that can store in variables or pass to functions.

When called, the constructor creates the new object, runs the code in the constructor, and returns the new object. 

So far, we have

```javascript
class Person {
  constructor(name, age, gender, interests) {
```

The above defines a method for the person class. Methods are used for functions that belong to a class.

**Variables and the Body of the `constructor` Method**

To access the arguments and associate them with a particular instance of the class, within the **`constructor`** method, create variables for each argument​ like this: `this.variableName = variableName`. 

Another component associated with classes are **attributes**. Attributes are characteristics of an object. The method called  `constructor()` is used to initialise the attributes of an object. Just as **methods** are functions defined in a class, attributes are variables defined in a class.

Each method in a class definition begins with a reference to the instance object. By convention, this is named 'this'.

In Javascript, the first parameter for methods is `this`. The `this` parameter is used to create member variables. Inside a class, we initialise any variables that might have different values depending on the specific instance of the class as `this.VariableName`. For the car example, we might want to access the `color` variable of `car_1` and the `color` variable of `car_2` and in order to assign each car its own `color` value, we need the `this`. 

The body of the constructor function for the example of person is as follows:

```javascript
this.name = name;
this.age = age;
this.gender = gender;
this.interests = interests;
```

This code creates member variables for the object that is created by the constructor. Member variables will begin with `this` to show that they are member variables belonging to the object, and not just regular local variables in the method. 

All put together, the class to describe a person looks like this:

```javascript
class Person {
  constructor(name, age, gender, interests) {
    
    this.name = name;
    this.age = age;
    this.gender = gender;
    this.interests = interests;
  }
```

### **Creating an Instance**

