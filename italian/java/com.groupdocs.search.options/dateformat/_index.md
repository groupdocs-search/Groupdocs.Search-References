---
title: "DateFormat"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un formato data."
type: docs
weight: 13
url: /it/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Rappresenta un formato data.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Rimozione dei formati data predefiniti
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Creazione di un modello di formato data 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Cerca nell'indice
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Inizializza una nuova istanza della classe  DateFormat . |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Inizializza una nuova istanza della classe  DateFormat . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Ottiene il separatore di data. |
|
|  | [toString()](#toString--) | Restituisce una Stringa che rappresenta il corrente  DateFormat . |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Inizializza una nuova istanza della classe  DateFormat .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | cultureName | java.lang.String | Il nome della cultura. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Gli elementi di formato. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Inizializza una nuova istanza della classe  DateFormat .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Gli elementi di formato. |
|
|  | dateSeparator | java.lang.String | Il separatore di data. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Ottiene il separatore di data.


**Returns:**
java.lang.String - Il separatore di data.

### toString() {#toString--}
```
public String toString()
```


Restituisce una Stringa che rappresenta il corrente  DateFormat .


**Returns:**
java.lang.String - Una Stringa che rappresenta il corrente  DateFormat .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
