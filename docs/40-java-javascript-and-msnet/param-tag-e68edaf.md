<!-- loioe68edafb62bc4aa2b3922733a0eb2b88 -->

# <param\> Tag



## Description

A block tag that adds a parameter entry to the Parameters section of a method or function comment.



## Syntax

```
<param name="parameter-name">
    parameter-description
</param>

```



## Guidelines

-   Mandatory in method and function descriptions for each parameter, even if the description is obvious.
-   Order the tags to match the order of the parameters in the method signature.
-   Provide the necessary information about the parameter.
-   Describe the default values and/or specific possible values.
-   Capitalize the first word in the parameter description.



## Example

```
/// ...
/// <param name="term">The search term</param>
/// <param name="exact">Defines whether to search for the exact term (default is true)</param>
/// <param name="sortBy">The field by which to sort</param>
/// ...
public Search(string term, boolean exact, string sortBy);
```

