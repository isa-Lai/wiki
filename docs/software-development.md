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
  
### Type of Design Patterns

| Type                                                                                                                                                                   | 包括                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 	**Creational Patterns** Create objects while hiding the creation logic, rather than instantiating objects directly using new operator. | * 工厂模式（Factory Pattern） * 抽象工厂模式（Abstract Factory Pattern） * 单例模式（Singleton Pattern） * 建造者模式（Builder Pattern） * 原型模式（Prototype Pattern） |
| **Structural Patterns** Class and object composition. Inheritance is used to compose interfaces and define ways to compose objects to obtain new functionalities.   | 适配器模式（Adapter Pattern） 桥接模式（Bridge Pattern） 过滤器模式（Filter、Criteria Pattern） 组合模式（Composite Pattern） 装饰器模式（Decorator Pattern） 外观模式（Facade Pattern） 享元模式（Flyweight Pattern） 代理模式（Proxy Pattern）  |
| **Behavioral Patterns** Communication between objects                                                                                                                       | 责任链模式（Chain of Responsibility Pattern） 命令模式（Command Pattern） 解释器模式（Interpreter Pattern） 迭代器模式（Iterator Pattern） 中介者模式（Mediator Pattern） 备忘录模式（Memento Pattern） 观察者模式（Observer Pattern） 状态模式（State Pattern） 空对象模式（Null Object Pattern） 策略模式（Strategy Pattern） 模板模式（Template Pattern） 访问者模式（Visitor Pattern） |
| **J2EE Patterns** Presentation tier(表示层)  | MVC 模式（MVC Pattern） 业务代表模式（Business Delegate Pattern） 组合实体模式（Composite Entity Pattern） 数据访问对象模式（Data Access Object Pattern） 前端控制器模式（Front Controller Pattern） 拦截过滤器模式（Intercepting Filter Pattern） 服务定位器模式（Service Locator Pattern） 传输对象模式（Transfer Object Pattern）           |
