---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Ausgabeadapter dar, der die Ausgabe als System.String sammelt."
type: docs
weight: 32
url: /de/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Stellt einen Ausgabeadapter dar, der die Ausgabe als `System.String` sammelt.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Erstellen eines String-Ausgabeadapters
index.getDocumentText(documents[0], adapter); // Generieren eines Dokumenttexts in den Adapter
String result = adapter.getResult(); // Ergebnis abrufen
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initialisiert eine neue Instanz der Klasse StringOutputAdapter. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getResult()](#getResult--) | Liefert die resultierende Zeichenkette. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Initialisiert eine neue Instanz der Klasse StringOutputAdapter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Das Ausgabeformat. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Liefert die resultierende Zeichenkette.


**Returns:**
java.lang.String - Die resultierende Zeichenkette.

