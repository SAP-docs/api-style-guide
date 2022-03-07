<!-- loiof49a845693f54d9f94273862ddb3723d -->

# <remarks\> Tag



## Description

An optional block tag that starts the detailed description for a namespace, class, or interface, or any of their members.



## Syntax

```
<remarks>member-description</remarks>
```



## Guidelines

-   Place after the `<summary>` tag.
-   Use only to provide detailed information about the member that is not already mentioned in the summary.



## Example

```
/// ...
/// <remarks>
/// Your client application must have an active connection to a database server before it can call
/// this method. An exception is thrown when a database connection has dropped or does not exist.
/// </remarks>
/// ...
public bool Find(short numColumns)

```

