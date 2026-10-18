---
title: "FileLogger"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un registrador que registra eventos y errores en un archivo local."
type: docs
weight: 20
url: /es/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Representa un registrador que registra eventos y errores en un archivo local.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Especificando la ruta al archivo de registro y una longitud máxima de 4 MB
Index index = new Index(indexFolder, settings); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchResult result = index.search(query); // Buscar en el índice
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Inicializa una nueva instancia de la clase FileLogger. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Registra un error que ocurrió en el índice. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Registra un evento que ocurrió en el índice. |
|
|  | [getFilePath()](#getFilePath--) | Obtiene la ruta del archivo de registro. |
|
|  | [getMaxSize()](#getMaxSize--) | Obtiene el tamaño máximo del archivo de registro en megabytes. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Inicializa una nueva instancia de la clase FileLogger.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo de registro. |
|
|  | maxSize | double | El tamaño máximo del archivo de registro en megabytes. El valor debe estar en el rango de 0.1 a 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Registra un error que ocurrió en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | message | java.lang.String | El mensaje de error. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Registra un evento que ocurrió en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | message | java.lang.String | El mensaje del evento. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Obtiene la ruta del archivo de registro.


**Returns:**
java.lang.String - La ruta del archivo de registro.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Obtiene el tamaño máximo del archivo de registro en megabytes.


**Returns:**
double - El tamaño máximo del archivo de registro en megabytes.

