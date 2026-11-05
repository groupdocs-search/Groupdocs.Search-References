---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет адаптер вывода, который собирает вывод в java.io.OutputStream."
type: docs
weight: 31
url: /ru/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Представляет выходной адаптер, который собирает вывод в java.io.OutputStream.


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Создание выходного потока
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Создание адаптера вывода в поток
index.getDocumentText(documents[0], adapter); // Генерация текста документа в поток
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Инициализирует новый экземпляр класса  StreamOutputAdapter . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getStream()](#getStream--) | Получает выходной поток. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Инициализирует новый экземпляр класса  StreamOutputAdapter .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Формат вывода. |
|
|  | stream | java.io.OutputStream | Выходной поток. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Получает выходной поток.


**Returns:**
java.io.OutputStream - Выходной поток.

