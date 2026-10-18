---
title: "IndexSettings"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la configuración del índice que permite personalizar las operaciones de indexación."
type: docs
weight: 19
url: /es/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Representa la configuración del índice que permite personalizar las operaciones de indexación.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Configurando el tipo de índice
Index index = new Index(indexFolder, settings); // Creando un índice
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Inicializa una nueva instancia de la clase  IndexSettings  . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Obtiene un valor que indica si el índice se almacena en memoria o en disco. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Obtiene un valor que indica si se deben usar palabras vacías o no. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Establece un valor que indica si se deben usar palabras vacías o no. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Obtiene el número máximo de informes de indexación. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Establece el número máximo de informes de indexación. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Obtiene el número máximo de informes de búsqueda. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Establece el número máximo de informes de búsqueda. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Obtiene un valor que indica si se deben usar reemplazos de caracteres o no. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Establece un valor que indica si se deben usar reemplazos de caracteres o no. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Obtiene un filtro de documento. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Establece un filtro de documento. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Obtiene la configuración de almacenamiento de texto. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Establece la configuración de almacenamiento de texto. |
|
|  | [getIndexType()](#getIndexType--) | Obtiene el tipo de índice. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Establece el tipo de índice. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Obtiene el número de hilos usados para la búsqueda. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Establece el número de hilos usados para la búsqueda. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Obtiene la colección de extractores personalizados. |
|
|  | [getLogger()](#getLogger--) | Obtiene un registrador que se usa para registrar eventos y errores en el índice. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Establece un registrador que se usa para registrar eventos y errores en el índice. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Inicializa una nueva instancia de la clase  IndexSettings  .


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Obtiene un valor que indica si el índice se almacena en memoria o en disco.


**Returns:**
boolean - Un valor que indica si el índice se almacena en memoria o en disco.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Obtiene un valor que indica si se usan palabras vacías o no. El valor predeterminado es  true .


**Returns:**
boolean - Un valor que indica si se usan palabras vacías o no.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Establece un valor que indica si se usan palabras vacías o no. El valor predeterminado es  true .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se usan palabras vacías o no. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Obtiene el número máximo de informes de indexación. El valor predeterminado es  5 .


**Returns:**
int - El número máximo de informes de indexación.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Establece el número máximo de informes de indexación. El valor predeterminado es  5 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de informes de indexación. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Obtiene el número máximo de informes de búsqueda. El valor predeterminado es  10 .


**Returns:**
int - El número máximo de informes de búsqueda.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Establece el número máximo de informes de búsqueda. El valor predeterminado es  10 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de informes de búsqueda. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Obtiene un valor que indica si se usan reemplazos de caracteres o no. El valor predeterminado es  false .


**Returns:**
boolean - Un valor que indica si se usan reemplazos de caracteres o no.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Establece un valor que indica si se usan reemplazos de caracteres o no. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se usan reemplazos de caracteres o no. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Obtiene un filtro de documentos. El  DocumentFilter  funciona con la lógica de inclusión. Use la clase  DocumentFilter  para crear una instancia de filtro de documentos. El valor predeterminado es  null , lo que significa que todos los documentos añadidos se indexan.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

El ejemplo muestra cómo establecer el filtro de documentos.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un filtro que omite documentos con extensiones '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creando filtro de extensión de archivo
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Invirtiendo filtro de extensión de archivo
settings.setDocumentFilter(invertedFilter);
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder, settings);
// Indexando documentos
index.add(documentsFolder);
// Buscando
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Establece un filtro de documento. El DocumentFilter funciona con la lógica de inclusión. Use la clase GroupDocs.Search.Options.DocumentFilter para crear instancias de filtros de documento. El valor predeterminado es null, lo que significa que todos los documentos añadidos se indexan.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | El filtro de documento. |

El ejemplo muestra cómo establecer el filtro de documentos.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un filtro que omite documentos con extensiones '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creando filtro de extensión de archivo
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Invirtiendo filtro de extensión de archivo
settings.setDocumentFilter(invertedFilter);
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder, settings);
// Indexando documentos
index.add(documentsFolder);
// Buscando
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Obtiene la configuración de almacenamiento de texto. El valor predeterminado es null, lo que significa que los textos de los documentos no se almacenan.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

El ejemplo muestra cómo establecer la configuración de almacenamiento de texto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando instancia de configuración de índice
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Estableciendo nivel de compresión alto para el almacenamiento de texto del índice
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder, settings);
// Indexando documentos
index.add(documentsFolder);
// Buscando
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Establece la configuración de almacenamiento de texto. El valor predeterminado es null, lo que significa que los textos de los documentos no se almacenan.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | La configuración de almacenamiento de texto. |

El ejemplo muestra cómo establecer la configuración de almacenamiento de texto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando instancia de configuración de índice
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Estableciendo nivel de compresión alto para el almacenamiento de texto del índice
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder, settings);
// Indexando documentos
index.add(documentsFolder);
// Buscando
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Obtiene el tipo de índice. El valor predeterminado es GroupDocs.Search.Options.IndexType.NormalIndex.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Establece el tipo de índice. El valor predeterminado es GroupDocs.Search.Options.IndexType.NormalIndex.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | El tipo de índice. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Obtiene el número de hilos utilizados para la búsqueda. El valor predeterminado es GroupDocs.Search.Options.NumberOfThreads.Default, lo que significa que la búsqueda se realizará utilizando un número de hilos igual al número de núcleos del procesador.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Establece el número de hilos utilizados para la búsqueda. El valor predeterminado es GroupDocs.Search.Options.NumberOfThreads.Default, lo que significa que la búsqueda se realizará utilizando un número de hilos igual al número de núcleos del procesador.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | El número de hilos utilizados para la búsqueda. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Obtiene la colección de extractores personalizados. El ejemplo completo de implementación de un extractor personalizado se presenta en la documentación de la interfaz GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Obtiene un registrador que se utiliza para registrar eventos y errores en el índice. Tenga en cuenta que el registrador no se guarda y debe crearse y asignarse cada vez que se crea o carga el índice.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Establece un registrador que se utiliza para registrar eventos y errores en el índice. Tenga en cuenta que el registrador no se guarda y debe crearse y asignarse cada vez que se crea o carga el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Un registrador que se utiliza para registrar eventos y errores en el índice. |
|

