---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een outputadapter voor die output verzamelt in een java.io.OutputStream."
type: docs
weight: 31
url: /nl/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Stelt een outputadapter voor die output verzamelt in een  java.io.OutputStream .


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Een outputstream maken
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Een stream-outputadapter maken
index.getDocumentText(documents[0], adapter); // Documenttekst genereren in de stream
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Initialiseert een nieuw exemplaar van de  StreamOutputAdapter  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getStream()](#getStream--) | Haalt een outputstream op. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Initialiseert een nieuw exemplaar van de  StreamOutputAdapter  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Het uitvoerformaat. |
|
|  | stream | java.io.OutputStream | De outputstream. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Haalt een outputstream op.


**Returns:**
java.io.OutputStream - De outputstream.

