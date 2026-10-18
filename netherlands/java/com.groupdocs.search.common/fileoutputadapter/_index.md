---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een output‑adapter voor die uitvoer in een bestand verzamelt."
type: docs
weight: 21
url: /nl/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Stelt een output‑adapter voor die uitvoer in een bestand verzamelt.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Een index maken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
DocumentInfo[] documents = index.getIndexedDocuments(); // Informatie ophalen over geïndexeerde documenten
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Een bestandsuitvoer‑adapter maken
index.getDocumentText(documents[0], adapter); // Een documenttekst genereren naar het uitvoerbestand
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Initialiseert een nieuw exemplaar van de  FileOutputAdapter  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Haalt een uitvoer‑bestandspad op. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Initialiseert een nieuw exemplaar van de  FileOutputAdapter  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Het uitvoerformaat. |
|
|  | filePath | java.lang.String | Het uitvoer‑bestandspad. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Haalt een uitvoer‑bestandspad op.


**Returns:**
java.lang.String - Het uitvoer‑bestandspad.

