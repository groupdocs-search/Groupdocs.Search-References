---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет алгоритм нечеткого поиска, содержащий соответствия между длинами слов и количеством допустимых ошибок."
type: docs
weight: 40
url: /ru/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Представляет алгоритм нечёткого поиска, который содержит соответствия между длинами слов и количеством допустимых ошибок. Этот алгоритм можно задать таблицей выходных значений или ступенчатой функцией.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Создание алгоритма нечёткого поиска
// Эта функция задаёт 1 как максимальное количество ошибок для слов от 1 до 4 символов.
// Она задаёт 2 как максимальное количество ошибок для слов от 5 до 7 символов.
// Она задаёт 3 как максимальное количество ошибок для слов от 8 и более символов.
SearchResult result = index.search(query, options); // Поиск в индексе
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Инициализирует новый экземпляр класса  TableDiscreteFunction  . |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Инициализирует новый экземпляр класса  TableDiscreteFunction  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Получает уровень схожести для указанной длины термина. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Получает максимальное допустимое количество ошибок для указанной длины термина. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Инициализирует новый экземпляр класса  TableDiscreteFunction  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | offsetOfInputs | int | Смещение индексов таблицы относительно входных значений. |
|
|  | tableOfOutputs | int[] | Таблица выходных значений. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Инициализирует новый экземпляр класса  TableDiscreteFunction  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | firstStepLevel | int | Уровень первого шага ступенчатой функции. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Следующие шаги ступенчатой функции. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Получает уровень схожести для указанной длины термина.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | termLength | int | Длина термина. |
|

**Returns:**
double - Уровень схожести.

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
int - Максимальное допустимое количество ошибок.

