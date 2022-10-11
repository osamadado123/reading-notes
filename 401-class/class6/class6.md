# What are Design Patterns

A design pattern is only a description or template for how to solve a problem! that can be used in many different situations. So every design pattern provide a solution to commonly occurring software design problems. Patterns are formalized best practices that the Software Developer can use to solve common problems when designing an application.

## There is 3 major types of design patterns:

<ol>
<li>Creational Patterns: Creational patterns provide ways to instantiate single or groups of objects. Making it easier to create objects in a way that suits the situation.
<ul>
<li> Factory Method. The factory pattern is used to replace class constructors, abstracting the process of object generation so that the type of the object instantiated can be determined at run-time. </li>
<li>Singleton. The singleton pattern ensures that only one object of a particular class is ever created.</li>
<li>Abstract Factory. The abstract factory pattern is used to provide a client with a set of related or dependent objects.</li>
</ul>
</li>
<li> Structural Patterns : Structural patterns provide a manner to define relationships between classes or objects. Making it easier for these entities to work together.
<ul>
<li>Facade. The facade pattern is used to define a simplified interface to a more complex subsystem.</li>
<li> Adapter. The adapter pattern is used to provide a link between two otherwise incompatible types by wrapping the “adaptee” with a class that supports the interface required by the client.</li>
<li>Decorator. The decorator pattern is used to extend or alter the functionality of objects at run-time by wrapping them in an object of a decorator class.</li>
</ul> </li>
<li>Behavioral Patterns :
Behavioral patterns define manners of communication between classes and objects. Making it easier and more flexible for these entities to communicate.
<ul>
<li>Observer. The observer pattern is used to allow an object to publish changes to its state. </li>
<li>Mediator. The mediator pattern is used to reduce coupling between classes that communicate with each other.</li>
<li>Chain of Responsibility. The chain of responsibility pattern is used to process varied requests, each of which may be dealt with by a different handler.</li>
</ul></li>
</ol>

# Risk Analysis

## Why use Risk Analysis?
In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

## possible risks that you could encounter

<ol>
<li>Use of new hardware</li>
<li>Use of new technology</li>
<li>Use of new automation tool</li>
<li>The sequence of code</li>
<li>Availability of test resources for the application</li>
</ol>

## risks that are unavoidable
 <ol>
 <li>The time that you allocated for testing</li>
 <li>A defect leakage due to the complexity or size of the application</li>
 <li>Urgency from the clients to deliver the project</li>
 <li>Incomplete requirements</li>
 </ol>

## Risk Identification 
<ol>
<li>Business Risks : This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.</li>
<li>Testing Risks : You should be well acquainted with the platform you are working on, along with the software testing tools being used.</li>
<li>Premature Release Risk : a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required</li>
<li>Software Risks : You should be well versed with the risks associated with the software development process.</li>
</ol>

# Dependency Injection

## what is Dependency Injection
 transferring the task of creating the object to someone else and directly using the dependency is called dependency injection.


## types of dependency injection
<ol>
<li>constructor injection : the dependencies are provided through a class constructor.</li>
<li>setter injection : the client exposes a setter method that the injector uses to inject the dependency.</li>
<li>interface injection : the dependency provides an injector method that will inject the dependency into any client passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency.</li>
</ol>

## Benefits of using dependency injection
<ol>
<li>Helps in Unit testing.</li>
<li>Boiler plate code is reduced, as initializing of dependencies is done by the injector component.</li>
<li>Extending the application becomes easier.</li>
<li>Helps to enable loose coupling, which is important in application programming.</li>
</ol>

## Disadvantages of dependency injection
<ol>
<li>It’s a bit complex to learn, and if overused can lead to management issues and other problems.</li>
<li>Many compile time errors are pushed to run-time.</li>
<li>Dependency injection frameworks are implemented with reflection or dynamic programming. This can hinder use of IDE automation, such as “find references”, “show call hierarchy” and safe refactoring.</li>

</ol>