---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет базовый класс для алгоритмов нечеткого поиска."
type: docs
weight: 20
url: /ru/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Представляет базовый класс для алгоритмов нечеткого поиска.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Получает уровень сходства для указанной длины термина. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Получает максимальное допустимое количество ошибок для указанной длины термина. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Получает уровень сходства для указанной длины термина.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | termLength | int | Длина термина. |
|

**Returns:**
double - Уровень сходства.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Получает максимальное допустимое количество ошибок для указанной длины термина.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | termLength | int | Длина термина. |
|

**Returns:**
int - Максимально допустимое количество ошибок.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
