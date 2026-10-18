---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output come System.String."
type: docs
weight: 32
url: /it/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Rappresenta un adattatore di output che raccoglie l'output come un  System.String .


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Creazione di un adattatore di output stringa
index.getDocumentText(documents[0], adapter); // Generazione del testo del documento nell'adattatore
String result = adapter.getResult(); // Ottenimento di un risultato
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Inizializza una nuova istanza della classe StringOutputAdapter. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getResult()](#getResult--) | Restituisce la stringa risultante. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Inizializza una nuova istanza della classe StringOutputAdapter.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Il formato di output. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Restituisce la stringa risultante.


**Returns:**
java.lang.String - La stringa risultante.

