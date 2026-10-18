---
title: "Datumformat"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett datumformat."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Representerar ett datumformat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Tar bort standarddatumformat
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Skapar ett datumformatmönster 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Sök i index
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Initierar en ny instans av klassen  DateFormat  . |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Initierar en ny instans av klassen  DateFormat  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Hämtar datumseparatorn. |
|
|  | [toString()](#toString--) | Returnerar en sträng som representerar den aktuella  DateFormat  . |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Initierar en ny instans av klassen  DateFormat  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | cultureName | java.lang.String | Kulturnamnet. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Formatets element. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Initierar en ny instans av klassen  DateFormat  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Formatets element. |
|
|  | dateSeparator | java.lang.String | Datumseparatorn. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Hämtar datumseparatorn.


**Returns:**
java.lang.String - Datumseparatorn.

### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar den aktuella  DateFormat  .


**Returns:**
java.lang.String - En sträng som representerar den aktuella  DateFormat  .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
