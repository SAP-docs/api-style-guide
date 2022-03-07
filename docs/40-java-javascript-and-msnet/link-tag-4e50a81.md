<!-- loio4e50a817f7e04537b8ab5b413aa5f406 -->

# @link Tag



## Description

An optional inline tag that inserts a hyperlink pointing to the documentation of the specified package, class, interface, member, or to external packages, such as Java Platform SE APIs, or to any URL.

Can be used in any part of a comment block and in any tag.

**Applies to: *Java, JavaScript*.**



## Syntax



### Java

```
{@link #constant label}
{@link #constructor(Type, Type,...) label}
{@link #constructor(Type id, Type id,...) label}
{@link #method(Type, Type,...) label}
{@link #method(Type id, Type id,...) label}

{@link class label}
{@link class#constant label}
{@link class#constructor(Type, Type,...) label}
{@link class#constructor(Type id, Type id,...) label}
{@link class#method(Type, Type,...) label}
{@link class#method(Type id, Type id,...) label}

{@link package.class label}
{@link package.class#constant label}
{@link package.class#Constructor(Type, Type,...) label}
{@link package.class#Constructor(Type id, Type id,...) label}
{@link package.class#method(Type, Type,...) label}
{@link package.class#method(Type id, Type id,...) label}
{@link package label}
```



### JavaScript

```
{@link pathOrURL}
[label]{@link pathOrURL}
{@link pathOrURL|label}
{@link pathOrURL label}
```



## Guidelines

-   Even though the number of `{@link}` tags allowed in a comment is unlimited, use this tag sparingly to keep the comment easy to read. We recommend using this tag where it adds value, and only for the first occurrence of each API name in the doc comment.
-   Method parameter types are optional.
-   Optionally, specify a label to display in place of the URL.
-   In Java, use the HTML tag `<a href="...">link</a>` to link to external web sites.
-   In JavaScript, if you enter free text in a `@see` tag, add `@link` to create a hyperlink.



## Examples



### Java

```
/**
 * Returns a business item from its full path.
 *      
 * @param rootFolder the root item folder, retrieved with 
 *   {@link com.sap.sl.sdk.authoring.businesslayer.BusinessLayer#getRootFolder()}
 * @param path the item full path
 * @param failed if <code>true</code>, an exception is thrown (item not found)
 * @return A <code>BlItem</code> object
 * @see #getBlItemPath(BlItem)
 * @since 14.1.5
 */
BlItem getBlItem(RootFolder rootFolder, String path, boolean failed);
```



### JavaScript

```
/**
* Sets a string parameter used for CHAR, VARCHAR column types.
* ...
* This function does not convert data; to improve performance, it stores data directly in the database.
* Note that special characters (in Unicode SMP or SIP) can cause the read operation to fail. 
* For more information see {@link http://en.wikipedia.org/wiki/Plane_%28Unicode%29|Plane (Unicode)}.
* ...
* @param {integer} columnIndex The index of the parameter in the statement starting from 1
* @param {string} value The string value to be set for this parameter
* @throws Throws an error on invalid parameters.
* @throws {SQLException}
*/
$.db.CallableStatement.prototype.setString = function(columnIndex, value){};
```

**Related Information**  


[@see Tag](see-tag-844e853.md)

[Inline Java Tags](inline-java-tags-eac856d.md "A list of tags that you can use in any documentation comments, such as in the description or block tags.")

[HTML Tags](html-tags-bf50118.md "A reference of the HTML tags that you can use in documentation comments.")

