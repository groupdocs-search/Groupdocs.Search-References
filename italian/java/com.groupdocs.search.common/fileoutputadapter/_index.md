---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output in un file."
type: docs
weight: 21
url: /it/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Rappresenta un adattatore di output che raccoglie l'output in un file.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Creazione di un adattatore di output file
index.getDocumentText(documents[0], adapter); // Generazione del testo del documento nel file di output
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Inizializza una nuova istanza della classe FileOutputAdapter. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Ottiene un percorso di file di output. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Inizializza una nuova istanza della classe FileOutputAdapter.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Il formato di output. |
|
|  | filePath | java.lang.String | Il percorso del file di output. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Ottiene un percorso di file di output.


**Returns:**
java.lang.String - Il percorso del file di output.

