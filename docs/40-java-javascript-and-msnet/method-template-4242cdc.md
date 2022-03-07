<!-- loio4242cdc218fb42ac9a0bb5dd4b4e5343 -->

# Method Template

A template for documenting a method.



The documentation comment should provide the following information:

-   Background information needed to understand and use this method
-   Special considerations that apply to this method

Documentation comments for a method are made of a description and block tags. A description has a mandatory first sentence and optional additional sentences. Block tags are listed in a specific order, as shown below:



## Syntax

```
/**
 * Constructs/Returns/Sets/Displays/Adds/Removes/Creates/Releases/Other_verb the ...
 * <p>More information</p>
 *
 * @param param1_name A(n) <code>param1_type</code> object that ...
 * @param param2_name A(n) <code>param2_type</code> that ...
 * @return A(n) <code>method_type</code> object that ...
 * @throws exception_name If ...
 * @see
 * @since
 * @deprecated As of
 *             Replaced by {@link anotherMethod_name}
 */
public method_type method_name(param1_type param1_name, param2_type param2_type) throws exception_name;
```

The following table lists standard formulations to use for descriptions of different method types:


<table>
<tr>
<th valign="top">

Method Type



</th>
<th valign="top">

Verb to Use



</th>
</tr>
<tr>
<td valign="top">

Constructor



</td>
<td valign="top">

Constructs



</td>
</tr>
<tr>
<td valign="top">

Boolean



</td>
<td valign="top">

Indicates \(whether...\)



</td>
</tr>
<tr>
<td valign="top">

Getter



</td>
<td valign="top">

Returns/Retrieves/Gets



</td>
</tr>
<tr>
<td valign="top">

Setter



</td>
<td valign="top">

Defines/Sets



</td>
</tr>
<tr>
<td valign="top">

Other



</td>
<td valign="top">

Adds/Removes/Creates/Releases/Other verb that applies



</td>
</tr>
</table>

The description of a setter method should contain the default value of the property to be set, if necessary. If the property is set via a constructor, you should mention the default value in the description of the constructor.

> ### Note:  
> You can add snippets of codes to this template using the `<pre>` HTML tag inside paragraph tags.
> 
> ```
> * <p>For example:
> * <pre>
> * …
> * </pre>
> * </p>
> ```



## Constructor Example

```
/**
 * Constructs a new HTTP request.
 * 
 * @param logonToken A <code>String</code> used to log on to the session
 * @throws Exception If the object is not correctly initialized
 */
public Request(String logonToken) throws Exception {
    this.logonToken = logonToken;
}
```



## Accessor Example

```
/**
 * Returns the fully qualified table name that identifies a table.
 * <p>
 * The returned string is formatted as "qualifier"."owner"."tablename".
 * </p>
 * 
 * @param qualifier A <code>String</code> that represents the qualifier of the table
 * @param owner A <code>String</code> that represents the owner of the table
 * @param table A <code>String</code> that represents the name of the table
 * @return A <code>String</code> containing the fully qualified table name
 * @see #splitTableFullName(String)
 * @since 14.1.2
 */
String getTableFullName(String qualifier, String owner, String table);
```



## Setter Example

```
/**
 * Sets the column description.
 *
 * @param value A <code>String</code> that represents description of the column
 * @see #getDescription()
 */
public void setDescription(String value);
```



## Boolean Example

```
/**
 * Indicates whether the object is mandatory in the query.
 *
 * @return <code>true</code> if it is mandatory, <code>false</code> otherwise
 * @see #setMandatory(boolean)
 */
boolean isMandatory();
```



## General Method Example

```
/**
 * Creates a parameter.
 * <p>Example:
 * 
 * <pre>
 * Parameter parameter = businessLayerFactory.<b>createParameter</b>("field", object);
 * ...
 * </pre></p>              
 *                     
 * @param name A <code>String</code> that represents the parameter name
 * @param object An <code>Object</code> that represents the object to 
 *   which the parameter is attached
 * @return A new parameter
 * @since 14.1.2
 */
Parameter createParameter(String name, Object object);
```

**Related Information**  


[@deprecated Tag](deprecated-tag-7fa712a.md)

[@return Tag](return-tag-542ce73.md)

[@see Tag](see-tag-844e853.md)

[@since Tag](since-tag-74dc80d.md)

[@throws Tag](throws-tag-6488d75.md)

[Documentation Comments](documentation-comments-daea465.md "To generate the API reference, write documentation comments in the API source code according to specific rules.")

