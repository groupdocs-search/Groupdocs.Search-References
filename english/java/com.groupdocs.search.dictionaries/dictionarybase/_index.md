---
title: DictionaryBase
second_title: GroupDocs.Search for Java API Reference
description: Represents the base class for a dictionary.
type: docs
weight: 15
url: /java/com.groupdocs.search.dictionaries/dictionarybase/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryBase
```

Represents the base class for a dictionary.

**Learn more**

 *  [Update index][].


[Update index]: https://docs.groupdocs.com/display/searchjava/Update+index
## Fields

| Field | Description |
| --- | --- |
| [ErrorOccurred](#ErrorOccurred) |  |
## Methods

| Method | Description |
| --- | --- |
| [exportDictionary(String filePath)](#exportDictionary-java.lang.String-) | Exports the dictionary to a file with the specified name. |
| [importDictionary(String filePath)](#importDictionary-java.lang.String-) | Imports a dictionary from the specified file. |
| [copyFrom(DictionaryBase other)](#copyFrom-com.groupdocs.search.dictionaries.DictionaryBase-) |  |
| [setFilePath(String filePath, boolean saveOnChange)](#setFilePath-java.lang.String-boolean-) |  |
### ErrorOccurred {#ErrorOccurred}
```
public final Event<Action1<String>> ErrorOccurred
```


### exportDictionary(String filePath) {#exportDictionary-java.lang.String-}
```
public final void exportDictionary(String filePath)
```


Exports the dictionary to a file with the specified name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file to export to. |

### importDictionary(String filePath) {#importDictionary-java.lang.String-}
```
public final void importDictionary(String filePath)
```


Imports a dictionary from the specified file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file to import from. |

### copyFrom(DictionaryBase other) {#copyFrom-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public void copyFrom(DictionaryBase other)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) |  |

### setFilePath(String filePath, boolean saveOnChange) {#setFilePath-java.lang.String-boolean-}
```
public void setFilePath(String filePath, boolean saveOnChange)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String |  |
| saveOnChange | boolean |  |

