---
title: "DateFormat"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Datumsformat dar."
type: docs
weight: 13
url: /de/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Stellt ein Datumsformat dar.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Erstellen eines Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Entfernt Standard-Datumsformate
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Erstellen eines Datumsformatmusters 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Suche im Index
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Initialisiert eine neue Instanz der  DateFormat  Klasse. |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Initialisiert eine neue Instanz der  DateFormat  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Liest das Datums‑Trennzeichen. |
|
|  | [toString()](#toString--) | Gibt einen String zurück, der das aktuelle  DateFormat  darstellt. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Initialisiert eine neue Instanz der  DateFormat  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | cultureName | java.lang.String | Der Kulturname. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Die Format‑Elemente. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Initialisiert eine neue Instanz der  DateFormat  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Die Format‑Elemente. |
|
|  | dateSeparator | java.lang.String | Das Datums‑Trennzeichen. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Liest das Datums‑Trennzeichen.


**Returns:**
java.lang.String - Das Datums‑Trennzeichen.

### toString() {#toString--}
```
public String toString()
```


Gibt einen String zurück, der das aktuelle  DateFormat  darstellt.


**Returns:**
java.lang.String - Ein String, der das aktuelle  DateFormat  darstellt.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
