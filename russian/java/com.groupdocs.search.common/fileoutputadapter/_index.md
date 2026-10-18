---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет адаптер вывода, который собирает вывод в файл."
type: docs
weight: 21
url: /ru/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Представляет адаптер вывода, который собирает вывод в файл.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
DocumentInfo[] documents = index.getIndexedDocuments(); // Получение информации об индексированных документах
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Создание адаптера вывода файла
index.getDocumentText(documents[0], adapter); // Генерация текста документа в выходной файл
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Инициализирует новый экземпляр класса  FileOutputAdapter . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Получает путь к выходному файлу. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Инициализирует новый экземпляр класса  FileOutputAdapter .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Формат вывода. |
|
|  | filePath | java.lang.String | Путь к выходному файлу. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Получает путь к выходному файлу.


**Returns:**
java.lang.String - Путь к выходному файлу.

