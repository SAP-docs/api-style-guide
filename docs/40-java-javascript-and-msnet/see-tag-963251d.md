<!-- loio963251dea92b457fb1149b1ee73d0f30 -->

# <see\> Tag



## Description

An optional block tag that adds a reference link, and creates a See Also section in the documentation if one doesn’t already exist.



## Syntax

```
<see cref="class-or-interface-name[.member-name[(parameter1-name, ...)]]" />
```



## Guidelines

-   A parameter list is not required if the class member name is not overloaded.
-   `parameter1-name` is the first in a list of parameters that belong to the member name.
-   Order multiple `see` tags from constant to namespace, from the least-qualified to the fully-qualified signatures.



## Example

```
/// ...
/// <see cref="DownloadTableData"/>
/// <see cref="DBConnectionContext.GetDownloadData"/>       
/// ...
public interface DownloadData {
```

