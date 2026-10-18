---
title: "StreamOutputAdapter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un adaptador de salida que recopila la salida en un java.io.OutputStream."
type: docs
weight: 31
url: /es/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Representa un adaptador de salida que recopila la salida en un `java.io.OutputStream`.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
DocumentInfo[] documents = index.getIndexedDocuments(); // Obteniendo información de los documentos indexados
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Creando un flujo de salida
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Creando un adaptador de salida de flujo
index.getDocumentText(documents[0], adapter); // Generando el texto del documento en el flujo
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Inicializa una nueva instancia de la clase  StreamOutputAdapter. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getStream()](#getStream--) | Obtiene un flujo de salida. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Inicializa una nueva instancia de la clase  StreamOutputAdapter.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | El formato de salida. |
|
|  | stream | java.io.OutputStream | El flujo de salida. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Obtiene un flujo de salida.


**Returns:**
java.io.OutputStream - El flujo de salida.

