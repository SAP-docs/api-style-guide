<!-- loio7fa712a886e140f6ba974061028191b2 -->

# @deprecated Tag



## Description

A mandatory block tag indicating that the class, interface, or member is deprecated.

**Applies to: *Java, JavaScript*.**



## Syntax

```
@deprecated As of version NN, replaced by {@link class_name}
```



## Guidelines

Do not leave the tag comment empty. Provide the following information:

-   "As of" followed by the API version in which the class, interface or member was deprecated.
-   "replaced by" followed by a link \(`@link` tag\) to the replacing class or member.



You can provide additional information about the deprecation, but avoid mentioning any specific time frames for the phaseout.



## Example

```
/**
 * Returns the SELECT clause of a SQL query.
 * 
 * @return A <code>String</code> that contains the SELECT clause
 * @deprecated As of version 2.4, replaced by {@link NewClass#getSelect()}
 * <p>{@link #getNewClass()} allows you to retrieve a {@link NewClass} object.</p> 
 */
String getSelect();
```

**Related Information**  


[API Deprecation Policy](../api-deprecation-policy-65a10e3.md "Rules that address API deprecation and decommission their deliverables.")

