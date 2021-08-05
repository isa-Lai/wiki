# SE

Design of Software

## Design Patterns

### Principles

1. **Open Close Principle（开闭原则）**
  Open for extension, but closed for modification.

2. **Liskov Substitution Principle（里氏代换原则）**
  If we substitute a superclass object reference with an object of any of its subclasses, the program should not break

3. **Dependence Inversion Principle（依赖倒转原则）**
  High-level modules should not depend on low-level modules. Both should depend on the abstraction.
  Abstractions should not depend on details. Details should depend on abstractions.
  Depend on Abstract not entity。

4. **Interface Segregation Principle（接口隔离原则）**
  No client should be forced to depend on methods it does not use.  ISP splits interfaces that are very large into smaller and more specific ones so that clients will only have to know about the methods that are of interest to them.

5. **Demeter Principle（迪米特法则/最少知道原则）**
  * Each unit should have only limited knowledge about other units: only units "closely" related to the current unit.
  * Each unit should only talk to its friends; don't talk to strangers.
  * Only talk to your immediate friends.

6. **Composite Reuse Principle（合成复用原则）**
  Classes should achieve polymorphic behavior and code reuse by their composition (by containing instances of other classes that implement the desired functionality) rather than inheritance from a base or parent class.
