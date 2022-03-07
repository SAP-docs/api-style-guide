<!-- loio9e5ad0687a8346699632dcda65cbd7b4 -->

# <example\> Tag



## Description

An optional block tag that inserts an example section into a comment block.



## Syntax

```
<example>
    example-description 
    <code>
        example-code
    </code>
</example>
```



## Guidelines

-   Optional for all members, but recommended.
-   Place this tag after the `<remarks>` tag, if it exists. Otherwise, place it after the `<summary>` tag.
-   Write an example description to introduce the example code that illustrates the use of the API.
-   Enclose the example code in the `<code>` tag.
-   Optionally, add a sentence after the example code to describe its results.



## Example

```
/// ...
/// <example>
/// The following example illustrates how to initialize an SQLAConnection object:
/// <code>
/// SQLAConnection conn = new SQLAConnection( 
///     'UID=admin;PWD=money;SERVER=hr;DBN=policies' );
/// conn.Open();
/// </code>
///
/// The previous statement connects to a database named policies running on a server
/// named hr. The connection logs in with the user ID "admin" and the password "money".
/// </example>
/// ...

public SQLAConnection(string connectionString)

```

