---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een outputadapter voor die output verzamelt als een System.String."
type: docs
weight: 32
url: /nl/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Stelt een outputadapter voor die output verzamelt als een  System.String .


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Een string outputadapter maken
index.getDocumentText(documents[0], adapter); // Een documenttekst genereren in de adapter
String result = adapter.getResult(); // Een resultaat ophalen
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initialiseert een nieuw exemplaar van de  StringOutputAdapter  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getResult()](#getResult--) | Haalt de resulterende string op. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Initialiseert een nieuw exemplaar van de  StringOutputAdapter  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Het uitvoerformaat. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Haalt de resulterende string op.


**Returns:**
java.lang.String - De resulterende string.

