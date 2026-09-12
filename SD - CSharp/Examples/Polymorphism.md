#### Definition

**Polymorphism**
Allows the same method to behave differently depending on the object.

___

#### Syntax

**Syntax 1**
```c#
abstract class ParentClass
{
    public abstract 
	    ReturnType MethodName();
}

class ChildClass : ParentClass
{
    public override 
    ReturnType MethodName()
    {
        // Implementation
    }
}

ParentClass objectName = 
	new ChildClass();

objectName.MethodName();
```

___
[[Four Pillars of OOP]]