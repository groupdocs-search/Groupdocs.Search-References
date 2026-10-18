---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoekresultaatmarkeerder voor die zoekresultaten markeert in de volledige documenttekst."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Stelt een zoekresultaatmarkeerder voor die zoekresultaten markeert in de volledige documenttekst.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Zoek naar de fase 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Markeren van gevonden woorden in de tekst van een document
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Initialiseert een nieuw exemplaar van de  DocumentHighlighter  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Haalt de output-adapter op die in de constructor is doorgegeven. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Initialiseert een nieuw exemplaar van de  DocumentHighlighter  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | De output-adapter die een resultaat van het markeren overdraagt. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Haalt de output-adapter op die in de constructor is doorgegeven.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

