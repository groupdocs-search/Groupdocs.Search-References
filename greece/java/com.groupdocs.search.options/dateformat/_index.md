---
title: "DateFormat"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά μια μορφή ημερομηνίας."
type: docs
weight: 13
url: /el/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Αναπαριστά μια μορφή ημερομηνίας.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Αφαίρεση προεπιλεγμένων μορφών ημερομηνίας
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Δημιουργία προτύπου μορφής ημερομηνίας 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Αναζήτηση στο ευρετήριο
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Αρχικοποιεί μια νέα παρουσία της κλάσης  DateFormat  . |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης  DateFormat  . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Λαμβάνει το διαχωριστικό ημερομηνίας. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον  DateFormat . |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  DateFormat  .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | cultureName | java.lang.String | Το όνομα πολιτισμού. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Τα στοιχεία μορφής. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  DateFormat  .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Τα στοιχεία μορφής. |
|
|  | dateSeparator | java.lang.String | Το διαχωριστικό ημερομηνίας. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Λαμβάνει το διαχωριστικό ημερομηνίας.


**Returns:**
java.lang.String - Το διαχωριστικό ημερομηνίας.

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον  DateFormat .


**Returns:**
java.lang.String - Ένα String που αντιπροσωπεύει το τρέχον  DateFormat .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
