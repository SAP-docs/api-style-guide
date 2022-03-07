<!-- loio35f6961ac1bc4ba3af2d5f3d518919d9 -->

# API Quality Checklist

A checklist for developers and UA developers who are responsible for API reference documentation to ensure that you deliver good quality APIs.

> ### Recommendation:  
> To make sure that you find as many issues as possible before publishing API reference documentation, ask different people to perform each part of the review.

There are some differences depending on the type of documentation that you work with. Expand the relevant section for more information.



<a name="loio35f6961ac1bc4ba3af2d5f3d518919d9__section_osb_gkz_mjb"/>

## Auto-Generated API Documentation

<a name="loio35f6961ac1bc4ba3af2d5f3d518919d9__table_pnb_dyv_sjb"/>1. Creating or Editing API Specification Files


<table>
<tr>
<th valign="top">

What?



</th>
<th valign="top">

Where to Get More Information, or Food for Thought



</th>
</tr>
<tr>
<td valign="top">

Have you used tags as required by the type of API that you're documenting?



</td>
<td valign="top">

-   REST and OData APIs for SAP API Business Hub: [Tags](../30-rest-and-odata-api-documentation/tags-ebbdea3.md)

-   Java, JavaScript, and MS.NET APIs: [Documentation Tags](../40-java-javascript-and-msnet/documentation-tags-4deb3c0.md)




</td>
</tr>
<tr>
<td valign="top">

Have you entered documentation comments?



</td>
<td valign="top">

-   REST and OData APIs for SAP API Business Hub: [General Guidelines for Descriptions](../30-rest-and-odata-api-documentation/general-guidelines-for-descriptions-7e6e472.md)

-   Java, JavaScript, and MS.NET APIs: [Documentation Comments](../40-java-javascript-and-msnet/documentation-comments-daea465.md)




</td>
</tr>
<tr>
<td valign="top">

Are the descriptions for each parameter clear and precise?



</td>
<td valign="top">

Put yourself in the reader's shoes: are the texts clear?



</td>
</tr>
<tr>
<td valign="top">

Have you used examples to illustrate complex concepts?



</td>
<td valign="top">

Put yourself in the reader's shoes: is a one-line generic description tangible enough?



</td>
</tr>
<tr>
<td valign="top">

Have you checked that your API doesn’t include sensitive or internal information?



</td>
<td valign="top">

Make sure that you don’t include sample payloads, internal server addresses, user IDs, or anything else that isn’t for public consumption.



</td>
</tr>
</table>

<a name="loio35f6961ac1bc4ba3af2d5f3d518919d9__table_o3f_q1w_sjb"/>2. Reviewing What You Created in API Specification Files


<table>
<tr>
<th valign="top">

What?



</th>
<th valign="top">

Where to Get More Information, or Food for Thought



</th>
</tr>
<tr>
<td valign="top">

Are the descriptions of similar elements consistent?



</td>
<td valign="top">

Does it look like everything was written by the same person or is it a mix of styles and levels of detail?



</td>
</tr>
<tr>
<td valign="top">

Are tags grouped and ordered consistently?



</td>
<td valign="top">

-   REST and OData APIs for SAP API Business Hub: [Tags](../30-rest-and-odata-api-documentation/tags-ebbdea3.md)

-   Java, JavaScript, and MS.NET APIs: [Documentation Tags](../40-java-javascript-and-msnet/documentation-tags-4deb3c0.md)




</td>
</tr>
<tr>
<td valign="top">

Has a UA developer reviewed all API names and descriptions?



</td>
<td valign="top">

If you aren't sure who your UA developer is, try asking your scrum master or product owner.

[API Naming Guidelines](../20-api-naming-guidelines/api-naming-guidelines-764cd6a.md)



</td>
</tr>
<tr>
<td valign="top">

Is all formatting correct and complete?



</td>
<td valign="top">

Take a critical look at the texts and formatting.



</td>
</tr>
<tr>
<td valign="top">

Is the documentation compiled completely and without errors?



</td>
<td valign="top">

Check if the documentation comments are generated accurately from the API source code.



</td>
</tr>
<tr>
<td valign="top">

Do all the links work?



</td>
<td valign="top">

Look at the links to ensure that they aren’t broken or not redirecting to an incorrect target.



</td>
</tr>
<tr>
<td valign="top">

Does the output look like you expected it to?



</td>
<td valign="top">

Look at your API specification and its elements to see if they look like and render in a way as you expected.



</td>
</tr>
</table>



<a name="loio35f6961ac1bc4ba3af2d5f3d518919d9__section_mbm_tkz_mjb"/>

## Manually Written API Documentation

-   Ensure that your documentation is complete by asking the following questions:
    -   Does each API element contain description and tags \(metadata used by operations\), or descriptions in the API definition file?
    -   Are all required tags, and optional tags where appropriate, present?
    -   Do the descriptions convey clear thought of purpose, functionality, and usage?
    -   Are examples and cross-references where appropriate, present?

-   Ensure that your documentation is correct and consistent by asking the following questions:
    -   Has a UA Developer reviewed all API names and descriptions?
    -   Are the scope, quantity, and style of descriptions consistent for all similar elements?
    -   Are the documentation tags grouped and ordered consistently?
    -   Is the HTML formatting used correctly and consistently?

-   Ensure that your documentation is published correctly by asking the following questions:
    -   Do all of the links open to the targeted page?
    -   Does the generated output look and work as expected?


**Related Information**  


[Manually Written REST and OData API Reference](../50-manually-written-rest-and-odata/manually-written-rest-and-odata-api-reference-49b7204.md "If the auto-generated API reference documentation does not match your product needs, or if you need to have the reference topics within your developer guide, you can manually document REST and OData APIs using the dedicated templates in the DITA CMS.")

[API Naming Guidelines](../20-api-naming-guidelines/api-naming-guidelines-764cd6a.md "Customers and partners find it easier to adopt APIs with names that are meaningful, clear, and self-explanatory. That’s why it’s important to use consistent naming conventions across all SAP APIs.")

[Tags](../30-rest-and-odata-api-documentation/tags-ebbdea3.md "You can define tags to group related operations by logical categories rather than just by resources.")

