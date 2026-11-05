---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет подсветку результатов поиска, которая выделяет результаты поиска в фрагментах текста."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Представляет подсветку результатов поиска, которая выделяет результаты поиска в фрагментах текста.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Поиск слова 'Einstein'
SearchResult result = index.search("Einstein");
// Назначение параметров выделения
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Выделение найденных слов в тексте документа
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Получение результата
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Печать HTML‑разметки в консоль
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Инициализирует новый экземпляр класса  FragmentHighlighter  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getResult()](#getResult--) | Получает массив результирующих контейнеров фрагментов. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Инициализирует новый экземпляр класса  FragmentHighlighter  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Формат вывода. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Получает массив результирующих контейнеров фрагментов.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Массив результирующих контейнеров фрагментов.

