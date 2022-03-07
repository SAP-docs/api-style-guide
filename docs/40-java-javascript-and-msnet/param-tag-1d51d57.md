<!-- loio1d51d574828042409e914967d2f9d313 -->

# @param Tag



## Description

A block tag that adds a parameter entry to the Parameters section of a method or function description. It is mandatory in method and constructor descriptions.

You must have one block tag for every parameter, even if the description is obvious.

**Applies to: *Java, JavaScript*.**



## Syntax



### Java

```
@param parameter-name parameter-description
```



### JavaScript

```
@param parameter-name
@param {parameter-type} parameter-name
@param {parameter-type} parameter-name parameter-description
@param {parameter-type} parameter-name=default-value parameter-description
@param {parameter-type} [optional-parameter-name] parameter-description
@param {parameter-type1|parameter-type2} parameter-name parameter-description
```



## Guidelines

-   Use a noun phrase to describe the value represented by the parameter.
-   For Java, the first letter of the first word in the description must be lowercase, with no hyphen before it.

    For JavaScript, the first letter of the first word must be uppercase.

    > ### Note:  
    > This is true for the common generation tools used at SAP, such as Javadoc, JSDoc and Doxygen, and depends on the way this tag is rendered in the output. For example, in generated Javadocs the description follows the parameter name on the same line, separated by a hyphen. If your API documentation is generated with a different tool, check the output to see the tag's rendering.

-   Do not end with a period.
-   Describe the default values and/or specific possible values.
-   For multiple parameters, include a separate tag for each parameter.
-   The order of tags should match the order of parameters in the method signature.

In addition, for JavaScript:

-   Enclose the parameter name in square brackets to mark it as optional.
-   Describe the multiple types of the parameter using a pipe \(|\) as a separator.
-   Use an asterisk in curly brackets \(\{\*\}\) to specify an arbitrary type.



## Example



### Java

```
/**
 * ...
 * @param term the search term
 * @param exact indicates whether to search for the exact term (default is true)
 * @param sortBy the field by which to sort
 * ...
 */ 
public string search(String term, Boolean exact, string sortBy);
```



### JavaScript with a simple type parameter

```
/**
 * ...
 * @param {string} statement The SQL statement to prepare
 * ...
 */
$.db.Connection.prototype.prepareStatement = function(statement){};
```



### JavaScript with an object parameter

```
/**
 * ...
 * @param {Object} obj The report
 * @param {integer} obj.id The selected report's ID
 * @param {integer} obj.pageNumber The selected page number 
 * ...
 */
WebiApplication.loadReport = function(obj) {
    parent.callImplementation(arguments, "loadReport");
};
```

