---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en utdataadapter som samlar utdata i ett java.io.OutputStream."
type: docs
weight: 31
url: /sv/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Representerar en utdataadapter som samlar utdata i ett java.io.OutputStream.


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Skapar en utdataström
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Skapar en strömutdataadapter
index.getDocumentText(documents[0], adapter); // Genererar dokumenttext till strömmen
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Initierar en ny instans av klassen  StreamOutputAdapter  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getStream()](#getStream--) | Hämtar en utdataström. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Initierar en ny instans av klassen  StreamOutputAdapter  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Utdataformatet. |
|
|  | ström | java.io.OutputStream | Utdataströmmen. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Hämtar en utdataström.


**Returns:**
java.io.OutputStream - Utdataströmmen.

