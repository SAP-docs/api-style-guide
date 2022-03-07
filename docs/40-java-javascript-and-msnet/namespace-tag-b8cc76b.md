<!-- loiob8cc76bf92d4440e8b5cbef0dd6944f1 -->

# @namespace Tag



## Description

A JavaScript block tag indicating that an object is being used as a namespace to keep a collection of classes or properties and methods under a single global name. Use this tag to describe the functionality provided by the namespace.

**Applies to: *JavaScript*.**



## Syntax



### Syntax 1

```
/**
* @namespace description 
*/
var S = { ...
};
```



### Syntax 2

```
/** Description
* @namespace [{type}] [name]
*/
```



## Guidelines

-   Use syntax 1 if the comment block is followed by code that defines the namespace directly.
-   Syntax 2 is more suitable when the namespace is defined indirectly. The namespace type and name are optional. The name specified in the comment must match the name in the code.



## Examples



### Syntax 1

```
/**
 * @namespace Defines namespace for UI library
 */
var ui = {
    ...
};
```



### Syntax 2

```
/**
 * Defines namespace for UI library
 * @namespace sap.ui
 */
jQuery.sap.define(’sap.ui’); // defines the “sap” namespace indirectly if it does not already exist
```

**Related Information**  


[External Resources](../external-resources-e019255.md "A collection of links to useful external resources relevant for the topics addressed in this document.")

