<!-- loio37bf213d83ff4b8f90bd965f6537265b -->

# <returns\> Tag



## Description

A mandatory block tag that adds a description of the return value of a method or function to the Returns section.



## Syntax

```
<returns>returned-value-description</returns>
```



## Guidelines

-   Required for methods or functions that return values other than void.
-   Provide the necessary information about the returned value.
-   Capitalize the first word in the returned value description.



## Example

```
/// ...
/// <returns>True when the property was successfully set;
/// otherwise, returns false.</returns>
/// ...
public Boolean SetProperty(String name, String value)
```

