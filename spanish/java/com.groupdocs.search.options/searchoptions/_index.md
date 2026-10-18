---
title: "SearchOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para la operación de búsqueda."
type: docs
weight: 34
url: /es/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Proporciona opciones para la operación de búsqueda.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Inicializa una nueva instancia de la  SearchOptions  clase. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Inicializa una nueva instancia de la  SearchOptions  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Obtiene la bandera de uso de sinónimos en la búsqueda. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Establece la bandera de uso de sinónimos en la búsqueda. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Obtiene la bandera de uso de homófonos en la búsqueda. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Establece la bandera de uso de homófonos en la búsqueda. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Obtiene la bandera de uso de diferentes formas de palabra en la búsqueda. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Establece la bandera de uso de diferentes formas de palabra en la búsqueda. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Obtiene la bandera de recuperación de atributos asociados con los documentos encontrados. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Establece la bandera de recuperación de atributos asociados con los documentos encontrados. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Obtiene las opciones de búsqueda difusa. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Obtiene las opciones del corrector ortográfico. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Obtiene las opciones del corrector de distribución del teclado. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Obtiene la bandera de búsqueda sensible a mayúsculas. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Establece la bandera de búsqueda sensible a mayúsculas. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Obtiene el número total máximo de ocurrencias de todos los términos en una consulta de búsqueda. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Establece el número total máximo de ocurrencias de todos los términos en una consulta de búsqueda. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Obtiene el número máximo de ocurrencias de cada término en una consulta de búsqueda. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Establece el número máximo de ocurrencias de cada término en una consulta de búsqueda. |
|
|  | [getDateFormats()](#getDateFormats--) | Obtiene la colección de formatos de fecha para la búsqueda por rango de fechas. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Obtiene la bandera de búsqueda por fragmentos. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Establece la bandera de búsqueda por fragmentos. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Obtiene el filtro de documento de búsqueda. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Establece el filtro de documentos de búsqueda. |
|
|  | [getCancellation()](#getCancellation--) | Obtiene el objeto de cancelación de la operación. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Establece el objeto de cancelación de la operación. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Inicializa una nueva instancia de la  SearchOptions  clase.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Inicializa una nueva instancia de la  SearchOptions  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Obtiene la bandera de uso de sinónimos en la búsqueda. El valor predeterminado es false.


**Returns:**
boolean - La bandera de uso de sinónimos en la búsqueda.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Establece la bandera de uso de sinónimos en la búsqueda. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de uso de sinónimos en la búsqueda. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Obtiene la bandera de uso de homófonos en la búsqueda. El valor predeterminado es false.


**Returns:**
boolean - La bandera de uso de homófonos en la búsqueda.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Establece la bandera de uso de homófonos en la búsqueda. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de uso de homófonos en la búsqueda. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Obtiene la bandera de uso de diferentes formas de palabra en la búsqueda. El valor predeterminado es false.


**Returns:**
boolean - La bandera de uso de diferentes formas de palabra en la búsqueda.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Establece la bandera de uso de diferentes formas de palabra en la búsqueda. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de usar diferentes formas de palabra en la búsqueda. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Obtiene la bandera de recuperar atributos asociados con los documentos encontrados. El valor predeterminado es false.


**Returns:**
boolean - La bandera de recuperar atributos asociados con los documentos encontrados.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Establece la bandera de recuperar atributos asociados con los documentos encontrados. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de recuperar atributos asociados con los documentos encontrados. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Obtiene las opciones de búsqueda difusa.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Obtiene las opciones del corrector ortográfico.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Obtiene las opciones del corrector de distribución del teclado.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Obtiene la bandera de búsqueda sensible a mayúsculas y minúsculas. El valor predeterminado es false.


**Returns:**
boolean - La bandera de búsqueda sensible a mayúsculas y minúsculas.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Establece la bandera de búsqueda sensible a mayúsculas y minúsculas. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de búsqueda sensible a mayúsculas y minúsculas. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Obtiene el número total máximo de ocurrencias de todos los términos en una consulta de búsqueda. El valor predeterminado es 500000.


**Returns:**
int - El número total máximo de ocurrencias.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Establece el número total máximo de ocurrencias de todos los términos en una consulta de búsqueda. El valor predeterminado es 500000.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número total máximo de ocurrencias. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Obtiene el número máximo de ocurrencias de cada término en una consulta de búsqueda. El valor predeterminado es 100000.


**Returns:**
int - El número máximo de ocurrencias de cada término en una consulta de búsqueda.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Establece el número máximo de ocurrencias de cada término en una consulta de búsqueda. El valor predeterminado es 100000.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de ocurrencias de cada término en una consulta de búsqueda. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Obtiene la colección de formatos de fecha para la búsqueda por rango de fechas. Los formatos de fecha predeterminados son 'dd.MM.yyyy', 'MM/dd/yyyy' y 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


El ejemplo muestra cómo establecer los formatos de fecha para la búsqueda.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Eliminando los formatos de fecha predeterminados
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Creando un patrón de formato de fecha 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Buscar en el índice
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Obtiene la bandera de búsqueda por fragmentos. El valor predeterminado es false.


**Returns:**
boolean - La bandera de búsqueda por fragmentos.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Establece la bandera de búsqueda por fragmentos. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de búsqueda por fragmentos. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Obtiene el filtro de documento de búsqueda.  SearchDocumentFilter  funciona con la lógica de inclusión. Use la clase  SearchDocumentFilter  para crear instancias de filtros de documento de búsqueda. El valor predeterminado es null, lo que significa que se devolverán todos los documentos encontrados.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


El ejemplo muestra cómo establecer el filtro de documentos.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos
index.add(documentsFolder);
// Creando un filtro de documentos de búsqueda que omite documentos con extensiones '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creando filtro de extensión de archivo
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Invirtiendo filtro de extensión de archivo
options.setSearchDocumentFilter(invertedFilter);
// Buscar en el índice
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Establece el filtro de documentos de búsqueda.  SearchDocumentFilter  funciona con la lógica de inclusión. Use la clase  SearchDocumentFilter  para crear instancias de filtros de documentos de búsqueda. El valor predeterminado es  null , lo que significa que se devolverán todos los documentos encontrados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | El filtro de documento de búsqueda. |


El ejemplo muestra cómo establecer el filtro de documentos.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos
index.add(documentsFolder);
// Creando un filtro de documentos de búsqueda que omite documentos con extensiones '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creando filtro de extensión de archivo
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Invirtiendo filtro de extensión de archivo
options.setSearchDocumentFilter(invertedFilter);
// Buscar en el índice
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Obtiene el objeto de cancelación de la operación. El valor predeterminado es  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Establece el objeto de cancelación de la operación. El valor predeterminado es  null .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | El objeto de cancelación de la operación. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
