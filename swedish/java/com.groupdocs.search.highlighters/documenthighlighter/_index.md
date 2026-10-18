---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en sökresultatmarkerare som markerar sökresultat i hela dokumenttexten."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Representerar en sökresultatmarkerare som markerar sökresultat i hela dokumenttexten.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Sök efter frasen 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Markering av hittade ord i texten i ett dokument
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Initierar en ny instans av klassen DocumentHighlighter. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Hämtar output‑adaptern som skickades in i konstruktorn. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Initierar en ny instans av klassen DocumentHighlighter.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Output‑adaptern som överför ett resultat av markeringen. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Hämtar output‑adaptern som skickades in i konstruktorn.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

