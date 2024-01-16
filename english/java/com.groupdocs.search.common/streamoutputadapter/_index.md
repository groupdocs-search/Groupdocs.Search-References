---
title: StreamOutputAdapter
second_title: GroupDocs.Search for Java API Reference
description: Represents an output adapter that collects output into a java.io.OutputStream.
type: docs
weight: 31
url: /java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Represents an output adapter that collects output into a  java.io.OutputStream .

**Learn more**

 *  [Output adapters][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 DocumentInfo[] documents = index.getIndexedDocuments(); // Getting information on indexed documents
 final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Creating an output stream
 StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Creating a stream output adapter
 index.getDocumentText(documents[0], adapter); // Generating a document text into the stream
 
```


[Output adapters]: https://docs.groupdocs.com/display/searchjava/Output+adapters
## Constructors

| Constructor | Description |
| --- | --- |
| [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Initializes a new instance of the  StreamOutputAdapter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getStream()](#getStream--) | Gets an output stream. |
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Initializes a new instance of the  StreamOutputAdapter  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | The output format. |
| stream | java.io.OutputStream | The output stream. |

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Gets an output stream.

**Returns:**
java.io.OutputStream - The output stream.
