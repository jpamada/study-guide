#### Definition

**Encapsulation**
Protects object's internal data and controlling how that data is accessed or modified.

___
#### Advantages

**Access Control**
Controls access to data through methods or properties

**Validation**
Can add validation when data is changed

___
#### Examples

**Without Validation**
```c#
public class Person
{
    public string Name { get; set; }
    public int Age { get; set; }
}
```
**With Validation**
```c#
class Person
{
    private int age;

    public int Age
    {
        get
        {
            return age;
        }

        set
        {
            if (value >= 0)
            {
                age = value;
            }
        }
    }
}
```

___
[[Four Pillars of OOP]]