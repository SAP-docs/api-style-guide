<!-- loio9bf4fea2546c4c368b068077ce0ade6c -->

# Security Scheme

Control access to your business-critical APIs using security schemes. Provide information about these schemes in the `securityDefinitions` object in an API description file.

`securityDefinitions` is a collection of individual `Security Scheme` objects. Each of the objects defines a security scheme for operations. A security scheme is defined by the name, description, type, and type-specific parameters. It can be applied for the whole API, or on the operation level.

The OpenAPI Specification currently supports the following security scheme types:

-   `basic`: User/password-based authentication.

-   `apiKey`: A key that must be included as part of every request either in a header, or in a query parameter.

-   `oauth2`: Used when the OAuth2 based authentication is required. In this case, additional parameters are defined, such as scopes.


> ### Note:  
> For detailed information about security definitions, see [Security Scheme Object](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#security-scheme-object) in the OpenAPI Specification.



<a name="loio9bf4fea2546c4c368b068077ce0ade6c__section_s4x_skt_21b"/>

## How to Describe

Enter a description of the security scheme, indicating the specifics of its usage in the `description` field. For example, on which level it should be applied, and how to obtain the credentials.



## Example

```

securityDefinitions:
  basicAuthentication:
    type: basic
  oauth2:
    type: oauth2
    description: >
      To use this API, you need to obtain the OAuth client credentials (client ID
      and secret) using the SAP HANA Cloud Platform cockpit. After that, pass these 
      client credentials to the SAP HANA Cloud Platform token endpoint to obtain an access token. 
    tokenUrl: >-
      https://api.hana.ondemand.com/oauth2/apitoken/v1?grant_type=client_credentials
    flow: application
    scopes:
      product_view: Read Product entities
      product_manage: Manage Product entities
```

**Related Information**  


[General Guidelines for Descriptions](general-guidelines-for-descriptions-7e6e472.md "Provide descriptions for the various API elements supported by the OpenAPI Specification.")

