<!-- loio764cd6ada43c4ff0bfff3d8f10ef6676 -->

# API Naming Guidelines

Customers and partners find it easier to adopt APIs with names that are meaningful, clear, and self-explanatory. That’s why it’s important to use consistent naming conventions across all SAP APIs.



Even though developers often define the API names, you as a UA developer have an important role to play to ensure that these names:

-   Are written in professional and correct English.
-   Use correct terminology.
-   Are consistent, meaningful, and unambiguous.
-   Comply with the industry-wide naming conventions for the relevant language or technology.



<a name="loio764cd6ada43c4ff0bfff3d8f10ef6676__section_hhk_rhp_xjb"/>

## Word Combination Conventions



In many cases, a single word isn’t enough to convey the meaning of an API element, so a name is a combination of two or more words. Follow these conventions to combine words:



-   Case-separated words: lowerCamelCase or UpperCamelCase.
-   Words in lower case delimited by the underscore: `snake_case`.
-   Words in lower case delimited by the hyphen: `kebab-case`.

> ### Note:  
> None of these conventions is a definitive preferred industry standard, especially regarding the parameter and property names. Your choice largely depends on the English language in which the APIs are written.



## Acronyms

-   Avoid using acronyms in API names.
-   If you can't avoid acronyms, use only well-known ones, such as XML, SQL, DB, or ID, or acronyms that are known in the context of this API.
-   The development community hasn’t reached consensus on capitalization of acronyms. The most commonly used rules of capitalization are as follows:
    -   Two and three letters: capitalize everywhere except for the first word in lowerCamelCase.

        For example: `userID`, `getDBName`, `getURL`, `getSQLExpression`, `ioChannel`.

    -   Four and more letters: capitalize the acronym as would a word.

        For example: `HttpRequest`, `loadHtml`, `smtpServer`.





<a name="loio764cd6ada43c4ff0bfff3d8f10ef6676__section_fdd_hmn_sfb"/>

## A Unique Name for the API

Always refer to an API with a unique, easy to remember name throughout the documentation. The following rules can help to name the APIs and therefore to increase consistency of API names . These rules aren’t restrictive. Feel free to decide which rules to apply in the context of your API.


<table>
<tr>
<th valign="top">

Rule



</th>
<th valign="top">

Incorrect



</th>
<th valign="top">

Improved



</th>
</tr>
<tr>
<td valign="top">

Do not add "API" to the title.



</td>
<td valign="top">

 `Custom Forms APIs` 



</td>
<td valign="top">

 `Custom Forms` 



</td>
</tr>
<tr>
<td valign="top">

Use capitalized words. This is the preferred industry standard.



</td>
<td valign="top">

 `transaction monitoring` 



</td>
<td valign="top">

 `Transaction Monitoring` 



</td>
</tr>
<tr>
<td valign="top">

For simplicity, the name shouldn’t contain the language or the architecture style, like Java or REST, but only reflect the purpose or functionality of the API.



</td>
<td valign="top">

 `Supplier Data REST API` 



</td>
<td valign="top">

 `Supplier Data` 



</td>
</tr>
<tr>
<td valign="top">

Don’t use verbs, prepositions, and abbreviations.



</td>
<td valign="top">

`Configuring Portal`

`Portal Config.`



</td>
<td valign="top">

 `Portal Configuration` 



</td>
</tr>
<tr>
<td valign="top">

Avoid acronyms.



</td>
<td valign="top">

 `DB Connection` 



</td>
<td valign="top">

 `Data Access` 



</td>
</tr>
<tr>
<td valign="top">

Don’t add "SAP" to the API name. This is reserved for the product name.



</td>
<td valign="top">

 `SAP Document Approval` 



</td>
<td valign="top">

 `Document Approval` 



</td>
</tr>
</table>

> ### Note:  
> -   If an API is released as a service, make sure that the API name is different from the service name, to avoid confusion. For example, the service name is API Management. API Management has two entities associated with, namely API Portal, and API Business Hub Enterprise. The analytics APIs for these entities are then named, Analytics for API Portal, and Analytics for API Business Hub Enterprise. So the service and the APIs have different names, but are closely related.
> -   Don’t call an API a microservice. A microservice is a self-contained component of a system and application, which is meant to do only one thing. APIs and microservices aren’t the same, but can work together: A microservice uses an API to connect and communicate with the other parts of the system or with other microservices. The backend of an API can be deployed as a microservice on a system.

-   **[Naming Guidelines for REST and OData APIs](naming-guidelines-for-rest-and-odata-apis-2595734.md "To make APIs intuitive and easy to use, name resources and parameters clearly and
		correctly.")**  
To make APIs intuitive and easy to use, name resources and parameters clearly and correctly.
-   **[Naming Guidelines for Native Library APIs](naming-guidelines-for-native-library-apis-c821c4e.md "The naming conventions for common elements of Java, JavaScript, C/C++, Python, and .NET
		APIs. ")**  
The naming conventions for common elements of Java, JavaScript, C/C++, Python, and .NET APIs.

**Related Information**  


[External Resources](../external-resources-e019255.md "A collection of links to useful external resources relevant for the topics addressed in this document.")

