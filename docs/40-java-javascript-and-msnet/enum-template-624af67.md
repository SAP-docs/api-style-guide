<!-- loio624af67b961548a8a41a0b0366c573bf -->

# Enum Template

A template for documenting an enumeration.



The documentation comment should provide the following information:

-   Background information needed to understand and use this enum
-   Special considerations that apply to the enum and values



## Syntax

```
/**
 * Provides...
 * or
 * An enumeration that provides... 
 * <p>More information</p>
 *
 */
public enum enum_name ...
{
    /**
     * Specifies/Defines/Is... or The...
     * <p>More information</p>
     *
     */
    enum_value,
}
```

Use this alternative syntax to provide the description of the enum value in a single line:

```
/** Specifies/Defines/Is... or The....    */
enum_value,
```



## Description

-   Start the description of the enum value with a verb \(third-person singular\) or a noun phrase. For example, "Allows " or "Provides".
-   Complete the description with additional information on a second line. It should clearly explain the behavior triggered by an enum value.



```
/**
 * Provides the statuses that can apply to a business security profile setting.
 */
public enum SecurityStatus implements InternalSecurityStatus {
	/** 
	 * Specifies that all elements are removed from a business security profile setting.
	 */
	UNSET(0, "Unset", "Unset"),

	/**
	 * Specifies that all elements are denied in a business security profile setting.
	 */
	DENIED(1, "Denied", "Denied"),

	/** 
	 * Specifies that all elements are granted in a business security profile setting.
	 */
	GRANTED(2, "Granted", "Granted");
     ... 
}
```

