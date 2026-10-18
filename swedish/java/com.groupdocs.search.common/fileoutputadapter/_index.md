---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en utdataadapter som samlar utdata i en fil."
type: docs
weight: 21
url: /sv/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Representerar en utdataadapter som samlar utdata i en fil.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
DocumentInfo[] documents = index.getIndexedDocuments(); // Hämtar information om indexerade dokument
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Skapar en filutdataadapter
index.getDocumentText(documents[0], adapter); // Genererar dokumenttext till utdatafilen
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Initierar en ny instans av klassen  FileOutputAdapter  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Hämtar en sökväg till utdatafilen. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Initierar en ny instans av klassen  FileOutputAdapter  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Utdataformatet. |
|
|  | filePath | java.lang.String | Utdatafilens sökväg. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Hämtar en sökväg till utdatafilen.


**Returns:**
java.lang.String - Utdatafilens sökväg.

