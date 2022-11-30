---
title: FileOutputAdapter
second_title: GroupDocs.Search for Java API Reference
description: Represents an output adapter that collects output into a file.
type: docs
weight: 23
url: /java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)
```
public class FileOutputAdapter extends OutputAdapter
```

Represents an output adapter that collects output into a file.

**Learn more**

 *  [Output adapters][]

The example demonstrates a typical usage of the class.

```
String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 DocumentInfo[] documents = index.getIndexedDocuments(); // Getting information on indexed documents
 FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Creating a file output adapter
 index.getDocumentText(documents[0], adapter); // Generating a document text into the output file
```


[Output adapters]: https://docs.groupdocs.com/display/searchjava/Output+adapters
## Constructors

| Constructor | Description |
| --- | --- |
| [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Initializes a new instance of the  FileOutputAdapter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getFilePath()](#getFilePath--) | Gets an output file path. |
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Initializes a new instance of the  FileOutputAdapter  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | The output format. |
| filePath | java.lang.String | The output file path. |

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Gets an output file path.

**Returns:**
java.lang.String - The output file path.
