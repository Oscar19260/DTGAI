# Design Patterns
Design patterns are typical solutions to commonly occurring problems in software design. They are like pre-made blueprints that you can customize to solve a recurring design problem in your code.

## What does the pattern consist of?
Most patterns are described very formally so people can reproduce them in many contexts. Sections that are usually present in a pattern description:
* __Intent__ of the pattern briefly describes both the problem and the solution.
* __Motivation__ further explains the problem and the solution the pattern makes possible.
* __Structure__ of classes shows each part of the pattern and how they are related.
* __Code example__ in one of the popular programming languages makes it easier to grasp the idea behind the pattern.

## Criticism of patterns
Most typical arguments against using patterns:
* __Kludges for a weak programming language__: Usually the need for patterns arises when people choose a programming language or a technology that lacks the necessary level of abstraction. In this case, patterns become a kludge that gives the language much-needed super-abilities.
> For example, the _Strategy pattern_ can be implemented with a simple anonymous (lambda) function in most modern programming languages.
* __Inefficient solutions__: Patterns try to systematize approaches that are already widely used. This unification is viewed by many as a dogma, and they implement patterns “to the letter”, without adapting them to the context of their project.
* __Unjustified use__: _If all you have is a hammer, everything looks like a nail_. This is the problem that haunts many novices who have just familiarized themselves with patterns. Having learned about patterns, they try to apply them everywhere, even in situations where simpler code would do just fine.

## Classification of patterns
Design patterns differ by their complexity, level of detail and scale of applicability to the entire system being designed.
All patterns can be categorized by their intent, or purpose. There are three main groups of patterns:

### Creational patterns
Provide object creation mechanisms that increase flexibility and reuse of existing code.
* #### [Factory Method / Virtual Constructor](https://refactoring.guru/design-patterns/factory-method)
    Provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created.
* #### [Abstract Factory](https://refactoring.guru/design-patterns/abstract-factory)
    Lets you produce families of related objects without specifying their concrete classes.
* #### [Builder](https://refactoring.guru/design-patterns/builder)
    Lets you construct complex objects step by step. The pattern allows you to produce different types and representations of an object using the same construction code.
* #### [Prototype / Clone](https://refactoring.guru/design-patterns/prototype)
    Lets you copy existing objects without making your code dependent on their classes.
* #### [Singleton](https://refactoring.guru/design-patterns/singleton)
    Lets you ensure that a class has only one instance, while providing a global access point to this instance.

### Structural patterns
Explain how to assemble objects and classes into larger structures, while keeping these structures flexible and efficient.
* #### [Adapter / Wrapper](https://refactoring.guru/design-patterns/adapter)
    Allows objects with incompatible interfaces to collaborate.
* #### [Bridge](https://refactoring.guru/design-patterns/bridge)
    Lets you split a large class or a set of closely related classes into two separate hierarchies—abstraction and implementation—which can be developed independently of each other.
* #### [Composite / Object tree](https://refactoring.guru/design-patterns/composite)
    Lets you compose objects into tree structures and then work with these structures as if they were individual objects.
* #### [Decorator / Wrapper](https://refactoring.guru/design-patterns/decorator)
    Lets you attach new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.
* #### [Facade](https://refactoring.guru/design-patterns/facade)
    Provides a simplified interface to a library, a framework, or any other complex set of classes.
* #### [Flyweight / Cache](https://refactoring.guru/design-patterns/flyweight)
    Lets you fit more objects into the available amount of RAM by sharing common parts of state between multiple objects instead of keeping all of the data in each object.
* #### [Proxy](https://refactoring.guru/design-patterns/proxy)
    Lets you provide a substitute or placeholder for another object. A proxy controls access to the original object, allowing you to perform something either before or after the request gets through to the original object.

### Behavioral patterns
Take care of effective communication and the assignment of responsibilities between objects.
* #### [Chain of Responsibility / CoR, Chain of Command](https://refactoring.guru/design-patterns/chain-of-responsibility)
    Lets you pass requests along a chain of handlers. Upon receiving a request, each handler decides either to process the request or to pass it to the next handler in the chain.
* #### [Command / Action, Transaction](https://refactoring.guru/design-patterns/command)
    Turns a request into a stand-alone object that contains all information about the request. This transformation lets you pass requests as a method arguments, delay or queue a request’s execution, and support undoable operations.
* #### [Iterator](https://refactoring.guru/design-patterns/iterator)
    Lets you traverse elements of a collection without exposing its underlying representation (list, stack, tree, etc.).
* #### [Mediator / Intermediary, Controller](https://refactoring.guru/design-patterns/mediator)
    Lets you reduce chaotic dependencies between objects. The pattern restricts direct communications between the objects and forces them to collaborate only via a mediator object.
* #### [Memento / Snapshot](https://refactoring.guru/design-patterns/memento)
    Lets you save and restore the previous state of an object without revealing the details of its implementation.
* #### [Observer / Event-Subscriber, Listener](https://refactoring.guru/design-patterns/observer)
    Lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.
* #### [State](https://refactoring.guru/design-patterns/state)
    Lets an object alter its behavior when its internal state changes. It appears as if the object changed its class.
* #### [Strategy](https://refactoring.guru/design-patterns/strategy)
    Lets you define a family of algorithms, put each of them into a separate class, and make their objects interchangeable.
* #### [Template Method](https://refactoring.guru/design-patterns/template-method)
    Defines the skeleton of an algorithm in the superclass but lets subclasses override specific steps of the algorithm without changing its structure.
* #### [Visitor](https://refactoring.guru/design-patterns/visitor)
    Lets you separate algorithms from the objects on which they operate.