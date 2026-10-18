---
title: "SearchQuery"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет поисковый запрос в виде объекта."
type: docs
weight: 25
url: /ru/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Представляет поисковый запрос в виде объекта.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
 
// Создание подзапроса поиска по диапазону дат
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Создание подзапроса с подстановкой, количество пропущенных слов от 0 до 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Создание подзапроса простого слова
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Установка параметров поиска только для подзапроса 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Создание объекта параметров поиска с увеличенной ёмкостью найденных вхождений
SearchOptions options = new SearchOptions(); // Общие параметры поиска
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Поиск
 
```
 
````


## Методы

| Метод | Описание |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Возвращает имя поля. |
|
|  | [getChildCount()](#getChildCount--) | Возвращает количество дочерних запросов. |
|
|  | [getFirstChild()](#getFirstChild--) | Возвращает первый дочерний запрос. |
|
|  | [getSecondChild()](#getSecondChild--) | Возвращает второй дочерний запрос. |
|
|  | [getChild(int index)](#getChild-int-) | Возвращает дочерний запрос по индексу. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Получает или задает параметры поиска этого seach запроса. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Получает или задает параметры поиска этого seach запроса. |
|
|  | [toString()](#toString--) | Возвращает  System.String  который представляет текущий  SearchQuery  экземпляр. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Создаёт простой запрос слова. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Создаёт запрос шаблона слова. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Создает запрос с регулярным выражением. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Создает запрос с регулярным выражением. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Создает запрос числового диапазона. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Создает запрос диапазона дат. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Создает запрос поиска фразы. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Создает комбинированный запрос, который найдет только документы, найденные для каждого исходного запроса. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Добавляет поле к указанному запросу. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Создает инвертированный запрос, который найдет остальные документы в индексе, в отличие от тех, которые будут найдены оригинальным запросом. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Создает комбинированный запрос, который найдет только документы, найденные для каждого исходного запроса. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Создает комбинированный запрос, который найдет все документы, найденные хотя бы по одному из исходных запросов. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Создает комбинированный запрос, который найдет все документы, найденные хотя бы по одному из исходных запросов. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Создает подстановочный шаблон для поиска фразы. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Создает подстановочный шаблон для поиска фразы. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Возвращает имя поля.


**Returns:**
java.lang.String - Имя поля.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Возвращает количество дочерних запросов.


**Returns:**
int - Количество дочерних запросов.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Возвращает первый дочерний запрос.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Возвращает второй дочерний запрос.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Возвращает дочерний запрос по индексу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Получает или задает параметры поиска этого seach запроса.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Получает или задает параметры поиска этого seach запроса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Возвращает  System.String  который представляет текущий  SearchQuery  экземпляр.


**Returns:**
java.lang.String - System.String, представляющий текущий экземпляр SearchQuery.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Создаёт простой запрос слова.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | терм | java.lang.String | Термин для поиска. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Создаёт запрос шаблона слова.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Шаблон слова. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Создает запрос с регулярным выражением.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pattern | java.lang.String | Шаблон регулярного выражения для сопоставления. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Создает запрос с регулярным выражением.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pattern | java.lang.String | Шаблон регулярного выражения для сопоставления. |
|
|  | options | int | Битовая комбинация значений перечисления, изменяющих регулярное выражение. Это значение должно содержать флаг  RegexOptions.IgnoreCase . |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Создает запрос числового диапазона.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | начало | long | Начальное значение диапазона. |
|
|  | конец | long | Конечное значение диапазона. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Создает запрос диапазона дат.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | начало | java.util.Date | Начальное значение диапазона. |
|
|  | конец | java.util.Date | Конечное значение диапазона. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Создает запрос поиска фразы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Дочерние запросы. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Создает комбинированный запрос, который найдет только документы, найденные для каждого исходного запроса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Имя поля для поиска. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Добавляет поле к указанному запросу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fieldName | java.lang.String | Имя поля для поиска. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос для добавления поля. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Создает инвертированный запрос, который найдет остальные документы в индексе, в отличие от тех, которые будут найдены оригинальным запросом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос для инвертирования. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Создает комбинированный запрос, который найдет только документы, найденные для каждого исходного запроса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос левого дочернего элемента. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос правого дочернего элемента. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Создает комбинированный запрос, который найдет все документы, найденные хотя бы по одному из исходных запросов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос левого дочернего элемента. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос правого дочернего элемента. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Создает комбинированный запрос, который найдет все документы, найденные хотя бы по одному из исходных запросов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Дочерние запросы. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Создает подстановочный шаблон для поиска фразы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | count | int | Количество слов в подстановочном знаке. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Создает подстановочный шаблон для поиска фразы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | minCount | int | Минимальное количество слов в подстановочном знаке. |
|
|  | maxCount | int | Максимальное количество слов в подстановочном знаке. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

