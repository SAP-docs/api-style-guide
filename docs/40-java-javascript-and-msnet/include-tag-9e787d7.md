<!-- loio9e787d786c2e49b2b362361a6a382e7d -->

# <include\> Tag



## Description

You can place documentation comments into XML files instead of adding them to the source code. Use the `<include>` tag to reference the XML file and member to document in the source code.



## Syntax

```
<include file="file-name" path="tag-path[@name='member-name-reference']" />
```



## Guidelines

-   Use when all documentation is separated from the source code and placed in XML files.
-   Document all members of a class or interface in one XML file.
-   `file-name` is the name or path of the XML file containing the documentation.
-   `tag-path` is the path of the tags in `file-name` that leads to the tag name.
-   `member-name-reference` is the ID for the tag that precedes the comments. Refer to a class name as `class`, and refer to a constructor as `ctor`. If the constructor is overloaded, add a number to the member name, starting with 2. For example, a class that contains three overloaded constructors should be referenced as `ctor`, `ctor2`, and `ctor3`, respectively.



## Example

The following is a sample XML file named `ULCreateParms.xml`:

```
<?xml version="1.0" encoding="ISO-8859-1"?>
<doc>
    <member name="class">
        <summary>
            <para>Builds a string of creation-time options for creating an
            UltraLite database.</para>
        </summary>
        <remarks>
            <para>A ULCreateParms object is used to specify the parameters
            for creating a database with the ULDatabaseManager.CreateDatabase
           method.</para>
        </remarks>
    </member>
    ...
    <member name="TimeFormat">
        <summary>
            <para>Specifies the time format used for string conversions by the
            new database.</para>
        </summary>
        <returns>A string specifying the time format. If the value is a null
       reference (Nothing in Visual Basic), the database uses "HH:NN:SS.SSS". In
        C#, you must escape any backslash characters in paths or use @-quoted string
       literals. The default is a null reference (Nothing in Visual Basic).</returns>
    </member>
</doc>
```

The following is an excerpt of a header file that uses the `<include>` tag to reference documentation stored in `ULCreateParms.xml`:

```
namespace Sap.Data.UltraLite {
    ...
    /// <include file='ULCreateParms.xml' path='doc/member[@name="class"]/*'/>
    public class ULCreateParms {
        ...
        /// <include file='ULCreateParms.xml' path='doc/member[@name="TimeFormat"]/*'/>
        public string TimeFormat {
            ...
        }
        ...
    }
    ...
}
```

