---
title: "IndexingReport"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет подробную информацию об операции индексирования."
type: docs
weight: 25
url: /ru/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Представляет подробную информацию об операции индексирования.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов
index.add(documentsFolder1);
index.add(documentsFolder2);
// Получение отчетов индексации
IndexingReport[] reports = index.getIndexingReports();
// Вывод отчетов в консоль
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Время: " + df.format(report.getStartTime()));
System.out.println("Продолжительность: " + report.getIndexingTime());
System.out.println("Всего документов: " + report.getTotalDocumentsInIndex());
System.out.println("Всего терминов: " + report.getTotalTermCount());
System.out.println("Размер проиндексированных документов (МБ): " + report.getIndexedDocumentsSize());
System.out.println("Размер индекса (МБ): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Получает общее количество документов в индексе. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Получает общее количество терминов в индексе. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Получает общую длину проиндексированных документов в МБ. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Получает количество сегментов индекса. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Получает общий размер индекса в байтах. |
|
|  | [getStartTime()](#getStartTime--) | Получает время начала индексации. |
|
|  | [getEndTime()](#getEndTime--) | Получает время окончания индексации. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Получает продолжительность индексации в секундах. |
|
|  | [getErrors()](#getErrors--) | Получает список ошибок. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Получает список проиндексированных документов. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Получает список обновлённых документов. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Получает список удалённых из индекса документов. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Получает общее количество документов в индексе.


**Returns:**
int - Общее количество документов в индексе.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Получает общее количество терминов в индексе.


**Returns:**
int - Общее количество терминов в индексе.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Получает общую длину проиндексированных документов в МБ.


**Returns:**
double - Общая длина проиндексированных документов в МБ.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Получает количество сегментов индекса.


**Returns:**
int - Количество сегментов индекса.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Получает общий размер индекса в байтах.


**Returns:**
long - Общий размер индекса в байтах.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Получает время начала индексации.


**Returns:**
java.util.Date - Время начала индексации.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Получает время окончания индексации.


**Returns:**
java.util.Date - Время завершения индексации.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Получает продолжительность индексации в секундах.


**Returns:**
double - Длительность индексации в секундах.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Получает список ошибок.


**Returns:**
java.lang.String[] - Список ошибок.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Получает список проиндексированных документов.


**Returns:**
java.lang.String[] - Список проиндексированных документов.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Получает список обновлённых документов.


**Returns:**
java.lang.String[] - Список обновлённых документов.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Получает список удалённых из индекса документов.


**Returns:**
java.lang.String[] - Список удалённых из индекса документов.

