---
title: "DateFormat"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет формат даты."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Представляет формат даты.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = \"daterange(2017-01-01 ~~ 2019-12-31)\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Удаление форматов даты по умолчанию
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// Создание шаблона формата даты 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Поиск в индексе
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Инициализирует новый экземпляр класса  DateFormat . |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Инициализирует новый экземпляр класса  DateFormat . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | Получает разделитель даты. |
|
|  | [toString()](#toString--) | Возвращает строку, представляющую текущий  DateFormat . |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Инициализирует новый экземпляр класса  DateFormat .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | cultureName | java.lang.String | Имя культуры. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Элементы формата. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Инициализирует новый экземпляр класса  DateFormat .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | Элементы формата. |
|
|  | dateSeparator | java.lang.String | Разделитель даты. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


Получает разделитель даты.


**Returns:**
java.lang.String - Разделитель даты.

### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий  DateFormat .


**Returns:**
java.lang.String - Строка, представляющая текущий  DateFormat .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
