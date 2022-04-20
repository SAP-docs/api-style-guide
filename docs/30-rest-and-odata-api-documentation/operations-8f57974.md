<!-- loio8f57974bc49449549e814f809152ae6e -->

# Operations

You provide information about resources, and operations on these resources, in the `Paths` property in the API description file.

Each operation or method is defined in its own `operation` object, including the path \(endpoint\), the HTTP method name, such as `GET` or `PUT`, the `description`, and a number of other objects and properties.

> ### Note:  
> For detailed information about these properties, see [Operation Object](Operation Objecthttps://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#operationObject) in the OpenAPI Specification.



<a name="loio8f57974bc49449549e814f809152ae6e__section_njg_1vy_lz"/>

## How to Describe

You describe an `operation` using the following properties:


<table>
<tr>
<th valign="top">

Property



</th>
<th valign="top">

Description



</th>
</tr>
<tr>
<td valign="top">

 `summary` 



</td>
<td valign="top">

A short summary of the operation. It appears in each operation's line in the *API References* view on SAP API Business Hub. This description should not be longer than 255 characters, the rest will be truncated.



</td>
</tr>
<tr>
<td valign="top">

 `description` 



</td>
<td valign="top">

An explanation of what the operation does, and its usage specifics, if any. It appears in the output when the operation line is expanded.

> ### Note:  
> Avoid starting the description with "this operation/method"; rather start directly with a verb in the third-person form: adds, creates, updates, sets, saves, reads, represents, gets, returns, deletes, and so on.

Do not repeat or start the description with the summary description. This description continues the explanation of what the operation does . If you do not need to provide more information, do not add a description.



</td>
</tr>
</table>



<a name="loio8f57974bc49449549e814f809152ae6e__section_k15_rdx_yz"/>

## Example

```

paths:
  /v1/task-instances:
    get:
      tags:
      - Task Instances
	 summary: Retrieves task instances.	
      description: Retrieves all active or completed task instances for a given workflow instance ID.
     
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

