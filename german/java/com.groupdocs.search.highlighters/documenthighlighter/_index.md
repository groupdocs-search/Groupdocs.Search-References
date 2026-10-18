---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Suchergebnis-Hervorheber dar, der Suchergebnisse im gesamten Dokumenttext hervorhebt."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Stellt einen Suchergebnis-Hervorheber dar, der Suchergebnisse im gesamten Dokumenttext hervorhebt.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Suche nach der Phrase 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Hervorheben gefundener Wörter im Text eines Dokuments
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Initialisiert eine neue Instanz der  DocumentHighlighter  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Gibt den im Konstruktor übergebenen Output‑Adapter zurück. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Initialisiert eine neue Instanz der  DocumentHighlighter  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Der Output‑Adapter, der ein Ergebnis der Hervorhebung überträgt. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Gibt den im Konstruktor übergebenen Output‑Adapter zurück.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

