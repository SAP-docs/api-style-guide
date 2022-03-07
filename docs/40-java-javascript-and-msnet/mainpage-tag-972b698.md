<!-- loio972b6980a8d84d80ac7e0053674b0898 -->

# \\mainpage Tag



## Description

Adds a documentation comment to the `index.html` page or the first LATEX chapter of the generated output. This comment describes a group of packages as the `overview.html` file in Java.



## Syntax

```
\mainpage title
```



## Guidelines

-   This documentation comment is standalone. Place it anywhere in an existing header file, or in a separate header file created for documentation purposes.
-   `title` is optional and replaces the default title. Specify `notitle` if you don't want a title.



## Example

The `\mainpage` documentation comment is standalone and placed in an existing header file that describes a namespace.

```
/** \mainpage ConnectionServer Component C++ API Reference
 *
 * This is the detailed description.
 *
 * etc.
 */

/**
 * Defines the ConnectionServer namespace. 'CS' can be used as an alias for 'ConnectionServer'. 
 * The whole CS Public API declares its entities within this namespace.
 */ 
namespace ConnectionServer
{
...
}
```

