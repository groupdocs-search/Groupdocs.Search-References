---
title: "SearchReport"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет подробную информацию о поисковой операции."
type: docs
weight: 30
url: /ru/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Представляет подробную информацию о поисковой операции.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Поиск в индексе
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Получение отчетов поиска
SearchReport[] reports = index.getSearchReports();
// Вывод отчетов в консоль
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Время: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Получает время начала поиска. |
|
|  | [getEndTime()](#getEndTime--) | Получает время окончания поиска. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Получает продолжительность поиска в секундах. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Получает количество найденных документов. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Получает общее количество найденных вхождений. |
|
|  | [getTextQuery()](#getTextQuery--) | Получает поисковый запрос в текстовой форме. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Получает поисковый запрос в виде объекта. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Получает параметры поиска. |
|
|  | [toString()](#toString--) | Возвращает строку, представляющую текущий SearchReport. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Получает время начала поиска.


**Returns:**
java.util.Date - Время начала поиска.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Получает время окончания поиска.


**Returns:**
java.util.Date - Время окончания поиска.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Получает продолжительность поиска в секундах.


**Returns:**
double - Продолжительность поиска в секундах.

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Получает количество найденных документов.


**Returns:**
int - Количество найденных документов.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Получает общее количество найденных вхождений.


**Returns:**
int - Общее количество найденных вхождений.

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Получает поисковый запрос в текстовой форме.


**Returns:**
java.lang.String - Поисковый запрос в текстовой форме.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Получает поисковый запрос в виде объекта.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Получает параметры поиска.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Возвращает строку, представляющую текущий SearchReport.


**Returns:**
java.lang.String - Строка, представляющая текущий SearchReport.

