---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Ausgabeadapter dar, der Ausgaben in einer Datei sammelt."
type: docs
weight: 21
url: /de/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Stellt einen Ausgabeadapter dar, der Ausgaben in einer Datei sammelt.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen eines Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
DocumentInfo[] documents = index.getIndexedDocuments(); // Informationen zu indizierten Dokumenten abrufen
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Erstellen eines Datei-Ausgabeadapters
index.getDocumentText(documents[0], adapter); // Generieren eines Dokumenttexts in die Ausgabedatei
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Initialisiert eine neue Instanz der  FileOutputAdapter  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Ruft einen Ausgabedateipfad ab. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Initialisiert eine neue Instanz der  FileOutputAdapter  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Das Ausgabeformat. |
|
|  | filePath | java.lang.String | Der Ausgabedateipfad. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Ruft einen Ausgabedateipfad ab.


**Returns:**
java.lang.String - Der Ausgabedateipfad.

