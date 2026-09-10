#### Definition

**Properties**
Variables inside a class that store data.

___
#### Syntax

**Public Fields**
Typical syntax similar to Java
```c#
public dataType attributeName;
```

**Attributes**
Most common in C#
```c#
public dataType attributeName
{
  get; set;
}
```

___
#### Examples

**Example 1**
```c#
public string model;
public int year;
```

**Example 2**
```c#
public string model { get; set; }
public int year { get; set; }
```
___
[[Basic Concepts]]