---
title: "SearchOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для операции поиска."
type: docs
weight: 34
url: /ru/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Предоставляет параметры для операции поиска.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Инициализирует новый экземпляр класса SearchOptions. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Инициализирует новый экземпляр класса SearchOptions. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Получает флаг использования синонимов в поиске. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Устанавливает флаг использования синонимов в поиске. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Получает флаг использования омонимов в поиске. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Устанавливает флаг использования омонимов в поиске. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Получает флаг использования различных форм слов в поиске. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Устанавливает флаг использования различных форм слов в поиске. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Получает флаг получения атрибутов, связанных с найденными документами. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Устанавливает флаг получения атрибутов, связанных с найденными документами. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Получает параметры нечеткого поиска. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Получает параметры корректора орфографии. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Получает параметры корректора раскладки клавиатуры. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Получает флаг поиска с учетом регистра. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Устанавливает флаг поиска с учетом регистра. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Получает максимальное общее количество вхождений всех терминов в поисковом запросе. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Устанавливает максимальное общее количество вхождений всех терминов в поисковом запросе. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Получает максимальное количество вхождений каждого термина в поисковом запросе. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Устанавливает максимальное количество вхождений каждого термина в поисковом запросе. |
|
|  | [getDateFormats()](#getDateFormats--) | Получает коллекцию форматов дат для поиска диапазона дат. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Получает флаг поиска по фрагментам. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Устанавливает флаг поиска по фрагментам. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Получает фильтр поискового документа. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Устанавливает фильтр поиска документов. |
|
|  | [getCancellation()](#getCancellation--) | Получает объект отмены операции. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Устанавливает объект отмены операции. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Инициализирует новый экземпляр класса SearchOptions.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Инициализирует новый экземпляр класса SearchOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Получает флаг использования синонимов в поиске. Значение по умолчанию — false.


**Returns:**
boolean - Флаг использования синонимов в поиске.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Устанавливает флаг использования синонимов в поиске. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг использования синонимов в поиске. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Получает флаг использования омонимов в поиске. Значение по умолчанию — false.


**Returns:**
boolean - Флаг использования омонимов в поиске.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Устанавливает флаг использования омонимов в поиске. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг использования омонимов в поиске. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Получает флаг использования разных форм слов в поиске. Значение по умолчанию — false.


**Returns:**
boolean - Флаг использования разных форм слов в поиске.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Устанавливает флаг использования разных форм слов в поиске. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг использования различных форм слов при поиске. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Получает флаг получения атрибутов, связанных с найденными документами. Значение по умолчанию — false.


**Returns:**
boolean - Флаг получения атрибутов, связанных с найденными документами.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Устанавливает флаг получения атрибутов, связанных с найденными документами. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг получения атрибутов, связанных с найденными документами. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Получает параметры нечеткого поиска.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Получает параметры корректора орфографии.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Получает параметры корректора раскладки клавиатуры.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Получает флаг чувствительного к регистру поиска. Значение по умолчанию — false.


**Returns:**
boolean - Флаг чувствительного к регистру поиска.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Устанавливает флаг чувствительного к регистру поиска. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг чувствительного к регистру поиска. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Получает максимальное общее количество вхождений всех терминов в запросе поиска. Значение по умолчанию — 500000.


**Returns:**
int - Максимальное общее количество вхождений.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Устанавливает максимальное общее количество вхождений всех терминов в запросе поиска. Значение по умолчанию — 500000.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное общее количество вхождений. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Получает максимальное количество вхождений каждого термина в запросе поиска. Значение по умолчанию — 100000.


**Returns:**
int - Максимальное количество вхождений каждого термина в запросе поиска.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Устанавливает максимальное количество вхождений каждого термина в запросе поиска. Значение по умолчанию — 100000.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество вхождений каждого термина в запросе поиска. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Получает коллекцию форматов дат для поиска по диапазону дат. Форматы дат по умолчанию: 'dd.MM.yyyy', 'MM/dd/yyyy' и 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Пример демонстрирует, как установить форматы дат для поиска.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Удаление форматов даты по умолчанию
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Создание шаблона формата даты 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Поиск в индексе
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Получает флаг поиска по фрагментам. Значение по умолчанию — false.


**Returns:**
boolean - Флаг поиска по фрагментам.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Устанавливает флаг поиска по фрагментам. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг поиска по фрагментам. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Получает фильтр документов поиска. SearchDocumentFilter работает по принципу включения. Используйте класс SearchDocumentFilter для создания экземпляров фильтра документов поиска. Значение по умолчанию — null, что означает, что будут возвращены все найденные документы.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Пример демонстрирует, как установить фильтр документов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов
index.add(documentsFolder);
// Создание фильтра документов поиска, который пропускает документы с расширениями '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Создание фильтра расширения файлов
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Инвертирование фильтра расширения файлов
options.setSearchDocumentFilter(invertedFilter);
// Поиск в индексе
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Устанавливает фильтр документов поиска.  SearchDocumentFilter работает по логике включения. Используйте класс SearchDocumentFilter для создания экземпляров фильтра документов поиска. Значение по умолчанию — null, что означает, что будут возвращены все найденные документы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Фильтр документов поиска. |


Пример демонстрирует, как установить фильтр документов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов
index.add(documentsFolder);
// Создание фильтра документов поиска, который пропускает документы с расширениями '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Создание фильтра расширения файлов
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Инвертирование фильтра расширения файлов
options.setSearchDocumentFilter(invertedFilter);
// Поиск в индексе
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Получает объект отмены операции. Значение по умолчанию — null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Устанавливает объект отмены операции. Значение по умолчанию — null.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Объект отмены операции. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
