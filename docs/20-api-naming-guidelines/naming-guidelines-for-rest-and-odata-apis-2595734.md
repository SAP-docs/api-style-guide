<!-- loio259573468585469f97651cfdfe0e4672 -->

# Naming Guidelines for REST and OData APIs

To make APIs intuitive and easy to use, name resources and parameters clearly and correctly.



<a name="loio259573468585469f97651cfdfe0e4672__section_mmq_zzz_khb"/>

## Language

Use correctly spelled American English words or combinations of them. Don't use words in other languages.



<a name="loio259573468585469f97651cfdfe0e4672__section_pry_l2z_tjb"/>

## Hierarchy of Resources and HTTP Methods

-   The hierarchy of resources in a URI should reflect relationships in the underlying data model.
-   A resource URI in combination with an HTTP method should make it easy to understand the meaning of an operation.

    > ### Example:  
    > -   *GET* `http://www.example.com/orders/{orderID}/items`
    > 
    >     Returns all items of a given order \(`orderID`\).
    > 
    > -   *POST* `http://www.example.com//orders/{orderID}/items`
    > 
    >     Creates a new item in a given order \(`orderID`\).




<a name="loio259573468585469f97651cfdfe0e4672__section_gqn_c11_lhb"/>

## Naming Conventions

-   camelCase is the preferred capitalization convention for resources and parameters \(REST APIs\) and for functions and actions \(OData APIs\). lowerCamelCase and UpperCamelCase are also possible.

    > ### Note:  
    > lowerCamelCase is the first letter isn’t capitalized and each subsequent word is capitalized. UpperCamelCase is the first letter of a word is capitalized and each subsequent word is too.

-   Separate resources in URIs with forward slashes.
-   Resource and parameter names are case-sensitive. So, a name in lowerCamelCase represents a different resource to the same name in UpperCamelCase.
-   Resources are concepts or objects that users want to control through HTTP requests. The requests address either a group of resources or a single resource. So, resources can be plural or singular.
-   Resource and parameter names should be meaningful, clear, and adequately describe the resource or parameter. Do not use abbreviations or acronyms.
-   Since a resource is an **object** rather than an action, use **nouns** rather than verbs. Resources should be plural.



<a name="loio259573468585469f97651cfdfe0e4672__section_ohr_pdr_mjb"/>

## Examples: Naming Conventions


<table>
<tr>
<th valign="top">

Example



</th>
<th valign="top">

Description



</th>
</tr>
<tr>
<td valign="top">

*GET* `http://www.example.com/customers/{customerID}/orders/{orderID}/items`



</td>
<td valign="top">

Returns all items of a given order \(`orderID`\) for a given customer \(`customerID`\).



</td>
</tr>
<tr>
<td valign="top">

*POST* `http://www.example.com/customers/{customerID}/orders/{orderID}/items`



</td>
<td valign="top">

Creates a new item in a given order \(`orderID`\) for a given customer \(`customerID`\).



</td>
</tr>
<tr>
<td valign="top">

`.../users/123/accountDetails`



</td>
<td valign="top">

The `users` and `accountDetails` resource names are lowerCamelCase.



</td>
</tr>
<tr>
<td valign="top">

 `.../Users/123/AccountDetails`



</td>
<td valign="top">

The `Users` and `AccountDetails` resource names are UpperCamelCase.



</td>
</tr>
<tr>
<td valign="top">

`.../products`



</td>
<td valign="top">

The `products` resource name is plural. A *GET* HTTP method on this URI retrieves a list of products.



</td>
</tr>
<tr>
<td valign="top">

`.../products/123/price`



</td>
<td valign="top">

The `price` resource name is singular. A *GET* HTTP method on this URI retrieves the price of product **123**.



</td>
</tr>
<tr>
<td valign="top">

```
{"id": "123",
 "productName": "Kitty Food",
 "productDescription": "Yummy!",
 "productPrice": {
 "value": 33.99,
 "currency":USD }
}
```



</td>
<td valign="top">

The request parameters are lowerCamelCase.



</td>
</tr>
<tr>
<td valign="top">

```
{"Id": "123",
 "ProductName": "Kitty Food",
 "ProductDescription": "Yummy!",
 "ProductPrice": {
 "Value": 33.99,
 "Currency":USD }
}
```



</td>
<td valign="top">

The request parameters are UpperCamelCase.



</td>
</tr>
</table>



<a name="loio259573468585469f97651cfdfe0e4672__section_kh5_krf_lhb"/>

## Examples: Parameter Names and Descriptions


<table>
<tr>
<th valign="top">

What to Avoid and Why



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

A mixture of lowerCamelCase and UpperCamelCase is inconsistent.



</td>
<td valign="top">

`/products?AvailableBy=2019-04-25`



</td>
<td valign="top">

`/products?availableBy=2019-04-25`



</td>
</tr>
<tr>
<td valign="top">

Ambiguous parameter names make the meaning unclear. Make the content and purpose of the parameter name more specific so that you don't have to rely on the description to convey the meaning.

Do not use abbreviations or acronyms.



</td>
<td valign="top">

Name: `exemptionReason`

Description: the exemption code \(string\)

Name: `user`

Description: user identifier \(string\)



</td>
<td valign="top">

Name: `exemptionReasonCode`

Name: `userId`



</td>
</tr>
<tr>
<td valign="top">

A mismatch between a parameter name and its description.



</td>
<td valign="top">

Name: `isTraceRequired`

Description: Shows whether tracing of the tax determination process is enabled.



</td>
<td valign="top">

Name: `isTraceEnabled` 



</td>
</tr>
<tr>
<td valign="top">

Incorrect word order is confusing.



</td>
<td valign="top">

`isCompanyDeferredTaxEnabled`



</td>
<td valign="top">

`isTaxDeferralEnabled`



</td>
</tr>
<tr>
<td valign="top">

Concatenation of parameter values instead of specific parameter names makes the meaning unclear and confusing.



</td>
<td valign="top">

`grossOrNet`

`netOrGross`



</td>
<td valign="top">

`amount`



</td>
</tr>
<tr>
<td valign="top">

Ambiguous abbreviations for parameter values are unclear and confusing.



</td>
<td valign="top">

The `grossOrNet` parameter has `g` and `n` values.



</td>
<td valign="top">

The `amount` parameter has `gross` and `net` values.



</td>
</tr>
<tr>
<td valign="top">

Don't use yes and no as values for Boolean parameters. Use enumerations if more choices are needed, for example: \(yes, probably, unlikely, and no\). Use numbers between 0 and 1 for fuzzy logic.



</td>
<td valign="top">

`isCashDiscountPlanned``: yes`



</td>
<td valign="top">

`isCashDiscountPlanned``: true`



</td>
</tr>
</table>

