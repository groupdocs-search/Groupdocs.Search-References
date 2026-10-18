---
title: "DateFormat"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een datumformaat voor."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Stelt een datumformaat voor.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Een index maken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Verwijdert standaard datumformaten
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Een datumformaatpatroon maken 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Zoeken in index
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Initialiseert een nieuw exemplaar van de  DateFormat  klasse. |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Initialiseert een nieuw exemplaar van de  DateFormat  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Haalt de datumseparator op. |
|
|  | [toString()](#toString--) | Retourneert een String die de huidige  DateFormat  weergeeft. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Initialiseert een nieuw exemplaar van de  DateFormat  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | cultureName | java.lang.String | De cultuurnaam. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | De formattelementen. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Initialiseert een nieuw exemplaar van de  DateFormat  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | De formattelementen. |
|
|  | dateSeparator | java.lang.String | De datumseparator. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Haalt de datumseparator op.


**Returns:**
java.lang.String - De datumseparator.

### toString() {#toString--}
```
public String toString()
```


Retourneert een String die de huidige  DateFormat  weergeeft.


**Returns:**
java.lang.String - Een String die de huidige  DateFormat  weergeeft.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
