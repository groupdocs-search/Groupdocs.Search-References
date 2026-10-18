---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет адаптер вывода, который собирает вывод как System.String."
type: docs
weight: 32
url: /ru/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Представляет выходной адаптер, который собирает вывод как System.String.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Создание адаптера вывода строки
index.getDocumentText(documents[0], adapter); // Генерация текста документа в адаптер
String result = adapter.getResult(); // Получение результата
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Инициализирует новый экземпляр класса  StringOutputAdapter  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getResult()](#getResult--) | Получает результирующую строку. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Инициализирует новый экземпляр класса  StringOutputAdapter  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Формат вывода. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Получает результирующую строку.


**Returns:**
java.lang.String - Результирующая строка.

