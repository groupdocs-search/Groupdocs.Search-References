---
title: "SimilarityLevel"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет алгоритм нечеткого поиска, который задает уровень схожести."
type: docs
weight: 35
url: /ru/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Представляет алгоритм нечеткого поиска, который задает уровень схожести. Алгоритм уровня схожести вычисляет максимальное количество ошибок для слова, обратно пропорциональное длине слова.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Включение нечёткого поиска
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Создание алгоритма нечеткого поиска
// Эта функция задает 0 как максимальное количество ошибок для слов от 1 до 4 символов.
// Она задает 1 как максимальное количество ошибок для слов от 5 до 9 символов.
// Она задает 2 как максимальное количество ошибок для слов от 10 до 14 символов. И так далее.
SearchResult result = index.search(query, options); // Поиск в индексе
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Инициализирует новый экземпляр класса  SimilarityLevel . |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Инициализирует новый экземпляр класса  SimilarityLevel . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Получает значение уровня схожести для указанной длины термина. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Получает максимальное допустимое количество ошибок для указанной длины термина. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Инициализирует новый экземпляр класса  SimilarityLevel .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | double | Значение уровня схожести. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Инициализирует новый экземпляр класса  SimilarityLevel .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Получает значение уровня схожести для указанной длины термина.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | termLength | int | Длина термина. |
|

**Returns:**
double - Значение уровня схожести.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Получает максимальное допустимое количество ошибок для указанной длины термина.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | termLength | int | Длина термина. |
|

**Returns:**
int - Максимально допустимое количество ошибок.

