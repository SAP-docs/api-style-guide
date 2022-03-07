<!-- loioe40c5b972e63457a8abf4ba0f871de64 -->

# Additional JavaScript Tags

A list of JavaScript tags, which are less commonly used in documentation comments, but are supported by the generation tools.



The following table contains the JavaScript tags that can include descriptions.


<table>
<tr>
<th valign="top">

Tag



</th>
<th valign="top">

Description



</th>
</tr>
<tr>
<td valign="top">

`@class` \(synonym: `@constructor`\)



</td>
<td valign="top">

Marks a function as being a constructor, which should be called with the `new` keyword to return an instance. This tag allows you to add a description of the class, rather than describe the constructor function. For example:

```
/**
    Creates a new Person.
    @class Represents a person. 
 */ 
Person = function() {
}
```



</td>
</tr>
<tr>
<td valign="top">

`@file` \(synonyms: `@fileoverview`, `@overview`\)



</td>
<td valign="top">

Includes the description of an entire file. Use this tag in a doc comment at the beginning of the file. For example:

```
/**
 * @file Contains functions related to documenting JavaScript.
 */
```



</td>
</tr>
<tr>
<td valign="top">

`@property` \(synonyms: `@prop`\)



</td>
<td valign="top">

Provides an easy way to document a list of static properties of a class, namespace, or other object. You must use this in the doc comments of a specific object For example, in a namespace with defaults and nested default properties:

```
/**
 * @namespace
 * @property {object}  defaults                The default values for parties
 * @property {number}  defaults.players        The default number of players
 * @property {string}  defaults.level          The default level for the party
 * @property {object}  defaults.treasure       The default treasure
 * @property {number}  defaults.treasure.gold  How much gold the party starts with
 */
var config = {
    defaults: {
        players: 1,
        level:   'beginner',
        treasure: {
            gold: 0
        }
    }
};

```



</td>
</tr>
</table>

For a complete reference of available JavaScript tags, see [External Resources](../external-resources-e019255.md).

**Related Information**  


[Java and JavaScript Tags](java-and-javascript-tags-6d32db8.md "A reference of the most commonly used Java and JavaScript block and inline tags that you can use in your documentation comments.")

