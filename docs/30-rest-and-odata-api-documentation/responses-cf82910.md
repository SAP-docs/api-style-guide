<!-- loiocf829106a236487080a77c620ffb11be -->

# Responses

You provide information about the response statuses and returned data in the `Responses` object of each operation in the API description file.

Each possible response returned by an operation is defined by its properties, such as `HTTP status code`, `description`, `headers`, `schema`, and more.

You don't have to document all possible HTTP status codes, since they may not be known in advance, but cover the successful operation response and any known errors.

If the same response is used in a number of different operations or services within the same API, you can create a definition for this response once, and reference it where relevant. For more information, see [Components \(Definitions\)](components-definitions-81aaaff.md).

> ### Note:  
> For detailed information about the response properties, see [Responses Object](Responses Objecthttps://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#responses-object) in the OpenAPI Specification.



<a name="loiocf829106a236487080a77c620ffb11be__section_tbz_jxy_lz"/>

## How to Describe

 `description`: Add a short and meaningful description of the response code in the current operation. For example, code 204 has a generic meaning "No content", but for a specific operation it has a specific meaning, for example, "the product is out of stock", or "the order is not found".

We recommend supplying a meaningful description for the success code of the current operation, rather than just a generic "Successful operation".



## Example

```
responses:
        '204':
          description: The product is out of stock.
        '400':
          description: Wrong format or structure of the provided request body.
        '403':
          description: Access denied. You did not have the required permissions to access the resource.
        '404':
          description: |
            Not found. Possible reasons:

            - You provided a wrong URL.
            - The given task you are referring to does not exist.
            - You are not allowed to access the task.
        '422':
          description: The workflow context that was provided in the request body contained invalid keys or values.
        '500':
          description: Internal server error. The operation you requested led to an error during execution.
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

