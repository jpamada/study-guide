#### Definition

**Abstraction**
Hides complex logic. Similar to inheritance but can use policy.

___
#### Syntax

**Syntax 1**
A child class must implement abstract methods.
```c#
abstract class ParentClass
{
    public abstract void MethodName();

    public void AnotherMethod()
    {
        // Code
    }
}

class ChildClass : ParentClass
{
    public override void MethodName()
    {
        // Implementation
    }
}
```
___
#### Examples

**Example 1**
```c#
abstract class Animal
{
    public abstract void MakeSound();
}

class Dog : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Woof!");
    }
}

class Cat : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Meow!");
    }
}
```

___
[[Four Pillars of OOP]]
