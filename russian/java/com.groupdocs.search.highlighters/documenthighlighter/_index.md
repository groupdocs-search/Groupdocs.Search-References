---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет подсветку результатов поиска, которая выделяет результаты поиска во всем тексте документа."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Представляет подсветку результатов поиска, которая выделяет результаты поиска во всем тексте документа.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Поиск фразы 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Выделение найденных слов в тексте документа
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Инициализирует новый экземпляр класса DocumentHighlighter. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Получает адаптер вывода, переданный в конструкторе. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Инициализирует новый экземпляр класса DocumentHighlighter.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Адаптер вывода, передающий результат выделения. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Получает адаптер вывода, переданный в конструкторе.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

