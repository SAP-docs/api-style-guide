<!-- loio7485ffd6707c4607a1947aebcd0db2ec -->

# Interface and Class Template

A template for documenting an interface or class.



The description of an interface or class should include the following:

-   Background information needed to understand and use this interface or class.
-   Special considerations that apply to this interface or class.



## Classic API

A classic API is intended to be used by third-party developers in their applications.

```
/** 
 * Represents/Contains/Provides/Defines...
 * <p>More information</p>
 *
 */
public interface_name
{
}
```



## Service Provider Interface \(SPI\)

Unlike classic APIs, an SPI is not intended to be used by developers. It is defined by a development platform to be implemented or extended by a third-party application to provide a custom service.

```
/**
 * Implement a service for...
 * or
 * Provide an implementation of ...
 * or
 * Provide services for...
 * or
 * Extend this abstract class to ...
 * <p>More information</p>
 *  
 */
public abstract class_name
{
}
```

```
/**
 * A skeletal implementation that ...
 * or
 * Defines a set of behaviors for ...
 * or
 * This class provides an implementation of ...
 * <p>You need to implement ...</p>
 *  
 */
public abstract class_name
{
}
```



## Description

-   Start the description with a verb \(imperative form or indicative form with third-person singular\) or a noun phrase. For example, "Allows you" or "Enables you".
-   Complete the description with additional information on a second line.



<a name="loio7485ffd6707c4607a1947aebcd0db2ec__section_qqd_hrd_5cb"/>

## Examples



### Classic API

```
/**
 * Allows you to manage connections in Data Access Layer internal connection pool.
 * <p>Provides basic methods to manage connections in the context of the use
 * of the connection pool.</p>
 *
 * @see #ConnectionPool
 */
public interface Connection
{
} 
```





### SPI

```
/**
 * Implement the loading service.
 *
 */
public abstract class ServiceLoader
{
}
```

