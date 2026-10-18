---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат поиска изображений, соответствующий поисковому изображению."
type: docs
weight: 12
url: /ru/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Представляет результат поиска изображений, соответствующий поисковому изображению.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Возвращает количество найденных изображений. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Возвращает найденное изображение по индексу. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Получает токен поиска фрагмента изображения для поиска следующего фрагмента. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Получает индекс узла, из которого был получен результат. |
|
|  | [getShardIndex()](#getShardIndex--) | Получает индекс шарда, из которого был получен результат. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Возвращает количество найденных изображений.


**Returns:**
int - Количество найденных изображений.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Возвращает найденное изображение по индексу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс найденного изображения. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Получает токен поиска фрагмента изображения для поиска следующего фрагмента.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Получает индекс узла, из которого был получен результат.


**Returns:**
int - Индекс узла, из которого был получен результат.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Получает индекс шарда, из которого был получен результат.


**Returns:**
int - Индекс шарда, из которого был получен результат.

