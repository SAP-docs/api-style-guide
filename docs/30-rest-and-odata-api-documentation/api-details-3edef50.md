<!-- loio3edef50b83134b6db51ea6ef3c9fca46 -->

# API Details

The *Details* section for each API provides important information to help developers understand its purpose.

The *Details* section for each API is written in the `info` object, and the `host`, `basePath`, `schemes`, `consumes`, and `produces` fields of the OpenAPI root document object.

> ### Note:  
> For detailed information about these fields, see [OpenAPI Object](OpenAPI Objecthttps://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#oasObject).



## How to Describe

The `artifact.json` object contains the following mandatory elements:


<table>
<tr>
<th valign="top">

Element



</th>
<th valign="top">

Description



</th>
</tr>
<tr>
<td valign="top">

 `title` 



</td>
<td valign="top">

The name of the API. Must not exceed 80 characters.



</td>
</tr>
<tr>
<td valign="top">

 `version` 



</td>
<td valign="top">

The version of the API. For example, 1.0.



</td>
</tr>
<tr>
<td valign="top">

 `x-sap-shortText` 



</td>
<td valign="top">

A high-level short description of the API that describes the exact purpose of the API in a maximum of 180 characters. This description appears in each of the API tiles, that can be seen in the API section of each package.



</td>
</tr>
<tr>
<td valign="top">

 `description` 



</td>
<td valign="top">

A long description \(one or two sentences\) of the API, which appears on the *Details* page of the API. It must not repeat the `x-sap-shortText`, but rather explain what the purpose of the API is in more detail.

> ### Caution:  
> If you don't add this description, the`x-sap-shortText` is used by default.



</td>
</tr>
<tr>
<td valign="top">

`contact`



</td>
<td valign="top">

You can add contact information at the API level.



</td>
</tr>
</table>



## Example

```
{
{openapi: 3.0.1
info:
  title: SAP Translation Hub
  description: To provide users of software in a global market with texts in their own language, translations are required. SAP Translation Hub enables you to draw on SAP's translation experience across multiple products and languages to propose translations for short texts.
version: 1.0

x-sap-shortText: Translate UI texts and get suggestions for UI texts during development.}
{contact: 
name: XXXX
url: https://api.sap.com/
email: xxxx@sap.com 
}
}

  
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

