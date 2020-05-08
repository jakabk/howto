#SOLID
#solid-principles
#SRP #single-responsibility
#OCP #open-closed
#LSP #liskov-substitution
#ISP #interface-segregation
#DIP #dependency-inversion


1) Single-responsibility
- you have only one job
- do one thing and do it well (UNIX philosophy)

2) Open-closed
- open for extension but closed for modification
- polymorphism
- prevents someone from changing already tried and tested code

3) Liskov Substitution
- parent/class should be replaceable with its derived/subclass

4) Interface Segregation
- no client should be forced to depend on methods it does not use
- do not add additional functionality to an existing interface by adding new methods

5) Dependency Inversion
- high-level modules should not depend on low-level modules, both should depend on abstractions
- abstractions should not depend on details. Details should depend on abstractions
- (dependency injection through the constructor)

- sources:
    - [scotch.io](https://scotch.io/bar-talk/s-o-l-i-d-the-first-five-principles-of-object-oriented-design)
    - [itnext.io](https://itnext.io/solid-principles-explanation-and-examples-715b975dcad4)
