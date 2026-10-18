---
title: "DateFormat"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un formato de fecha."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Representa un formato de fecha.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Eliminando los formatos de fecha predeterminados
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Creando un patrón de formato de fecha 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Buscar en el índice
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Inicializa una nueva instancia de la  DateFormat  clase. |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Inicializa una nueva instancia de la  DateFormat  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Obtiene el separador de fecha. |
|
|  | [toString()](#toString--) | Devuelve un String que representa el  DateFormat  actual. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Inicializa una nueva instancia de la  DateFormat  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | cultureName | java.lang.String | El nombre de la cultura. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Los elementos de formato. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Inicializa una nueva instancia de la  DateFormat  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Los elementos de formato. |
|
|  | dateSeparator | java.lang.String | El separador de fecha. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Obtiene el separador de fecha.


**Returns:**
java.lang.String - El separador de fecha.

### toString() {#toString--}
```
public String toString()
```


Devuelve un String que representa el  DateFormat  actual.


**Returns:**
java.lang.String - Un String que representa el  DateFormat  actual.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
