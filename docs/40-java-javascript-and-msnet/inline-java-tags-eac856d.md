<!-- loioeac856db877b4544a130a208fed3d5ff -->

# Inline Java Tags

A list of tags that you can use in any documentation comments, such as in the description or block tags.




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

`{@code text}`



</td>
<td valign="top">

Displays text in a code font without interpreting the text as HTML markup or nested Javadoc tags. This allows you to use regular angle brackets instead of HTML entities \(`&lt;` and `&gt;`\) in doc comments.



</td>
</tr>
<tr>
<td valign="top">

`{@docRoot}`



</td>
<td valign="top">

Represents the relative path to the generated document's root directory from any generated page. Useful when you want to reference a file, such as a copyright page, from all generated pages.



</td>
</tr>
<tr>
<td valign="top">

`{@inheritDoc}`



</td>
<td valign="top">

Inherits documentation from the nearest inheritable class or implementable interface, into the current doc comment at this tag's location.



</td>
</tr>
<tr>
<td valign="top">

`{@link}`



</td>
<td valign="top">

Inserts a hyperlink with a visible text label pointing to the documentation of the specified package, class, or interface, or any of their members. For more information, see [@link Tag](link-tag-4e50a81.md).



</td>
</tr>
<tr>
<td valign="top">

`{@linkplain}` 



</td>
<td valign="top">

Identical to `{@link}`, except that the link's label is displayed in plain text instead of code font.



</td>
</tr>
<tr>
<td valign="top">

`{@literal text}`



</td>
<td valign="top">

Displays text without interpreting it as HTML markup or nested Javadoc tags.



</td>
</tr>
<tr>
<td valign="top">

`{@value [package.class#constant]}`



</td>
<td valign="top">

Displays the value of a constant.



</td>
</tr>
</table>

**Related Information**  


[Java and JavaScript Tags](java-and-javascript-tags-6d32db8.md "A reference of the most commonly used Java and JavaScript block and inline tags that you can use in your documentation comments.")

[External Resources](../external-resources-e019255.md "A collection of links to useful external resources relevant for the topics addressed in this document.")

