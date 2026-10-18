---
title: "DateFormat"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili format tanggal."
type: docs
weight: 13
url: /id/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Mewakili format tanggal.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Menghapus format tanggal default
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Membuat pola format tanggal 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Cari di indeks
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Menginisialisasi sebuah instance baru dari kelas  DateFormat  . |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas  DateFormat  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Mendapatkan pemisah tanggal. |
|
|  | [toString()](#toString--) | Mengembalikan sebuah String yang mewakili  DateFormat  saat ini. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Menginisialisasi sebuah instance baru dari kelas  DateFormat  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | cultureName | java.lang.String | Nama budaya. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Elemen format. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Menginisialisasi sebuah instance baru dari kelas  DateFormat  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Elemen format. |
|
|  | dateSeparator | java.lang.String | Pemisah tanggal. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Mendapatkan pemisah tanggal.


**Returns:**
java.lang.String - Pemisah tanggal.

### toString() {#toString--}
```
public String toString()
```


Mengembalikan sebuah String yang mewakili  DateFormat  saat ini.


**Returns:**
java.lang.String - Sebuah String yang mewakili  DateFormat  saat ini.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
