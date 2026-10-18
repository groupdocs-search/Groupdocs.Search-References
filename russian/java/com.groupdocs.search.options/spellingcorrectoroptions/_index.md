---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для корректора орфографии."
type: docs
weight: 36
url: /ru/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Предоставляет параметры для корректора орфографии.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Возвращает значение, указывающее, включён ли корректор орфографии. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Устанавливает значение, указывающее, включён ли корректор орфографии. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Возвращает максимальное количество ошибок. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Устанавливает максимальное количество ошибок. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Возвращает значение, указывающее, будут ли возвращаться только лучшие результаты. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Устанавливает значение, указывающее, будут ли возвращаться только лучшие результаты. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Возвращает максимальное превышение минимального количества найденных ошибок. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Устанавливает максимальное превышение минимального количества найденных ошибок. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Возвращает значение, указывающее, должен ли алгоритм рассматривать транспозицию двух соседних символов как одну ошибку. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Устанавливает значение, указывающее, должен ли алгоритм рассматривать транспозицию двух соседних символов как одну ошибку. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Возвращает значение, указывающее, включён ли корректор орфографии. Значение по умолчанию — false.


**Returns:**
boolean — значение, указывающее, включён ли корректор орфографии.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Устанавливает значение, указывающее, включён ли корректор орфографии. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, включён ли корректор орфографии. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Возвращает максимальное количество ошибок. Значение по умолчанию — 2.


**Returns:**
int - Максимальное количество ошибок.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Устанавливает максимальное количество ошибок. Значение по умолчанию — 2.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество ошибок. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Возвращает значение, указывающее, будут ли возвращены только лучшие результаты. Значение по умолчанию — false.


**Returns:**
boolean - true, если будут возвращены только лучшие результаты; иначе false.

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Устанавливает значение, указывающее, будут ли возвращены только лучшие результаты. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | true, если будут возвращены только лучшие результаты; иначе false. |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Возвращает максимальное превышение минимального количества найденных ошибок. Значение по умолчанию — 0.


**Returns:**
byte - Максимальное превышение минимального количества найденных ошибок.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Устанавливает максимальное превышение минимального количества найденных ошибок. Значение по умолчанию — 0.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | byte | Максимальное превышение минимального количества найденных ошибок. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Возвращает значение, указывающее, должен ли алгоритм рассматривать транспозицию двух соседних символов как одну ошибку. Значение по умолчанию — true.


**Returns:**
boolean - true, если алгоритм исправления орфографии учитывает транспозиции; иначе false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Устанавливает значение, указывающее, должен ли алгоритм рассматривать транспозицию двух соседних символов как одну ошибку. Значение по умолчанию — true.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | true, если алгоритм исправления орфографии учитывает транспозиции; иначе false. |
|

