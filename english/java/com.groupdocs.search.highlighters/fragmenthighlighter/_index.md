---
title: FragmentHighlighter
second_title: GroupDocs.Search for Java API Reference
description: Represents a search result highlighter that highlights search results in text fragments.
type: docs
weight: 11
url: /java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Represents a search result highlighter that highlights search results in text fragments.

**Learn more**

 *  [Highlighting search results][]

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Search for the word 'Einstein'
 SearchResult result = index.search("Einstein");
 // Assigning highlight options
 HighlightOptions options = new HighlightOptions();
 options.setTermsBefore(5);
 options.setTermsAfter(5);
 options.setTermsTotal(15);
 // Highlighting found words in the text of a document
 FoundDocument document = result.getFoundDocument(0);
 FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
 index.highlight(document, highlighter, options);
 // Getting the result
 FragmentContainer[] fragmentContainers = highlighter.getResult();
 for (int i = 0; i < fragmentContainers.length; i++) {
     FragmentContainer container = fragmentContainers[i];
     String[] fragments = container.getFragments();
     if (fragments.length > 0) {
         System.out.println(container.getFieldName());
         System.out.println();
         for (int j = 0; j < fragments.length; j++) {
             // Printing HTML markup to console
             System.out.println(fragments[j]);
             System.out.println();
         }
     }
 }
 
```


[Highlighting search results]: https://docs.groupdocs.com/display/searchjava/Highlighting+search+results
## Constructors

| Constructor | Description |
| --- | --- |
| [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Initializes a new instance of the  FragmentHighlighter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getResult()](#getResult--) | Gets an array of resulting fragment containers. |
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Initializes a new instance of the  FragmentHighlighter  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | The output format. |

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Gets an array of resulting fragment containers.

**Returns:**
com.groupdocs.search.common.FragmentContainer[] - An array of resulting fragment containers.
