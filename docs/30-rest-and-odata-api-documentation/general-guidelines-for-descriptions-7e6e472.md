<!-- loio7e6e4727d03a44d5a4e6244f1497a301 -->

# General Guidelines for Descriptions

Provide descriptions for the various API elements supported by the OpenAPI Specification.

Each API written using the Open API Specification has various elements, for example:

-   API Parameters
-   API Operations
-   API Responses

Each of these elements must be described, to ensure that the API consumer has a clear picture of what the API does. For example, when API consumers must enter a value for an API parameter, unless they understand what the parameter means, they’ll be unable to provide a suitable value.

The following applies to all descriptions:

-   Start description sentences with a capital letter, and end with a full stop.

-   Avoid describing implementation details and dependencies unless they’re important for usage.

-   Avoid repetitions and misplacements of information: for example, don't write about parameters in an operation description.




A good example of a description for an API parameter is in the [SAP Translation Hub](https://api.sap.com/api/translationhub/resource) API on the SAP API Business Hub. The parameter*Search* under the *Domains* operation is described as, "Shows whether a particular domain is available in SAP Translation Hub. Enter all or part of the short description of the domain, for example,`financial`.

-   **[Package Descriptions](package-descriptions-22c017a.md "SAP API Business Hub supports package descriptions. You write package descriptions in
		the package.json file, which is a part of each API deployment package. ")**  
SAP API Business Hub supports package descriptions. You write package descriptions in the `package.json` file, which is a part of each API deployment package.
-   **[API Details](api-details-3edef50.md "The Details section for each API  provides important information
		to help developers understand its purpose. ")**  
The *Details* section for each API provides important information to help developers understand its purpose.
-   **[Operations](operations-8f57974.md "You provide information about resources, and operations on these resources, in the
			Paths property in the API description file. ")**  
You provide information about resources, and operations on these resources, in the `Paths` property in the API description file.
-   **[Parameters](parameters-31c543a.md "You provide information about the request parameters in the
			Parameters object of each operation in the API
		description file.")**  
You provide information about the request parameters in the `Parameters` object of each operation in the API description file.
-   **[Responses](responses-cf82910.md "You provide information about the response statuses and returned data  in the
			Responses object of each operation in the API
		description file.")**  
You provide information about the response statuses and returned data in the `Responses` object of each operation in the API description file.
-   **[Components \(Definitions\)](components-definitions-81aaaff.md "If the same data type, parameter, or response are used in multiple operations within the
    same API or service, you can create a reusable component for each of them, and reference it
    where relevant across the API.")**  
If the same data type, parameter, or response are used in multiple operations within the same API or service, you can create a reusable component for each of them, and reference it where relevant across the API.
-   **[Security Scheme](security-scheme-9bf4fea.md "Control access to your business-critical APIs using security schemes. Provide
		information about these schemes in the
			securityDefinitions object in an API
		description file.")**  
Control access to your business-critical APIs using security schemes. Provide information about these schemes in the `securityDefinitions` object in an API description file.
-   **[Tags](tags-ebbdea3.md "You can define tags to group related operations by logical categories rather than just
		by resources.")**  
You can define tags to group related operations by logical categories rather than just by resources.
-   **[External Documentation](external-documentation-5455384.md "You can enhance your API reference documentation by providing links to external
		documentation. ")**  
You can enhance your API reference documentation by providing links to external documentation.

