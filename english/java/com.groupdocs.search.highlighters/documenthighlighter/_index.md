---
title: DocumentHighlighter
second_title: GroupDocs.Search for Java API Reference
description: Represents a search result highlighter that highlights search results in an entire document text.
type: docs
weight: 10
url: /java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)
```
public class DocumentHighlighter extends Highlighter
```

Represents a search result highlighter that highlights search results in an entire document text.

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
 // Search for the phase 'Theory of Relativity'
 SearchResult result = index.search("\"Theory of Relativity\"");
 // Highlighting found words in the text of a document
 FoundDocument document = result.getFoundDocument(0);
 OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
 Highlighter highlighter = new DocumentHighlighter(outputAdapter);
 index.highlight(document, highlighter);
 
```


[Highlighting search results]: https://docs.groupdocs.com/display/searchjava/Highlighting+search+results
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Initializes a new instance of the  DocumentHighlighter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getOutputAdapter()](#getOutputAdapter--) | Gets the output adapter passed in the constructor. |
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Initializes a new instance of the  DocumentHighlighter  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | The output adapter transferring a result of the highlighting. |

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Gets the output adapter passed in the constructor.

**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.
