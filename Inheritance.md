#### Definition

**Inheritance**
Allows a class to inherit properties and methods from another class.

___
#### Syntax

**Syntax 1**
```c#
```csharp
class BaseClass
{
  // properties and methods
}

class DerivedClass : BaseClass
{
  // Can use properties and
  // methods of BaseClass but
  // also create its own
}
```

___
#### Examples

**Example 1**
```c#
class Vehicle 
{
  public string Engine
  { 
    get; set; 
  }
  
  public void Start()
  {
    Console.Write("Engine Start");
  }
}

class Car : Vehicle
{
  // Inherits Engine property
  // and Start() method
}

Car myCar = new Car();
myCar.Start();
```

___
[[Four Pillars of OOP]]
