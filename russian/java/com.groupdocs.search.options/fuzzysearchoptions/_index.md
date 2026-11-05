---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры нечеткого поиска."
type: docs
weight: 21
url: /ru/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Предоставляет параметры нечеткого поиска.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Возвращает значение, указывающее, включена ли функция нечеткого поиска. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Устанавливает значение, указывающее, включена ли функция нечеткого поиска. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Получает алгоритм нечеткого поиска. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Устанавливает алгоритм нечеткого поиска. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Возвращает значение, указывающее, будут ли возвращаться только лучшие результаты. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Устанавливает значение, указывающее, будут ли возвращаться только лучшие результаты. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Возвращает максимальное превышение минимального количества найденных ошибок. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Устанавливает максимальное превышение минимального количества найденных ошибок. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Получает значение, указывающее, должен ли алгоритм нечеткого поиска рассматривать транспозицию двух соседних символов как одну ошибку. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Устанавливает значение, указывающее, должен ли алгоритм нечеткого поиска рассматривать транспозицию двух соседних символов как одну ошибку. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Получает значение, указывающее, включена ли функция нечеткого поиска. Значение по умолчанию — false.


**Returns:**
boolean — значение, указывающее, включена ли функция нечеткого поиска.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Устанавливает значение, указывающее, включена ли функция нечеткого поиска. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, включена ли функция нечеткого поиска. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Получает алгоритм нечеткого поиска. В настоящее время доступные алгоритмы нечеткого поиска —  SimilarityLevel  и  TableDiscreteFunction . Значение по умолчанию — экземпляр  SimilarityLevel  с уровнем сходства 0.5.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Пример демонстрирует, как установить алгоритм нечеткого поиска.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Включение нечёткого поиска
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Создание алгоритма нечёткого поиска
// Эта функция задаёт 1 как максимальное количество ошибок для слов от 1 до 4 символов.
// Она задаёт 2 как максимальное количество ошибок для слов от 5 до 7 символов.
// Она задаёт 3 как максимальное количество ошибок для слов от 8 и более символов.
SearchResult result = index.search(query, options); // Поиск в индексе
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Устанавливает алгоритм нечеткого поиска. В настоящее время доступные алгоритмы нечеткого поиска —  SimilarityLevel  и  TableDiscreteFunction . Значение по умолчанию — экземпляр  SimilarityLevel  с уровнем сходства 0.5.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Алгоритм нечеткого поиска. |


Пример демонстрирует, как установить алгоритм нечеткого поиска.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Включение нечёткого поиска
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Создание алгоритма нечёткого поиска
// Эта функция задаёт 1 как максимальное количество ошибок для слов от 1 до 4 символов.
// Она задаёт 2 как максимальное количество ошибок для слов от 5 до 7 символов.
// Она задаёт 3 как максимальное количество ошибок для слов от 8 и более символов.
SearchResult result = index.search(query, options); // Поиск в индексе
 
```
 
````

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


Получает значение, указывающее, должен ли алгоритм нечеткого поиска рассматривать транспозицию двух соседних символов как одну ошибку. Значение по умолчанию — true.


**Returns:**
boolean — true, если алгоритм нечеткого поиска учитывает транспозиции; иначе false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Устанавливает значение, указывающее, должен ли алгоритм нечеткого поиска рассматривать транспозицию двух соседних символов как одну ошибку. Значение по умолчанию — true.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | :  true  если алгоритм нечеткого поиска учитывает транспозиции; иначе  false . |
|

