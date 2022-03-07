<!-- loio5a8aea9c4f56440ea1b8f5b21ca11ce5 -->

# \\file Tag



## Description

Adds a description of a header file. This description is made up of two parts:

-   A mandatory summary sentence containing a short and exact description of the file
-   An optional detailed description that provides additional information



## Syntax

```
\file file-name
```



## Guidelines

-   This documentation comment is standalone. Place it anywhere in the specified header file.
-   `file-name` is optional.
-   `file-name` may include part of the path if the file name is not unique.



## Example

```
/** \file sacapi.h
 * Main API header file.
 * This file describes all the data types and entry points of the API.
 */
```

