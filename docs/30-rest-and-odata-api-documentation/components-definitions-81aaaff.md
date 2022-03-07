<!-- loio81aaafffe97d43a0a84583b15ba8fcb9 -->

# Components \(Definitions\)

If the same data type, parameter, or response are used in multiple operations within the same API or service, you can create a reusable component for each of them, and reference it where relevant across the API.

> ### Note:  
> Components is called Definitions in OpenAPI Specification, version 2.0.

All reusable objects appear under the `Definitions` object. A data type definition is a schema, identified by a name. It has a number of properties, such as `$ref`, `format`, `title`, `description`, `default`, and more, coming from the JSON Schema definition.

Definitions aren’t rendered in the output, so their descriptions are internal and optional.

> ### Note:  
> For detailed information, see [Definitions Object](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/2.0.md#definitionsObject) in the OpenAPI Specification.



<a name="loio81aaafffe97d43a0a84583b15ba8fcb9__section_rlz_ctp_d1b"/>

## Error Components Example

```

responses:
        '200':
          description: Returns a list of error messages.
          schema:
            $ref: '#/definitions/ErrorMessages'
...

definitions:
    ErrorMessages:
    items:
      properties:
        activityId:
          type: string
        activityName:
          type: string
        errorCode:
          type: string
        logId:
          type: string
        message:
          type: string
        timestamp:
          format: date-time
          type: string
      type: object
    type: array
```



## Schema Components Example

```

responses:
        '200':
          description: Returns a list of running and erroneous workflow instances.
          schema:
            $ref: '#/definitions/WorkflowInstanceList'
...
WorkflowInstanceList:
    items:
      properties:
        definitionId:
          type: string
        definitionVersion:
          type: string
        id:
          type: string
        startedAt:
          format: date-time
          type: string
        startedBy:
          type: string
        status:
          enum:
          - RUNNING
          - ERRONEOUS
          type: string
        subject:
          type: string
      type: object
    type: array
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

