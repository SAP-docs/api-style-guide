<!-- loiob3075650ec294e0e9d99edca25371c81 -->

# Package Pages

A template for documenting a package.

Add a file called `package.html` at the appropriate folder level of the source code to include Java package summary descriptions and information. This separate HTML file is the introduction or overview of the Java source files that are grouped together as a package.

> ### Remember:  
> It is mandatory to use this file.

Provide the following information in the package page file:

-   Purpose of the package
-   Overview of the content of the package
-   Background information needed to understand and use the package
-   Relationships between the classes in the package

The first sentence of the file is a summary description, similar to a doc comment.



```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"> 
    <html> 
        <head> 
            <meta http-equiv="content-type" content="text/html; 
              charset=windows-1250"> 
            <title>datafoundation</title> 
        </head> 
        <body> 
            <p>This package provides classes to create data foundations and 
                 manage objects for editing data foundations.</p>
            <p>The interfaces also provide methods to:
                <ul>
                    <li>Enable SQL options for the data foundation.</li>
                    <li>Set and get generic properties of the data foundation
                          objects (name, description, etc.).</li>
                    <li>...</li>
                </ul>
            </p> 
        </body> 
    </html>
```

