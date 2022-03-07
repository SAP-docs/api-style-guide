<!-- loio31c543a25bf64761a2a44afaace40410 -->

# Parameters

You provide information about the request parameters in the `Parameters` object of each operation in the API description file.



<a name="loio31c543a25bf64761a2a44afaace40410__section_hww_tgr_51b"/>

## Parameter Properties

Each parameter accepted by an operation is defined by the properties of the `parameter` object.

The `in` property defines the location in which the parameter is passed, and can have the following values:

-   `path`: The parameter value is part of the operation URL, not including the host or base path of the API. For example, `id` in `/items/{id}`.

-   `query`: The parameter is appended to the request URL. For example, `id` in `/items?id=###`.

-   `header`: The parameter is expected as a custom header of the request.

-   `body`: The parameter is the payload appended to the request. Limited to one per operation.

-   `formData`: The parameter is the payload appended to the request when either `application/x-www-form-urlencoded, multipart/form-data`, or both are used as the content type of the request.


The other parameter properties are `name`, `required`, and `description`.

If the same parameter is used in a number of different operations or services within the same API or service, you can create a definition for this parameter once, and reference it where relevant. For more information, see [Components \(Definitions\)](components-definitions-81aaaff.md).

> ### Note:  
> For detailed information about these properties, see [Parameter Object](Parameter Objecthttps://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#parameterObject) in the OpenAPI Specification.



<a name="loio31c543a25bf64761a2a44afaace40410__section_tbz_jxy_lz"/>

## How to Describe

Enter a short noun phrase describing the parameter in the `description` field. If applicable, describe usage specifics, for example, for different values. The description is rendered in a table column, so it keep it short and concise.



## Example

```
parameters:
      - description: The workflow instance ID for which the task instances are returned.
        in: query
        name: workflowInstanceID
        required: true
        type: string
		description:The XSRF token that is valid for the current session (see resource '/v1/xsrf-token').
        in: header
        name: X-CSRF-Token
        type: string
      - in: body
        name: body
        required: true
        schema:
          $ref: '#/definitions/CompleteTaskBody'
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

