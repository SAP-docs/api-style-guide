<!-- loioc866250dabed4680a80e8df607af10d0 -->

# Overview Page

A template for documenting a group of packages.



## Java

Add a file called `overview.html` at the appropriate source code folder level to include top-level specifications that apply to a group of related packages. This separate HTML file is like a cover sheet allowing you to quickly describe the content of the API documentation. Adding this file is not mandatory, but recommended.

Provide the following information in the overview page:

-   Purpose of the API
-   A list of the main features provided by the API
-   An overview of included packages
-   Links or text references to other API resources, such as developer guides, object model diagrams, or documents on the SAP Help Portal

The first sentence is a summary description, similar to a documentation comment.



```
<!DOCTYPE html>
<html>
    <head>
        <title>SAP BI Semantic Layer Java API Reference</title>
    </head>
    <body> 
        <p>The SAP BI Semantic Layer Java SDK allows you to develop a Java 
           application that performs creation and publication tasks on universes
           and associated resources (connections and profiles) on top of a 
           BI platform.</p>
        <p>The API is made of the <code>com.sap.sl.authoring</code> and
           <code>com.sap.sl.framework</code> packages, which provide a series
           of interfaces and classes used for developing your application.</p>
        <p>You use this API to develop the following main functionality for your 
           application: 
            <ul> 
                <li>Creating single-source data foundations</li> 
                <li>Creating multisource-enabled data foundations</li>
                <li>Publishing resources from the user local workspace to the CMS
                    repository</li>
                <li>...</li> 
            </ul>
        </p> 
        <p>For more information on the API, see the following documents on the 
           <a href="http://help.sap.com/bobip41">help portal</a>:
            <ul>
                <li><em>Information Design Tool User Guide</em></li>
                <li>BI Semantic Layer Java SDK Developer Guide</li>
            </ul>
        </p>
    </body>
</html>
```



## JavaScript

Add a file called `readme.md` in the appropriate source code folder to include top-level specifications that apply to a group of related packages. Write this file in Markdown. You can also use HTML tags. Adding this file is not mandatory, but recommended.



```
SAP HANA XS JavaScript Reference
================================

This API provides server-side JavaScript code running inside SAP HANA XS with access to request processing-related data and operations.

- [Request Processing API]($.web.html)
- [Database API]($.db.html)
- [HTTP Outbound API]($.net.http.html)
- [Trace API]($.trace.html)
- [Job Scheduling API]($.jobs.html)
- [Util API]($.util.html)
```

```
# SAP BusinessObjects Web Intelligence UI Extension Points
# JavaScript Reference

----------------
<br>
This API provides functions to set up the Web Intelligence DHTML or Java interface for interaction with documents and reports.

- [Web Intelligence Application API](WebiApplication.html)
  
  You can use these functions to interact with the Web Intelligence user interface.

- [Web Intelligence Service Document API](WebiServices.document.html)

  You can use these functions to interact with Web Intelligence documents and reports.
  
  These APIs make calls to the methods provided by the Web Intelligence RESTful Web Service SDK. The JSON
objects used as parameters or returned by these functions provide the same data than the JSON objects or XML streams that the
SDK methods can use as inputs or return. The XML streams are described in the SDK documentation. For
more information, see the *SAP BusinessObjects RESTful Web Service SDK User Guide for Web Intelligence and the
BI Semantic Layer* on the <a href="http://help.sap.com/saphelpiis_sbo41sp5wi-sdk/frameset.htm">help portal</a>.
```

**Related Information**  


[External Resources](../external-resources-e019255.md "A collection of links to useful external resources relevant for the topics addressed in this document.")

