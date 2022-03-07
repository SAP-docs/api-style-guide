<!-- loio6488d755a6904effa896449b376d751e -->

# @throws Tag



## Description

A mandatory block tag that adds the description of the exception thrown when an error occurs during a method call. You must have one tag for every exception.

**Applies to: *Java, JavaScript*.**



## Syntax



### Java

```
@throws type description
```



### JavaScript

```
@throws {type} description
```



## Guidelines

-   Use a noun phrase \(standard sentence\) to describe the exception.
-   Capitalize the first word with no hyphen before it.
-   The exceptions should be listed alphabetically by exception name.
-   `type` is optional.



## Example



### Java

```
/**
 * Updates a database connection in the repository.
 * 
 * @param connection the connection to the database
 * @throws SDKException If an error occurs during the connection update
 * @see DatabaseConnection
 * @since 14.0.5
 */
void saveConnection(DatabaseConnection connection) throws SDKException;
```



### JavaScript

```
/**
 * Prepares a statement for execution.
 *
 * @param {string} statement The SQL statement to prepare
 * @return {$.db.PreparedStatement} A PreparedStatement object that represents
 *   the prepared statement
 * @throws {$.db.SQLException} Throws an error on invalid parameter
 */
$.db.Connection.prototype.prepareStatement = function(statement){};
```

