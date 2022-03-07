<!-- loio00a8ec19a93e4bcf9219f3babce64a09 -->

# Constant Template

A template for documenting a constant.



The documentation comment should provide the following information:

-   Background information needed to understand and use this constant
-   Special considerations that apply to this constant



## Syntax

```
/**
 * Specifies/Defines/Is... or The...
 * <p>More information</p>
 *
 */
public static final constant_type constant_name = constant_value;
```

Use this alternative syntax to provide the description in one line:

```
/** Specifies/Defines/Is... or The....    */
public static final constant_type constant_name = constant_value;
```



## Description

-   Start the description with a verb \(third-person singular\) or noun phrase. For example, "Specifies" or "Defines".
-   Complete the description with additional information in a second line.



```
/**
 *  The password used to log in to the CMS.
 *  <p>This password must not contain any spaces.</p>
 */ 
static final String CMS_PASS = "YOUR PASSWORD";
```

```
/** The year of the date. */         
public short year;
```

