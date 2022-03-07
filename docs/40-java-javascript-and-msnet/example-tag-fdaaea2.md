<!-- loiofdaaea2ec1af4245be3ad383e8af04a1 -->

# @example Tag



## Description

An optional JavaScript block tag that inserts an example into a comment block.

**Applies to: *JavaScript*.**



## Syntax

```
@example title
...
```



## Guidelines

-   Add empty lines and indent code lines to make the comment easy to read.
-   Optionally, add a title to the example.
-   This tag can be used more than once in the same comment block.



## Examples



### With a title

```
/**
 * ...
 * @example To create a client
 * var client = new $.net.http.Client();
 *
 */
```



### Without a title

```
/**
 * ...
 * @example
 * // creates client
 * var client = new $.net.http.Client();
 * 
 * // where and what to send
 * var dest = $.net.http.readDestination("testApp", "myDestination");
 * var request = new $.net.http.Request($.net.http.GET, "/"); // new Request(METHOD, PATH)
 *
 */ 
```



### With indentations

```
/**
 * ...
 * @example
 * var id = myjob.schedules.add({
 *     description: "Added at runtime, run every 10 minutes",
 *     xscron: "* * * * * *\/10 0",
 *     parameter: {
 *         a: "c"
 *     }
 * });
```

**Related Information**  


[Custom or Legacy Java Tags](custom-or-legacy-java-tags-e12c967.md "A list of custom or legacy tags that appear in the Java API documentation.")

[HTML Tags](html-tags-bf50118.md "A reference of the HTML tags that you can use in documentation comments.")

