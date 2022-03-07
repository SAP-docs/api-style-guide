<!-- loio33a5538222af43b79d9d6f1390f9df9d -->

# Description

The description is mandatory in a documentation comment of a class, interface, class member, or interface member.



A description is usually made up of two parts:

-   A mandatory summary sentence containing a short description of the declared member.
-   An optional detailed description that provides additional information about this member.



## Guidelines

-   In the summary sentence, avoid clauses like "This class" or "This method".
-   For a member that represents an action, start with a verb in the third-person form: adds, allocates, constructs, converts, deallocates, destroys, gets, provides, reads, removes, represents, returns, sets, saves, and so on. For example:
    -   `Adds a new customer`
    -   `Provides read and write access to employee data`
    -   `Retrieves a Role object`

-   For a member that represents an object rather than an action, use a noun phrase. For example:
    -   `Base class for navigation`
    -   `Alias of a backend system`

-   Write a detailed description to provide additional information without repeating the API name and the summary sentence.
-   Avoid implementation details and dependencies unless they are important for usage.
-   To avoid line wrapping, make sure that each line of the description does not exceed 80 characters.
-   In the output, if the line breaks in a description are ignored, then it appears as one block of text. Use HTML tags to avoid this.
-   Use the `code` tag to emphasize language keywords, API names, and code examples in a description.



## Syntax

**Java and JavaScript** 

Only the summary sentence ending with a period appears in the summary section of a generated reference. Everything after this first period is cut off, so make sure that you write this sentence to make it stand on its own.

> ### Code Syntax:  
> Java
> 
> ```
> /**
>  * This is the summary sentence.
>  * <p>
>  * This is the detailed description. Note that you can have
>  * multiple sentences in the detailed description.
>  * </p>
>  * 
>  */
> ```

**.NET**

The summary sentence and detailed description are enclosed by the dedicated `<summary>` and `<remarks>` tags. To format descriptions, use the `<para>` tag.

> ### Code Syntax:  
> .NET
> 
> ```
> <summary>
>     <para>This is the summary sentence.</para>
> </summary>
> <remarks>
>     <para>This is the detailed description.</para>
> 	<para>Note that you can have multiple sentences in the detailed description.</para>
> </remarks>
> ```

**Related Information**  


[Java and JavaScript Tags](java-and-javascript-tags-6d32db8.md "A reference of the most commonly used Java and JavaScript block and inline tags that you can use in your documentation comments.")

[.NET Tags](net-tags-f882a72.md "A reference of the .NET tags that you can use in documentation comments.")

[HTML Tags](html-tags-bf50118.md "A reference of the HTML tags that you can use in documentation comments.")

[External Resources](../external-resources-e019255.md "A collection of links to useful external resources relevant for the topics addressed in this document.")

