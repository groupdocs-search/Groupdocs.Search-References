---
title: "DateFormat"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir tarih biçimini temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Bir tarih biçimini temsil eder.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Varsayılan tarih formatlarını kaldırma
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// 'MM/dd/yyyy' tarih formatı deseni oluşturma
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // İndekste arama
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | DateFormat sınıfının yeni bir örneğini başlatır. |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | DateFormat sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Tarih ayırıcıyı alır. |
|
|  | [toString()](#toString--) | Geçerli DateFormat'ı temsil eden bir String döndürür. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


DateFormat sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | cultureName | java.lang.String | Kültür adı. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Biçim öğeleri. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


DateFormat sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Biçim öğeleri. |
|
|  | dateSeparator | java.lang.String | Tarih ayırıcı. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Tarih ayırıcıyı alır.


**Returns:**
java.lang.String - Tarih ayırıcı.

### toString() {#toString--}
```
public String toString()
```


Geçerli DateFormat'ı temsil eden bir String döndürür.


**Returns:**
java.lang.String - Geçerli DateFormat'ı temsil eden bir String.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
