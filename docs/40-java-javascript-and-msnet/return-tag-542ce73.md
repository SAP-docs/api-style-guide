<!-- loio542ce73bb2e045e0b50f29c82fd5abb1 -->

# @return Tag



## Description

A mandatory block tag that adds a description of the return value of a method or function to the Returns section.

**Applies to: *Java, JavaScript*.**



## Syntax



### Java

```
@return description
```



### JavaScript

```
@return {type1|type2|...} description
```



## Guidelines

-   Omit for constructors and for methods that return void.
-   Include for all other methods even when the description is obvious.
-   Use a noun phrase to describe the return value of the method.
-   Capitalize the first word with no hyphen before it.
-   Do not end with a period.
-   Describe all possible returned values, especially when the method returns `null` or a Boolean value \(`true` or `false`\).
-   Start the description with the data type of the return value, preceded by an article or a Boolean indicating success or failure.
-   In Java, wrap the result name with `<code>`...`</code>` in the noun phrase \(object name, returned type, `null`, or Boolean value\).
-   In JavaScript, document the multiple returned types, if any, using `{type1|type2|...}`.
-   In JavaScript, `description` is optional.



## Examples



### Java

```
/**
 * Returns the server port.
 *
 * @return An <code>int</code> specifying the server port
 */ 
public int getPort();
```

```
/**
 * Returns whether the object can be used as result object in the query.
 *
 * @return <code>true</code> if the object can be used, <code>false</code> otherwise
 */
boolean isUsableInResults();
```



### JavaScript

```
/**
 * Returns a resultset representing a table output parameter.
 *
 * @return {db.ResultSet} ResultSet of the next output table parameter
 */
$.db.PreparedStatement.prototype.getResultSet = function(){};
```

