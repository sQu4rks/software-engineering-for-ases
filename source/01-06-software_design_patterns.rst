Software Design Patterns
========================

In software engineering, as in many other engineering disciplines, the same problem might occur in 
different projects. In order to not constantly reinvent the wheel and have some best-practices at 
hand, software design patterns (or software patterns) provide proven solutions to common problems 
in software engineering. 

The *de-facto* standard for design pattern is a book called *Design Patterns: Elements of Reusable Object-Oriented Software*
written by Erich Gamma, Richard Helm, Ralph Johnson and John Vlissides in 1994. The authors subsequently became 
known as "the gang of four" and design patterns are sometimes referred to by their position within the 
book (i.e. *(Gang of Four 1995:18)*). With over 500'000 copies sold this book can be counted amongst the 
most influential computer science books of all times. 

The gang of four differentiates three types of design patterns. 

* **Creational patterns** that create objects instead of directly instantiating them. An example would be the *Singleton Pattern* that only allows the creation of one object of a specific class.
* **Structural patterns** that compose objects to obtain new functionality. An example would be the *Proxy Pattern* that allows us to use a placeholder object, enforce access rights or reduce computational cost by caching results.
* **Behavioral patterns** that are concerned with communication between objects. An example would be the *Observer Pattern* that allows observer to subscribe to events occuring.
