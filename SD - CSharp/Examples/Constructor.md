#### Definition

**Constructor**

___
#### Syntax

**Syntax 1**
```c#
class ClassName
{
    public ClassName()
    {
        // Initialization code
    }
}
```

___
#### Examples

**Example 1**
```c#
class Person
{
    public string Name { get; set; }
    public int Age { get; set; }

    public Person(string name, int age)
    {
        Name = name;
        Age = age;
    }
}

Person person = new Person("John", 25);
```

___
[[Basic Concepts]]