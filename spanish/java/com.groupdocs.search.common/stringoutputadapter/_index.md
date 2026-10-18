---
title: "StringOutputAdapter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un adaptador de salida que recopila la salida como un System.String."
type: docs
weight: 32
url: /es/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Representa un adaptador de salida que recopila la salida como una `System.String`.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Creando un adaptador de salida de cadena
index.getDocumentText(documents[0], adapter); // Generando el texto del documento en el adaptador
String result = adapter.getResult(); // Obteniendo un resultado
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Inicializa una nueva instancia de la  StringOutputAdapter  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getResult()](#getResult--) | Obtiene la cadena resultante. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Inicializa una nueva instancia de la  StringOutputAdapter  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | El formato de salida. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Obtiene la cadena resultante.


**Returns:**
java.lang.String - La cadena resultante.

