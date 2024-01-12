# Kung-Fu-Panda
Game developed using Java where user catches plates to gain score point and avoid falling bombs and kunais that cost him hp.

# Table of Contents

1. [Kung-Fu-Panda](#Kung-Fu-Panda)
2. [Project Functionalities](#project-functionalities)
3. [Tools](#tools)
4. [Deployment](#deployment)
5. [Design Patterns](#design-patterns)
6. [S.O.L.I.D Principles](#solid-principles)
7. [Data Base](#data-base)
8. [Documentation](#documentation)
9. [Contributors](#contributors)
10. [Screenshots](#screenshots)

## Project Functionalities

1. User enters his name so his score can be saved in the database.
2. User moves roght and left to pick the falling object or prevent the bombs.
3. User can increase the difficulty of the game by increasing the speed of the projectiles or increase the intensity of bombs.

## Tools

1.IntelliJ IDEA (IDE)
2.Java
3.Java.swing
4.MySQL for database
5.Creately for UMLs diagrams
6.LaTeX for writing documentation

## Deployment

To run the program, you have to run the class named "CircusOfPlates.java" as your main class with Java SDK 16

## Design Patterns

1. Factory Design Pattern We have used Factory design patter in order to create new Objects without need of construction and to avoid coupling and dependency between Classes. So we constructed new instances of classes through this factory and returning it in needed methods or classes.

2. Prototype Design Pattern We have used Prototype design pattern by implementing “Cloneable” interface and implementing “clone()”method in each and every Shape class and also Cloning instances of “Point” class. It helped us making copies of our Objects using values not references that helped us in copy method.

3. Singleton Design Pattern We have used Singleton design pattern to assure the creation of only one object of “Score” class which has main aim to update the score table in the database and it is the only instance that is allowed to do such task.

4. Abstract Design Pattern We have used Abstract design pattern as it offers a simple interface to more complex underlying objects. So we could use draw methods using objects of “ShapeMakerFacade” class and not by accessing the shapes classes itself.

5. Iterator Design Pattern Iterator design Pattern facilitates looping across the array list of projectile object needed to be dropped.
   
6. Observer Design Pattern Observer design pattern helped us with automatic update the score in the database(update method) while playing (auto-documentation) as it takes the current score each and every time the game ends by only changing the state in the scoreObserver class.

7. State Design Pattern allows an object to alter its behavior when its internal state changes. The object will appear to change its class.

8. Strategy Design PatternDefine a family of algorithms, encapsulate each one, and make them interchangeable.

## S.O.L.I.D Principles

1. Single-Responsibility Principle A class should have one and only one reason to change, meaning that a class should have only one job, that's why we made classes like Bomb, Monkey, NinjaKnife and Plates. Those classes are only responsiple for one job as shown from their names.

2. Open-Closed Principle Objects or entities should be open for extension but closed for modification, so if anyone wants to contribute to project and add another shape, he can do so effortlessly by adding a class and extending it from "Droppable" class.


## Screenshots


![Screenshot 2023-03-09 140241](https://user-images.githubusercontent.com/97104406/224017962-74eaa96e-825b-4b2f-aa7a-eee6be49a531.png)
![Screenshot 2023-03-09 140302](https://user-images.githubusercontent.com/97104406/224018112-5951c6f2-060f-4cc6-a2b1-19a732b8d4d4.png)
![Screenshot 2023-03-09 140327](https://user-images.githubusercontent.com/97104406/224018133-91bd5ed5-5992-46bd-a5f2-e5dd6cbc192b.png)
