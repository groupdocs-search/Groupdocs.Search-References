---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Ausgabeadapter dar, der die Ausgabe in einen java.io.OutputStream sammelt."
type: docs
weight: 31
url: /de/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Stellt einen Ausgabeadapter dar, der die Ausgabe in einen `java.io.OutputStream` sammelt.


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Einen Ausgabestream erstellen
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Einen Stream-Ausgabeadapter erstellen
index.getDocumentText(documents[0], adapter); // Dokumenttext in den Stream generieren
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Initialisiert eine neue Instanz der Klasse  StreamOutputAdapter . |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getStream()](#getStream--) | Gibt einen Ausgabestream zurück. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Initialisiert eine neue Instanz der Klasse  StreamOutputAdapter .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Das Ausgabeformat. |
|
|  | stream | java.io.OutputStream | Der Ausgabestream. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Gibt einen Ausgabestream zurück.


**Returns:**
java.io.OutputStream - Der Ausgabestream.

