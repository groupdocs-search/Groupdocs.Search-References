---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат поиска, соответствующий поисковому запросу."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Представляет результат поиска, соответствующий поисковому запросу.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
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
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Получает токен поиска фрагмента для поиска следующего фрагмента. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Получает индекс узла, из которого был получен результат. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
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
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Возвращает найденный документ по индексу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс найденного документа. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Возвращает итератор, который перебирает коллекцию найденных документов.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Итератор, который можно использовать для перебора коллекции найденных документов.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Получает токен поиска фрагмента для поиска следующего фрагмента.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Получает индекс узла, из которого был получен результат.


**Returns:**
int - Индекс узла, из которого был получен результат.

