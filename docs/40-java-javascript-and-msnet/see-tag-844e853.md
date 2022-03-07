<!-- loio844e853c34044d16bf264603e7fe0873 -->

# @see Tag



## Description

An optional block tag that adds a reference to the See Also section. This reference can be:

-   A text entry with no link
-   A link defined by a URL
-   A link with a label to the documentation of the name that is referenced

**Applies to: *Java, JavaScript*.**



## Syntax



### Java

```
@see "free text"

@see <a href="URL#value">text</a>

@see package.class#member label
```

You can also use the following formats:

```
@see #constant
@see #constructor(Type, Type,...)
@see #constructor(Type id, Type id,...)
@see #method(Type, Type,...)
@see #method(Type id, Type id,...)

@see class
@see class#constant
@see class#constructor(Type, Type,...)
@see class#constructor(Type id, Type id,...)
@see class#method(Type, Type,...)
@see class#method(Type id, Type id,...)

@see package.class
@see package.class#constant
@see package.class#constructor(Type, Type,...)
@see package.class#constructor(Type id, Type id,...)
@see package.class#method(Type, Type,...)
@see package.class#method(Type id, Type id,...)
@see package
```



### JavaScript

```
@see path
@see free text
```



## Guidelines

-   In Java, if you enter free text, use double quotes to create a reference with no link in the See Also section. Add the `<a href="URL#value">` HTML tag to create a hyperlink. The `URL#value` is a relative or absolute URL.
-   In Java, `label` is optional.
-   In Java, `@see` tags are ordered from constant to package, from least-qualified to fully-qualified signature.
-   In JavaScript, if you provide a path, a hyperlink to the path is added automatically. If you provide a free text, add `@link` to create a hyperlink.



## Examples



### Java

```
/**
 * ...
 * @see Table
 * @see Table#getColumns()
 * @see TableColumn#setDataType(TableDataType) setDataType              
 * ...
 */
TableColumn createTableColumn(String name, Table table);
```



### JavaScript

```
/**
 * ...
 * @see setObject 
 * @see {@link setObject} for more information
 * @see {@link http://sap.help.com|the SAP Help Portal} for further information
 *
 */
function getObject(){};
```

**Related Information**  


[@link Tag](link-tag-4e50a81.md)

