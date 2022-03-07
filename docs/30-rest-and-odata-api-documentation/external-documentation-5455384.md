<!-- loio5455384f6f1b4d44b83d6e5e7af18478 -->

# External Documentation

You can enhance your API reference documentation by providing links to external documentation.

You define the external links in the `externalDocs` object, which can be used on the root level for the entire API, or on the operation or tag level, as required.

> ### Note:  
> For more information about this object, see [External Documentation Object](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#externalDocumentationObject) in the OpenAPI Specification.



<a name="loio5455384f6f1b4d44b83d6e5e7af18478__section_a15_vwy_21b"/>

## How to Describe

You describe an external documentation using the following properties:


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

 `description` 



</td>
<td valign="top">

A short description of the external documentation.



</td>
</tr>
<tr>
<td valign="top">

 `url` 



</td>
<td valign="top">

The link to the external documentation, in URL format.



</td>
</tr>
</table>



## Example

```

externalDocs:
  description: SAP Workflow service Documentation
  url: https://help.sap.com/viewer/p/WORKFLOW_SERVICE
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

