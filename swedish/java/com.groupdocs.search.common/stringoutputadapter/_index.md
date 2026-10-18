---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en utdataadapter som samlar utdata som en System.String."
type: docs
weight: 32
url: /sv/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Representerar en utdataadapter som samlar utdata som en System.String.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Skapar en strängutdataadapter
index.getDocumentText(documents[0], adapter); // Genererar dokumenttext i adaptern
String result = adapter.getResult(); // Hämtar ett resultat
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initierar en ny instans av klassen StringOutputAdapter. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getResult()](#getResult--) | Hämtar den resulterande strängen. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Initierar en ny instans av klassen StringOutputAdapter.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Utdataformatet. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Hämtar den resulterande strängen.


**Returns:**
java.lang.String - Den resulterande strängen.

