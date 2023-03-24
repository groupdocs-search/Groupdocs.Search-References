---
title: IFieldExtractor
second_title: GroupDocs.Search for Java API Reference
description: Provides methods for extracting fields from a document.
type: docs
weight: 39
url: /java/com.groupdocs.search.common/ifieldextractor/
---```
public interface IFieldExtractor
```

Provides methods for extracting fields from a document.

**Learn more**

 *  [Custom text extractors][]

The example demonstrates how to implement the interface.

```

 public class LogExtractor implements IFieldExtractor {
     private final String[] extensions = new String[] { ".log" };
 
     public final String[] getExtensions() { return extensions; }
 
     public final DocumentField[] getFields(String filePath) {
         File file = new File(filePath);
         DocumentField[] fields = new DocumentField[] {
             new DocumentField("FileName", file.getAbsolutePath()),
             new DocumentField("Content", extractContent(filePath)),
         };
         return fields;
     }
 
     private String extractContent(String filePath) {
         StringBuilder result = new StringBuilder();
         try {
             List lines = Files.readAllLines(Paths.get(filePath), StandardCharsets.UTF_8);
             for (int i = 0; i < lines.size(); i++) {
                 String line = lines.get(i);
                 String processedLine = line.substring(12);
                 result.append(processedLine);
             }
         } catch (IOException ex) {
             throw new RuntimeException(ex);
         }
         return result.toString();
     }
 }
 
```

The example demonstrates how to use the custorm extractor for indexing.

```

 String indexFolder = "c:\\MyIndex\\"; // Specify path to the index folder
 String documentsFolder = "c:\\MyDocuments\\"; // Specify path to a folder containing documents to search
 Index index = new Index(indexFolder); // Creating or loading an index
 index.getIndexSettings().getCustomExtractors().addItem(new LogExtractor()); // Adding custom text extractor to index settings
 index.add(documentsFolder); // Indexing documents from the specified folder
 
```


[Custom text extractors]: https://docs.groupdocs.com/display/searchjava/Custom+text+extractors
## Methods

| Method | Description |
| --- | --- |
| [getExtensions()](#getExtensions--) | Gets the supported extensions. |
| [getFields(String filePath)](#getFields-java.lang.String-) | Extracts all fields from the specified document. |
| [getFields(InputStream stream)](#getFields-java.io.InputStream-) | Extracts all fields from the specified document. |
### getExtensions() {#getExtensions--}
```
public abstract String[] getExtensions()
```


Gets the supported extensions.

**Returns:**
java.lang.String[] - The supported extensions.
### getFields(String filePath) {#getFields-java.lang.String-}
```
public abstract DocumentField[] getFields(String filePath)
```


Extracts all fields from the specified document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The document file path. |

**Returns:**
com.groupdocs.search.common.DocumentField[] - The extracted fields.
### getFields(InputStream stream) {#getFields-java.io.InputStream-}
```
public abstract DocumentField[] getFields(InputStream stream)
```


Extracts all fields from the specified document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The document stream. |

**Returns:**
com.groupdocs.search.common.DocumentField[] - The extracted fields.
