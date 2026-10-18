---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca nell'intero testo del documento."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca nell'intero testo del documento.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Cerca la frase 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Evidenzia le parole trovate nel testo di un documento
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Inizializza una nuova istanza della classe DocumentHighlighter. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Ottiene l'adapter di output passato nel costruttore. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Inizializza una nuova istanza della classe DocumentHighlighter.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adapter di output che trasferisce un risultato dell'evidenziazione. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Ottiene l'adapter di output passato nel costruttore.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

