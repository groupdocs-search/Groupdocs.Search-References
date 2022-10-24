---
title: StringOutputAdapter
second_title: GroupDocs.Search for Java API Reference
description: Represents an output adapter that collects output as a System.String.
type: docs
weight: 34
url: /java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)
```
public class StringOutputAdapter extends OutputAdapter
```

Represents an output adapter that collects output as a  System.String .

**Learn more**

 *  [Output adapters][]

The example demonstrates a typical usage of the class.

```
String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 DocumentInfo[] documents = index.getIndexedDocuments(); // Getting information on indexed documents
 StringOutputAdapter adapter = new StringOutputAdapter(); // Creating a string output adapter
 index.getDocumentText(documents[0], adapter); // Generating a document text into the adapter
 String result = adapter.getResult(); // Getting a result
```


[Output adapters]: https://docs.groupdocs.com/display/searchjava/Output+adapters
## Constructors

| Constructor | Description |
| --- | --- |
| [StringOutputAdapter()](#StringOutputAdapter--) | Initializes a new instance of the  StringOutputAdapter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getResult()](#getResult--) | Gets the resulting string. |
### StringOutputAdapter() {#StringOutputAdapter--}
```
public StringOutputAdapter()
```


Initializes a new instance of the  StringOutputAdapter  class.

### getResult() {#getResult--}
```
public final String getResult()
```


Gets the resulting string.

**Returns:**
java.lang.String - The resulting string.
