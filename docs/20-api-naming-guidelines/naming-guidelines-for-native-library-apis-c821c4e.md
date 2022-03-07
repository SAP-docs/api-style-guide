<!-- loioc821c4e282724697a9220a13a9b4bcae -->

# Naming Guidelines for Native Library APIs

The naming conventions for common elements of Java, JavaScript, C/C++, Python, and .NET APIs.



<a name="loioc821c4e282724697a9220a13a9b4bcae__section_ozh_sd4_lhb"/>

## Guidelines


<table>
<tr>
<th valign="top">

Element



</th>
<th valign="top">

Rule



</th>
<th valign="top">

Example



</th>
</tr>
<tr>
<td valign="top">

Interface, class, constructor



</td>
<td valign="top">

Noun or noun phrase in UpperCamelCase. Interface names should start with a capital "I". Abstract classes should start with "Abstract".



</td>
<td valign="top">

`RuleDefinition`

`IProperty`

`AbstractProcessor`



</td>
</tr>
<tr>
<td valign="top">

Method



</td>
<td valign="top">

Verb or verb phrase, starting with a verb, in lowerCamelCase for Java and JavaScript, UpperCamelCase for .NET and C/C++.



</td>
<td valign="top">

`getCustomerAddress`

`LoadDataset`



</td>
</tr>
<tr>
<td valign="top">

Parameter



</td>
<td valign="top">

Noun or noun phrase in lowerCamelCase.



</td>
<td valign="top">

`userName` 



</td>
</tr>
<tr>
<td valign="top">

Constant



</td>
<td valign="top">

Combination of words in upper case, separated by an underscore.



</td>
<td valign="top">

`MAX_LENGTH`

`READ_WRITE`



</td>
</tr>
<tr>
<td valign="top">

Package \(Java\), namespace \(JavaScript\)



</td>
<td valign="top">

Lower case, dot-separated, unique combination of nouns, matching the package hierarchy. For Java: start with the reversed company domain name, for example: `com.sap`.



</td>
<td valign="top">

`com.sap.portal.directory`

`com.sap.mdm.data.commands`

`sap.ui.controller`



</td>
</tr>
<tr>
<td valign="top">

Namespace \(.NET\)



</td>
<td valign="top">

UpperCamelCase, dot-separated, unique combination of namespace components.



</td>
<td valign="top">

`Sap.Data.Hana`



</td>
</tr>
</table>



<a name="loioc821c4e282724697a9220a13a9b4bcae__section_nzx_4d4_lhb"/>

## Common Mistakes


<table>
<tr>
<th valign="top">

What to Avoid and Why



</th>
<th valign="top">

Incorrect



</th>
<th valign="top">

Improved



</th>
</tr>
<tr>
<td valign="top">

Too long names: difficult to read, understand, and use



</td>
<td valign="top">

`recalculateNodePresentationLayoutObjects()`



</td>
<td valign="top">

`recalculateNodeLayouts()`



</td>
</tr>
<tr>
<td valign="top">

Ambiguous names: confusing



</td>
<td valign="top">

`getData()`



</td>
<td valign="top">

`getAddress()`



</td>
</tr>
<tr>
<td valign="top">

Plurals inside combined names: grammatically incorrect



</td>
<td valign="top">

`ServicesProvider`

`getRecordsCount()`



</td>
<td valign="top">

`ServiceProvider` 

`getRecordCount()`



</td>
</tr>
<tr>
<td valign="top">

Ambiguous abbreviations: meaning is unclear and confusing



</td>
<td valign="top">

`ComProperty`

`IClientProviderAuth`



</td>
<td valign="top">

`ComponentProperty`

`IClientProviderAuthentication`



</td>
</tr>
<tr>
<td valign="top">

Product names: subject to change



</td>
<td valign="top">

`HiVoUserGroup`



</td>
<td valign="top">

`UserGroup`



</td>
</tr>
<tr>
<td valign="top">

Explaining implementation logic: doesn’t concern the user



</td>
<td valign="top">

`updateIfFound()`

`updateIfModified()`



</td>
<td valign="top">

`update()`



</td>
</tr>
<tr>
<td valign="top">

Mismatch between a name and its description: one of the two isn’t correct.



</td>
<td valign="top">

Name: `RetrieveLimitedRecordsCompoundEx`

Description: This command is responsible for retrieving set of records by record IDs



</td>
<td valign="top">

Name: `RetrieveRecordsByID` 

Description: Retrieves a set of records by their IDs



</td>
</tr>
<tr>
<td valign="top">

Incorrect order of words: confusing



</td>
<td valign="top">

`maxRowCountEnable()`



</td>
<td valign="top">

`enableMaxRowCount()`



</td>
</tr>
</table>

