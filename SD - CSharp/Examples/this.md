#### Definition

**this**
Refers to the current instance (object) of the class.

___
#### Syntax

**Syntax 1**
```c#
this.MemberName
```

___
#### Examples

**Example 1**
```c#
class Person
{
	public string Name { get; set; }

	public void Introduce(string name)
	{
		this.Name = name;

		Console.WriteLine(
			$"My name is {this.Name}"
		);
	}
}
```

___
[[Basic Concepts]]
