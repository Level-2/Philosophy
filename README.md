Level-2
-------

Level-2 is a set of next-gen PHP libraries with a focus on lightweight extensible components that follows the X.org design principles

* Do not add new functionality unless an implementor cannot complete a real application without it.
* It is as important to decide what a system is not as to decide what it is. Do not serve all the world's needs; rather, make the system extensible so that additional needs can be met in an upwardly compatible fashion.
* The only thing worse than generalizing from one example is generalizing from no examples at all.
* If a problem is not completely understood, it is probably best to provide no solution at all.
* If you can get 90 percent of the desired effect for 10 percent of the work, use the simpler solution. (See also Worse is better.)
* Isolate complexity as much as possible.

These principles are frequently lost in the PHP community with authors often providing monstorous libraries with dozens of dependencies that try to do everything at the expense of clarity of vision and ease of use. Instead, Level-2 opts for smaller, extensible dependencyless libriaries that people can add features to *if they need them* rather than trying to cater to everyone's needs up front.

Level-2 focusses on *limited-scope* libraries that are easily extensible. This provides much clearer boundaries between what the libraries should and should not provide.

People often measure class size and complexity using metrics such as Cylcomatic Complexity and pat themselves on the back when they make a huge library that scores well for its individual classes ignoring the overall size of the library. There seems to be a "more is better" approach to writing code that ignores the complexity for the end user. Level-2 takes the idea of Cyclomatic Compelxity as a valuable metric and applies it to a library. Libraries should not need to be much over 300 total complexity.

A smaller library with fewer classes and methods means there is a far easier learning curve. Libraries can become insanely huge. Doctrine 2, for example is 369 classes and 2397 methods. That's a hell of a lot for someone using the library to take in. And that's ignoring Doctrine 2's dependencies! Maphper, Level-2's ORM on the other hand has a combined Cyclomatic Complexity of 197. That's 20 times lower yet it contains all the features you really need.

Level-2 is made up (currently) of the following libraries:

* Dice Dependency Injection Container (71 Cyclomatic Complexity, for comparison, PHP-DI is 401 and Laravel's Illuminate is 146)
* Maphper ORM - (197 cyclomatic complexity, for comparison Doctrine 2 is 4302)
* Vision Template Engine (35 Cyclomatic Complexity, for comparison Twig is 1286)
* Aphplication PHP Application server
* Axel Extensible Autoloader


