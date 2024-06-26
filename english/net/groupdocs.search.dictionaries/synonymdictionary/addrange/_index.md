---
title: AddRange
second_title: GroupDocs.Search for .NET API Reference
description: Adds the specified collection of synonym groups to this instance of the SynonymDictionarygroupdocs.search.dictionaries/synonymdictionary.
type: docs
weight: 30
url: /net/groupdocs.search.dictionaries/synonymdictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Adds the specified collection of synonym groups to this instance of the [`SynonymDictionary`](../../synonymdictionary).

```csharp
public void AddRange(IEnumerable<string[]> synonyms)
```

| Parameter | Type | Description |
| --- | --- | --- |
| synonyms | IEnumerable`1 | The collection of synonym groups to add to the dictionary. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Thrown when *synonyms* is `null`. |
| ArgumentException | Thrown when number of synonyms in a group is less than 2. |

### See Also

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Adds the specified collection of synonym groups to this instance of the [`SynonymDictionary`](../../synonymdictionary).

```csharp
public void AddRange(string[][] synonyms)
```

| Parameter | Type | Description |
| --- | --- | --- |
| synonyms | String[][] | The collection of synonym groups to add to the dictionary. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Thrown when *synonyms* is `null`. |
| ArgumentException | Thrown when number of synonyms in a group is less than 2. |

### See Also

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
