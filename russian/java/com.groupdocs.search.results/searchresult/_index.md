---
title: "SearchResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат поиска, соответствующий поисковому запросу."
type: docs
weight: 19
url: /ru/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Представляет результат поиска, соответствующий поисковому запросу.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentFolder);
// Установка параметров поиска
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Включение нечёткого поиска
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Установка максимального количества различий до 3
// Поиск документов, содержащих слово 'Einstein' или фразу 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Вывод результата
System.out.println("Документы: " + result.getDocumentCount());
System.out.println("Общее количество вхождений: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tДокумент: " + document.getDocumentInfo().getFilePath());
System.out.println("\tВхождения: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tПоле: " + field.getFieldName());
System.out.println("\t\tOccurrences: " + document.getOccurrenceCount());
// Печать найденных терминов
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Печать найденных фраз
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Получает количество найденных документов. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Получает общее количество найденных вхождений. |
|
|  | [getTruncated()](#getTruncated--) | Возвращает значение, указывающее, что результат усечён. |
|
|  | [getWarnings()](#getWarnings--) | Возвращает предупреждения, описывающие результат. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Получает токен поиска фрагмента для поиска следующего фрагмента. |
|
|  | [getStartTime()](#getStartTime--) | Получает время начала поиска. |
|
|  | [getEndTime()](#getEndTime--) | Получает время окончания поиска. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Получает продолжительность поиска в секундах. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Возвращает найденный документ по индексу. |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который перебирает коллекцию найденных документов. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Возвращает значение, указывающее, что результат усечён.


**Returns:**
boolean - Значение, указывающее, что результат усечён.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Возвращает предупреждения, описывающие результат.


**Returns:**
java.lang.String - Предупреждения, описывающие результат.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Получает токен поиска фрагмента для поиска следующего фрагмента.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Возвращает найденный документ по индексу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс найденного документа. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Возвращает итератор, который перебирает коллекцию найденных документов.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Итератор, который может использоваться для перебора коллекции найденных документов.

