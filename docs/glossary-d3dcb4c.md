<!-- loiod3dcb4c759b84ce7b71829307f527c98 -->

# Glossary

Terms and definitions used in the standards and guidelines.


<table>
<tr>
<th valign="top">

Term



</th>
<th valign="top">

Definition



</th>
</tr>
<tr>
<td valign="top">

API documentation comment



</td>
<td valign="top">

In Java, JavaScript, and .NET APIs, a documentation comment is the combination of a description and block tags written in API source code for generating API reference documentation. The description and block tags are written according to specific rules and are separated using delimiters.



</td>
</tr>
<tr>
<td valign="top">

API documentation generators



</td>
<td valign="top">

Tools that process source code to extract documentation comments and generate structured API reference documentation, such as the following widely used industry tools: Javadoc, JSDoc, Doxygen, and Swagger.



</td>
</tr>
<tr>
<td valign="top">

code snippet



</td>
<td valign="top">

Several lines of code that illustrate the usage of an API method or function. Code snippets are published in API reference information or in a developer guide.



</td>
</tr>
<tr>
<td valign="top">

code sample file



</td>
<td valign="top">

A file that illustrates a feature or series of features of the API. Delivered together with the API. For example, as part of an SDK.



</td>
</tr>
<tr>
<td valign="top">

demo application



</td>
<td valign="top">

A basic implementation of the API that demonstrates its main features. Demo applications are delivered as a project together with the API.



</td>
</tr>
<tr>
<td valign="top">

documentation tag



</td>
<td valign="top">

A tag in a documentation comment that instructs the generator how to format this part of the comment. Each generator recognizes its own set of tags, however there’s a subset of commonly used tags supported by most generators.



</td>
</tr>
<tr>
<td valign="top">

deprecated



</td>
<td valign="top">

An API or any of its elements that will no longer be supported in future releases, therefore not encouraged for use. Deprecated elements can’t be removed immediately from APIs, because this can break existing client code. Deprecation is a tool for ensuring smooth transition between API releases.

In the OpenAPI SpecificationI, the API and its elements must be deprecated using the `x-sap-stateInfo` attribute.



</td>
</tr>
<tr>
<td valign="top">

exception



</td>
<td valign="top">

An event that is generated when an error occurs during the execution of a method. Exceptions must be caught and handled by a calling application, therefore they need to be documented along with the method.



</td>
</tr>
<tr>
<td valign="top">

path



</td>
<td valign="top">

In the OpenAPI Specification, a path is an endpoint or a resource, such as `/users`, `/users{id}` that your API exposes. For each path, you define operations or HTTP methods that can be used to access it. In OpenAPI terms, path and resource are used interchangeably.



</td>
</tr>
<tr>
<td valign="top">

partner APIs



</td>
<td valign="top">

An API that is modeled by SAP partners for SAP customers and published on the SAP API Business Hub.



</td>
</tr>
<tr>
<td valign="top">

private APIs



</td>
<td valign="top">

An API is **private** or internal, if the access to it is limited to the vendor company and/or to its partners or selected customers.



</td>
</tr>
<tr>
<td valign="top">

public APIs



</td>
<td valign="top">

An API is public if it is available in the public domain.

Once released, an API becomes a contract between the vendor and its clients, so it shouldn’t be changed in a way that can break existing client code.



</td>
</tr>
<tr>
<td valign="top">

return type, value



</td>
<td valign="top">

A value of a certain data type that is returned by a method.



</td>
</tr>
<tr>
<td valign="top">

REST \(Representational State Transfer\) APIs



</td>
<td valign="top">

REST APIs, or RESTful Web Services, are cross-platform APIs used to perform CRUD \(Create, Read, Update, Delete\) operations on data resources over HTTP.



</td>
</tr>
<tr>
<td valign="top">

operation



</td>
<td valign="top">

In the OpenAPI Specification, an operation is an HTTP method such as `GET`, `PUT`, `POST`, that can be used to manipulate a path or an endpoint.



</td>
</tr>
<tr>
<td valign="top">

parameter



</td>
<td valign="top">

In the OpenAPI Specification, a parameter is an option that you can pass along with the path or an endpoint. For example, you pass the `userId` parameter along with the `/users` path and a `GET` operation to retrieve a user by numeric ID.



</td>
</tr>
<tr>
<td valign="top">

response



</td>
<td valign="top">

A response is a combination of HTTP status code and a description that describes the expected result of an API operation.In the OpenAPI Specification, each API operation must be associated with at least one response. A response is defined using an HTTP status code `200,` `400`, `401`, `404`, etc.



</td>
</tr>
<tr>
<td valign="top">

SPI \(Service Provider Interface\)



</td>
<td valign="top">

An interface defined by a vendor platform in order to be implemented or extended by a third-party application to provide a service.



</td>
</tr>
</table>

