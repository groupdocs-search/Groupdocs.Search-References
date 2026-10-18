---
title: "FileOutputAdapter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un adaptador de salida que recopila la salida en un archivo."
type: docs
weight: 21
url: /es/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Representa un adaptador de salida que recopila la salida en un archivo.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Creando un adaptador de salida de archivo
index.getDocumentText(documents[0], adapter); // Generando el texto del documento en el archivo de salida
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Inicializa una nueva instancia de la  FileOutputAdapter  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Obtiene una ruta de archivo de salida. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Inicializa una nueva instancia de la  FileOutputAdapter  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | El formato de salida. |
|
|  | filePath | java.lang.String | La ruta del archivo de salida. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Obtiene una ruta de archivo de salida.


**Returns:**
java.lang.String - La ruta del archivo de salida.

