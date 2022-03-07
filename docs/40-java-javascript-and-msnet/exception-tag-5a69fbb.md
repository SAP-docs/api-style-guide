<!-- loio5a69fbbcdeec452ebf4e55cfe1f51665 -->

# <exception\> Tag



## Description

A mandatory block tag that adds the description of the exception thrown when an error occurs during a method call.



## Syntax

```
<exception cref="exception-name">
    exception-description
</exception>
```



## Guidelines

-   Required for each method that throws an exception.
-   List multiple exceptions alphabetically by the exception name.
-   Capitalize the first word of the description.



## Example

```
/// Updates a database connection in the repository.
/// 
/// <exception cref="System.FormatException">
/// Thrown when the given string is not in the correct format.
/// </exception>
/// ...
public static DateTimeWithTimeZone Parse( string val )
```

