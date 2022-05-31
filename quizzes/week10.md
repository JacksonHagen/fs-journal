# C# Fundamentals


**1.** What is the purpose of a `namespace`?
<!-- enter you answer in the space below -->
```
To declare the scope of the export
```
**2.** What is the difference between a `class` and a `struct`?
<!-- enter you answer in the space below -->
```
A class can have inherited properties and a struct cannot.
```
**3.** What is the method that returns an instance of a class, yet it has no return type?
<!-- enter you answer in the space below -->
```
constructor
```
## Example 1
```c#
abstract class Car
{
	...
  public virtual string Start()
  {
    return "Vroooom";
  }
}
```
**5.** In the example what is the access modifier of the `Start()` method?
<!-- enter you answer in the space below -->
```
public
```
**6.** In the example what is `string` an indication of?
<!-- enter you answer in the space below -->
```
the return type
```
**7.** In the example what is `abstract` preventing?
<!-- enter you answer in the space below -->
```
It is preventing the class from being instantiated
```
**8.** In the example what is the purpose of `virtual`?
<!-- enter you answer in the space below -->
```
To stop the method from being overwritten
```
**9.** Name four access modifiers:
<!-- enter you answer in the space below -->
```
public, internal, protected, private
```
**10.** If you set a class or method to private, what can access it?
<!-- enter you answer in the space below -->
```
Methods only within the same file
```