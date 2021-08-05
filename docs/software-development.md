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

<table class="reference notranslate">
  <tr><th style="width:5%;">#</th><th style="width:45%;">Type</th><th>Patterns</th></tr>
  <tr><td>1</td><td><b>Creational Patterns</b><br />Create objects while hiding the creation logic, rather than instantiating objects directly using new operator.</td>
    <td>
    <ul>
      <li><a href="#/software-development?id=factory-pattern">工厂模式（Factory Pattern）</a></li>
    <li>抽象工厂模式（Abstract Factory Pattern）</li>
    <li>单例模式（Singleton Pattern）</li>
    <li>建造者模式（Builder Pattern）</li>
    <li>原型模式（Prototype Pattern）</li>
    </ul>
    </td>
  </tr>
  <tr><td>2</td><td><b>Structural Patterns</b><br />Class and object composition. Inheritance is used to compose interfaces and define ways to compose objects to obtain new functionalities. </td>
    <td>
      <ul>
        <li>适配器模式（Adapter Pattern）</li>
        <li>桥接模式（Bridge Pattern）</li>
        <li>过滤器模式（Filter、Criteria Pattern）</li>
        <li>组合模式（Composite Pattern）</li>
        <li>装饰器模式（Decorator Pattern）</li>
        <li>外观模式（Facade Pattern）</li>
        <li>享元模式（Flyweight Pattern）</li>
        <li>代理模式（Proxy Pattern）</li>
      </ul>
    </td>
  </tr>
  <tr><td>3</td><td><b>Behavioral Patterns</b><br /> Communication between objects </td>
    <td>
      <ul>
        <li>责任链模式（Chain of Responsibility Pattern）</li>
        <li>命令模式（Command Pattern）</li>
        <li>解释器模式（Interpreter Pattern）</li>
        <li>迭代器模式（Iterator Pattern）</li>
        <li>中介者模式（Mediator Pattern）</li>
        <li>备忘录模式（Memento Pattern）</li>
        <li>观察者模式（Observer Pattern）</li>
        <li>状态模式（State Pattern）</li>
        <li>空对象模式（Null Object Pattern）</li>
        <li>策略模式（Strategy Pattern）</li>
        <li>模板模式（Template Pattern）</li>
        <li>访问者模式（Visitor Pattern）</li>
      </ul>
    </td>
  </tr>
  <tr><td>4</td><td><b>J2EE Patterns</b><br />resentation tier(表示层)</td>
    <td>
      <ul>
        <li>MVC 模式（MVC Pattern）</li>
        <li>业务代表模式（Business Delegate Pattern）</li>
        <li>组合实体模式（Composite Entity Pattern）</li>
        <li>数据访问对象模式（Data Access Object Pattern）</li>
        <li>前端控制器模式（Front Controller Pattern）</li>
        <li>拦截过滤器模式（Intercepting Filter Pattern）</li>
        <li>服务定位器模式（Service Locator Pattern）</li>
        <li>传输对象模式（Transfer Object Pattern）</li>
      </ul>
    </td>
  </tr>
</table>

#### Factory Pattern
