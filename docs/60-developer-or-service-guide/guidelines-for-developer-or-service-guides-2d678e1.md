<!-- loio2d678e1f65414b36b2447e5344696414 -->

# Guidelines for Developer or Service Guides

To make developer or service guides easy to use and consistent, there are some best practices and guidelines to follow.



<a name="loio2d678e1f65414b36b2447e5344696414__section_bhy_jpw_sjb"/>

## Fundamental Information Design

Development guidelines cover many different technologies, platforms, and product areas. Therefore, it isn't possible to provide a template, so take a moment to consider the following points about the structure of your guide:

-   Create separate chapters for concepts, tasks, and reference information.
-   Apply a task-oriented approach to enable developers to accomplish tasks quickly and easily.
-   Use consistent title conventions for topics throughout the guide.

The following table shows the topic types used in developer guides and their title conventions.


<table>
<tr>
<th valign="top">

Topic Type



</th>
<th valign="top">

Content



</th>
<th valign="top">

Title Style



</th>
<th valign="top">

Example



</th>
</tr>
<tr>
<td valign="top">

Concept



</td>
<td valign="top">

Introduction, overview, background



</td>
<td valign="top">

Noun phrase



</td>
<td valign="top">

SAP HANA Cloud



</td>
</tr>
<tr>
<td valign="top">

Reference



</td>
<td valign="top">

API reference, tables, details



</td>
<td valign="top">

Noun phrase



</td>
<td valign="top">

SAP HANA Cloud JavaScript Reference



</td>
</tr>
<tr>
<td valign="top">

Task \(complex\)



</td>
<td valign="top">

Tutorial, multistep procedure with code samples



</td>
<td valign="top">

Gerund



</td>
<td valign="top">

Developing SAP HANA Cloud Applications



</td>
</tr>
<tr>
<td valign="top">

Task \(detailed\)



</td>
<td valign="top">

Single task with code samples



</td>
<td valign="top">

Gerund



</td>
<td valign="top">

Creating an Application Project



</td>
</tr>
</table>



<a name="loio2d678e1f65414b36b2447e5344696414__section_hdy_mpw_sjb"/>

## Choice of Content

Don't try to cover all of the APIs in your product. Work with your product owner \(PO\) to determine which APIs and their use cases are the most relevant for your consumers. Once you know the scope of your guide, bear in mind the following:

-   Don’t provide information that is already available on the SAP API Business Hub. The information you provide should give more in-depth information about your APIs.

-   Don't write a novel, keep the topics short and concise.
-   Provide only information that is relevant for your customers. Don't get sidetracked with internal implementation details.
-   Good diagrams help people to understand concepts. But don't make them too complex or clutter them with redundant details.

    > ### Note:  
    > If you reuse internal architectural diagrams, make sure that you adapt them for external customers.

-   For complex implementation tasks, use a tutorial format and break down the tasks into smaller chunks or subtopics.



<a name="loio2d678e1f65414b36b2447e5344696414__section_xfn_4pw_sjb"/>

## Code Samples

To explain specific tasks, provide code samples rather than lengthy explanations. Get code samples from developers, and make sure that they:

-   Compile without errors
-   Are short, and only contain code that illustrates the usage of the API
-   Contain enough comments to understand what is going on
-   Can be easily copied and pasted into a code editor

