---
title: EnglishWordFormsProvider
second_title: GroupDocs.Search for Java API Reference
description: Represents an English word forms provider.
type: docs
weight: 17
url: /java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Represents an English word forms provider.

**Learn more**

 *  [Search for different word forms][]
 *  [Word forms provider][]


[Search for different word forms]: https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms
[Word forms provider]: https://docs.groupdocs.com/display/searchjava/Word+forms+provider
## Constructors

| Constructor | Description |
| --- | --- |
| [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Initializes a new instance of the  EnglishWordFormsProvider  class. |
## Methods

| Method | Description |
| --- | --- |
| [getWordForms(String word)](#getWordForms-java.lang.String-) | Gets the word forms for the specified word. |
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Initializes a new instance of the  EnglishWordFormsProvider  class.

### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Gets the word forms for the specified word. The resulting array does not contain the original word.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word to suggest the word forms. |

**Returns:**
java.lang.String[] - The word forms for the specified word or empty array if the  IWordFormsProvider  does not provide word forms for the specified word.
