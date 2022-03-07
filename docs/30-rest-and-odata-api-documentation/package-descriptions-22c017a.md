<!-- loio22c017ac31574d99abb9f0b9508f89e9 -->

# Package Descriptions

SAP API Business Hub supports package descriptions. You write package descriptions in the `package.json` file, which is a part of each API deployment package.



## How to Describe

The`package.json` file has the following descriptive fields:


<table>
<tr>
<th valign="top">

Name



</th>
<th valign="top">

Description



</th>
<th valign="top">

Example



</th>
</tr>
<tr>
<td valign="top">

Package title



</td>
<td valign="top">

The package title must reflect the product or product line to which the APIs belong to.

You can also combine the naming conventions with additional business-related information.

Don't use functionality for the package title. For example, Messaging API must not be the title of a package, but of a specific API within the package.

> ### Note:  
> If the product whose APIs are being packaged is still in the alpha or beta phase, then add a suffix to the package name with the terms Alpha and Beta in brackets, respectively. For example, **<ProductName\> \(Alpha\)** or **<Product Name\> \(Beta\)**.



</td>
<td valign="top">

-   SAP SuccessFactors Employee Central
-   SAP S/4HANA Cloud
-   SAP Leonardo Machine Learning Foundation - Functional Services




</td>
</tr>
<tr>
<td valign="top">

Short description



</td>
<td valign="top">

-   Summarize what the customer can achieve with the service in one sentence \(no more than 250 characters\). Start the sentence with an imperative \(such as "Create..." or "Build..."\).

-   Do not use a full stop at the end of the sentence.

-   Keep it short and simple, and convey the essence of the package briefly. Don’t repeat what the title already says.

-   Avoid phrases like "enables/allows you/use the service to do this...".

-   Don’t state the name of the package or use phrases like "on SAP BTP".

    Ideally this description is written by Product Management and reviewed by a UA developer.

    > ### Note:  
    > If you don’t provide a short description, the first 250 characters are taken from the overview description of your package. This could result in an incomplete sentence in the short description, so make sure that you write separate texts for the short and long descriptions.




</td>
<td valign="top">

-   Platform for all people and HR data that transforms your work experience
-   Translate UIs into more than 40 languages using SAP's translation experience
-   Simplify end-to-end process integration across cloud-based and on-premise applications



</td>
</tr>
<tr>
<td valign="top">

Overview description



</td>
<td valign="top">

-   This is a longer description, and it can be seen in the Details sections of the package. You can provide details about the package and its functionality.

    In 2-3 sentences, describe what the customer can achieve by using the service.

    -   Address the customer directly.
    -   Keep it short and simple. Don't use "...allows customers and partners to do this or that".

    > ### Note:  
    > Currently, Markdown formatting isn’t supported for package descriptions, but you can use \\n for line breaks.




</td>
<td valign="top">

SAP SuccessFactors Employee Central serves not only as a system of record for all people- and HR-related data, but also as a platform where everything in the organization comes together to transform the work experience. The HR organization can build value-based relationships with everyone supporting the business – engaging permanent and external workers to collaborate in new ways, using consumer-style tools and social HR.

It can help management design, plan, and implement better people strategies for better business results. One of the main strengths of SAP SuccessFactors Employee Central is its global and unmatched localized capabilities, ensuring legal and corporate compliance and taking into consideration local culture and people’s expectations for broad and seamless adoption.



</td>
</tr>
</table>

> ### Note:  
> Package descriptions appear prominently in the hub tile and in the landing page of every package. Hence, they should be written carefully and consistently with the product positioning. We recommend aligning with product management.



## Example

```

"shortText": "Orchestrate and extend workflows across people and organizations", 
"description": "Automate business processes using workflow technology. Build process extensions to SAP cloud applications or integrate with on-premises systems."
```

