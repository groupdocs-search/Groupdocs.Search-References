---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output in un java.io.OutputStream."
type: docs
weight: 31
url: /it/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Rappresenta un adattatore di output che raccoglie l'output in un  java.io.OutputStream .


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
DocumentInfo[] documents = index.getIndexedDocuments(); // Ottenere informazioni sui documenti indicizzati
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Creazione di un flusso di output
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Creazione di un adattatore di output stream
index.getDocumentText(documents[0], adapter); // Generazione del testo del documento nel flusso
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Inizializza una nuova istanza della classe  StreamOutputAdapter  . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getStream()](#getStream--) | Ottiene un flusso di output. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Inizializza una nuova istanza della classe  StreamOutputAdapter  .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Il formato di output. |
|
|  | stream | java.io.OutputStream | Il flusso di output. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Ottiene un flusso di output.


**Returns:**
java.io.OutputStream - Il flusso di output.

