---
layout: post
title: Stupid or Solid
subtitle: Stupid or Solid?
tags: [blog, coding]
---

## Introduction
In today's post, I will be discussing the article **From STUPID to SOLID Code!"** by William Durand. The article discusses good and bad principles used in object-oriented programming. Although these principles are not laws, the author states that they are guidelines that every programmer should follow. 

## Reflection
Prior to reading this article, I was unaware that I have written STUPID code. The STUPID acronym stands for Singleton, Tight Coupling, Untestability, Premature Optimization, Indescriptive Naming, and Duplication. Mainly, I have unintentionally used singleton code, tight coupling, and premature optimization. Before reading this article, I had no idea that those habits were bad practices. The Singleton pattern only allows for a single instantion of a class. This becomes a problem when dealing with global states and is directly tied to tight coupling. Tight coupling forms strong dependencies between modules and makes testing extremely difficult. Premature Optimization is another anti pattern that results in unreadable and unusable code. However, I have to say that throughout my programming courses at the college, especially CSCI 221, I learned to stray away from indescriptive names, untestability, and duplication. I always make a point to give my variables, modules, objects, and classes descriptive names that are easy to understand. I find that this helps organize my code and prevents me from writing duplicated code. 

Likewise, I feel as though I have continuously followed the SOLID principles. The SOLID acronym stands for Single Responsibility, Open/Closed Principle, Liskov Substitution Principle, Interface Segregration Principle, and the Dependency Inversion Principle. In Java, we learned that each class should have their own specific responsibility. This would be what we call Single Responsibility. Meanwhile, the Open/Closed Principle states that the software you write should be open for extension, but closed for modification. Moreover, the member variables of each class should be private or at least protected. The Liskov Substitution Principle (LSP) "states that objects in a program should be replaceable with instances of their subtypes without altering the correctness of the program". This is important when dealing with super and subclasses as shown in the square and rectangle example in the article. Likewise, the Interface Segregation Principle (ISP) suggests that creating multiple specific interfaces are better than just one for general purposes. This practice enforces low coupling as well as high cohesion and organization. And lastly, the Dependency Inversion Principle (DIP) is made up of two main factors. The first being that abstractions shouldn't depend on details and the second being that details should depend on abstractions. This principle allows for the auto-wiring of classes and reduces dependency and makes code more reusable. 

## Conclusion
Without a doubt, every developer has their own personal style in terms of the way they write code. However, a uniformed list of guidelines will not only make it easier for people to become better at coding, but also enable more people to collaborate with each other. I feel as though these guidelines should be implemented in teaching code everywhere. After reading this article, I am now more aware of the differences between STUPID vs SOLID code and I definitely feel more inclined to write SOLID code. 




