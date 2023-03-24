---
title: IWordFormsProvider
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a word forms provider.
type: docs
weight: 23
url: /java/com.groupdocs.search.dictionaries/iwordformsprovider/
---```
public interface IWordFormsProvider
```

Defines interface of a word forms provider.

**Learn more**

 *  [Search for different word forms][]
 *  [Word forms provider][]

The following example demonstrates how to implement a custom word forms provider.

```

 public class SimpleWordFormsProvider implements IWordFormsProvider {
     public final String[] getWordForms(String word) {
         ArrayList result = new ArrayList();
         // Assume that the input word is in the plural, then we add the singular
         if (word.length() > 2 &&
             word.toLowerCase().endsWith("es")) {
             result.add(word.substring(0, word.length() - 2));
         }
         if (word.length() > 1 &&
             word.toLowerCase().endsWith("s")) {
             result.add(word.substring(0, word.length() - 1));
         }
         // Then assume that the input word is in the singular, we add the plural
         if (word.length() > 1 &&
             word.toLowerCase().endsWith("y")) {
             result.add(word.substring(0, word.length() - 1).concat("is"));
         }
         result.add(word.concat("s"));
         result.add(word.concat("es"));
         // All rules are implemented in the EnglishWordFormsProvider class
         return result.toArray(new String[0]);
     }
 }
 
```

The next example demonstrates how to set a custom word forms provider for using.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Setting the custom word forms provider instance
 index.getDictionaries().setWordFormsProvider(new SimpleWordFormsProvider());
 // Creating a search options instance
 SearchOptions options = new SearchOptions();
 options.setUseWordFormsSearch(true); // Enabling search for word forms
 // Searching in the index
 SearchResult result = index.search("relative", options);
 // The following words can be found:
 // relative
 // relatives
 
```


[Search for different word forms]: https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms
[Word forms provider]: https://docs.groupdocs.com/display/searchjava/Word+forms+provider
## Methods

| Method | Description |
| --- | --- |
| [getWordForms(String word)](#getWordForms-java.lang.String-) | Gets the word forms for the specified word. |
### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public abstract String[] getWordForms(String word)
```


Gets the word forms for the specified word. The resulting array does not contain the original word.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word to suggest the word forms. |

**Returns:**
java.lang.String[] - The word forms for the specified word or empty array if the  IWordFormsProvider  does not provide word forms for the specified word.
