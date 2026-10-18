---
title: "DocumentHighlighter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un resaltador de resultados de búsqueda que resalta los resultados de búsqueda en el texto completo de un documento."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Representa un resaltador de resultados de búsqueda que resalta los resultados de búsqueda en el texto completo de un documento.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Buscar la frase 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Resaltando palabras encontradas en el texto de un documento
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Inicializa una nueva instancia de la clase  DocumentHighlighter  . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Obtiene el adaptador de salida pasado en el constructor. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Inicializa una nueva instancia de la clase  DocumentHighlighter  .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | El adaptador de salida que transfiere un resultado del resaltado. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Obtiene el adaptador de salida pasado en el constructor.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

