---
title: HtmlFragmentHighlighter
second_title: GroupDocs.Search for Java API Reference
description: Represents a search result highlighter that highlights search results in HTML formatted text fragments.
type: docs
weight: 11
url: /java/com.groupdocs.search.highlighters/htmlfragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)
```
public class HtmlFragmentHighlighter extends Highlighter
```

Represents a search result highlighter that highlights search results in HTML formatted text fragments.

**Learn more**

 *  [Highlighting search results][]

The example demonstrates a typical usage of the class.

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
 HtmlFragmentHighlighter highlighter = new HtmlFragmentHighlighter();
 index.highlight(document, highlighter, options);
 // Getting the result
 FragmentContainer[] fragmentContainers = highlighter.getResult();
 for (int i = 0; i < fragmentContainers.length; i++)
 {
     FragmentContainer container = fragmentContainers[i];
     String[] fragments = container.getFragments();
     if (fragments.length > 0)
     {
         System.out.println(container.getFieldName());
         System.out.println();
         for (int j = 0; j < fragments.length; j++)
         {
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
| [HtmlFragmentHighlighter()](#HtmlFragmentHighlighter--) | Initializes a new instance of the  HtmlFragmentHighlighter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getResult()](#getResult--) | Gets an array of resulting fragment containers. |
### HtmlFragmentHighlighter() {#HtmlFragmentHighlighter--}
```
public HtmlFragmentHighlighter()
```


Initializes a new instance of the  HtmlFragmentHighlighter  class.

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Gets an array of resulting fragment containers.

**Returns:**
com.groupdocs.search.common.FragmentContainer[] - An array of resulting fragment containers.
