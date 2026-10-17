---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un adaptateur de sortie qui collecte la sortie dans un java.io.OutputStream."
type: docs
weight: 31
url: /fr/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Représente un adaptateur de sortie qui collecte la sortie dans un java.io.OutputStream.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
DocumentInfo[] documents = index.getIndexedDocuments(); // Obtention des informations sur les documents indexés
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Création d'un flux de sortie
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Création d'un adaptateur de sortie de flux
index.getDocumentText(documents[0], adapter); // Génération du texte du document dans le flux
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Initialise une nouvelle instance de la classe  StreamOutputAdapter  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getStream()](#getStream--) | Obtient un flux de sortie. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Initialise une nouvelle instance de la classe  StreamOutputAdapter  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Le format de sortie. |
|
|  | stream | java.io.OutputStream | Le flux de sortie. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Obtient un flux de sortie.


**Returns:**
java.io.OutputStream - Le flux de sortie.

