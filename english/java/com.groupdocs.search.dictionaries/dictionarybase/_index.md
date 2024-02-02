---
title: DictionaryBase
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a dictionary.
type: docs
weight: 17
url: /java/com.groupdocs.search.dictionaries/dictionarybase/
---```
public interface DictionaryBase
```

Defines interface of a dictionary.

**Learn more**

 *  [Update index][].


[Update index]: https://docs.groupdocs.com/display/searchjava/Update+index
## Methods

| Method | Description |
| --- | --- |
| [getDictionaryType()](#getDictionaryType--) | Gets the dictionary type. |
| [exportDictionary(String filePath)](#exportDictionary-java.lang.String-) | Exports the dictionary to a file with the specified name. |
| [importDictionary(String filePath)](#importDictionary-java.lang.String-) | Imports a dictionary from the specified file. |
| [clear()](#clear--) | Clears the dictionary. |
### getDictionaryType() {#getDictionaryType--}
```
public abstract DictionaryType getDictionaryType()
```


Gets the dictionary type.

**Returns:**
[DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) - The dictionary type.
### exportDictionary(String filePath) {#exportDictionary-java.lang.String-}
```
public abstract void exportDictionary(String filePath)
```


Exports the dictionary to a file with the specified name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file to export to. |

### importDictionary(String filePath) {#importDictionary-java.lang.String-}
```
public abstract void importDictionary(String filePath)
```


Imports a dictionary from the specified file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file to import from. |

### clear() {#clear--}
```
public abstract void clear()
```


Clears the dictionary.

