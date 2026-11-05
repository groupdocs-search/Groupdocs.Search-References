---
title: "FileLogger"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет регистратор, который записывает события и ошибки в локальный файл."
type: docs
weight: 20
url: /ru/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Представляет регистратор, который записывает события и ошибки в локальный файл.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Указание пути к файлу журнала и максимальной длины 4 МБ
Index index = new Index(indexFolder, settings); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchResult result = index.search(query); // Поиск в индексе
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Инициализирует новый экземпляр класса FileLogger. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Записывает ошибку, произошедшую в индексе. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Записывает событие, произошедшее в индексе. |
|
|  | [getFilePath()](#getFilePath--) | Получает путь к файлу журнала. |
|
|  | [getMaxSize()](#getMaxSize--) | Получает максимальный размер файла журнала в мегабайтах. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Инициализирует новый экземпляр класса FileLogger.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу журнала. |
|
|  | maxSize | double | Максимальный размер файла журнала в мегабайтах. Значение должно находиться в диапазоне от 0.1 до 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Записывает ошибку, произошедшую в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | сообщение | java.lang.String | Сообщение об ошибке. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Записывает событие, произошедшее в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | сообщение | java.lang.String | Сообщение о событии. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Получает путь к файлу журнала.


**Returns:**
java.lang.String - Путь к файлу журнала.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Получает максимальный размер файла журнала в мегабайтах.


**Returns:**
double - Максимальный размер файла журнала в мегабайтах.

