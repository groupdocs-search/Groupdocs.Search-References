---
title: CharacterReplacementDictionary
second_title: GroupDocs.Search for .NET API Reference
description: Represents a character replacement dictionary that is used during the indexing process. Character replacement can be used for example to remove accents from accented characters or to make caseinsensitive index.
type: docs
weight: 380
url: /net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Represents a character replacement dictionary that is used during the indexing process. Character replacement can be used, for example, to remove accents from accented characters or to make case-insensitive index.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Gets the number of Unicode code points contained in this [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Gets the dictionary type. |

## Methods

| Name | Description |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Adds the specified collection of character replacements to this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Adds the specified collection of character replacements to this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Adds the specified collection of character replacements to this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Adds the specified collection of Unicode code point replacements to this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Removes all character replacements from a [`CharacterReplacementDictionary`](../characterreplacementdictionary) object. |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Determines whether a [`CharacterReplacementDictionary`](../characterreplacementdictionary) object contains a replacement for the specified Unicode code point. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exports the dictionary to a file with the specified name. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Returns an enumerator that iterates through the collection. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Gets a replacement for the specified Unicode code point. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Imports a dictionary from the specified file. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Removes the specified collection of character replacements from this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Removes the specified collection of character replacements from this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Removes the specified collection of Unicode code points replacements from this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Removes the specified collection of Unicode code points replacements from this instance of the [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Remarks

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### See Also

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
