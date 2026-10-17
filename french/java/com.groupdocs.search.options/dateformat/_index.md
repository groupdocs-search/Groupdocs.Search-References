---
title: "DateFormat"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un format de date."
type: docs
weight: 13
url: /fr/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Représente un format de date.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Suppression des formats de date par défaut
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Création d'un modèle de format de date 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Rechercher dans l'index
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Initialise une nouvelle instance de la classe  DateFormat . |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Initialise une nouvelle instance de la classe  DateFormat . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Obtient le séparateur de date. |
|
|  | [toString()](#toString--) | Renvoie une chaîne qui représente le  DateFormat  actuel. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Initialise une nouvelle instance de la classe  DateFormat .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | cultureName | java.lang.String | Le nom de la culture. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Les éléments de format. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Initialise une nouvelle instance de la classe  DateFormat .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Les éléments de format. |
|
|  | dateSeparator | java.lang.String | Le séparateur de date. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Obtient le séparateur de date.


**Returns:**
java.lang.String - Le séparateur de date.

### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente le  DateFormat  actuel.


**Returns:**
java.lang.String - Une chaîne qui représente le  DateFormat  actuel.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
