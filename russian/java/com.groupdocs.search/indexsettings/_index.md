---
title: "IndexSettings"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет настройки индекса, позволяющие настраивать операции индексации."
type: docs
weight: 19
url: /ru/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Представляет настройки индекса, позволяющие настраивать операции индексации.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Установка типа индекса
Index index = new Index(indexFolder, settings); // Создание индекса
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Инициализирует новый экземпляр класса IndexSettings. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Возвращает значение, указывающее, хранится ли индекс в памяти или на диске. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Возвращает значение, указывающее, использовать ли стоп-слова. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Устанавливает значение, указывающее, использовать ли стоп-слова. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Возвращает максимальное количество отчетов индексации. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Устанавливает максимальное количество отчетов индексации. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Возвращает максимальное количество отчетов поиска. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Устанавливает максимальное количество отчетов поиска. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Возвращает значение, указывающее, использовать ли замену символов. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Устанавливает значение, указывающее, использовать ли замену символов. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Возвращает фильтр документов. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Устанавливает фильтр документов. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Возвращает настройки хранения текста. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Устанавливает настройки хранения текста. |
|
|  | [getIndexType()](#getIndexType--) | Возвращает тип индекса. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Устанавливает тип индекса. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Получает количество потоков, используемых для поиска. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Устанавливает количество потоков, используемых для поиска. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Получает пользовательскую коллекцию извлекателей. |
|
|  | [getLogger()](#getLogger--) | Получает регистратор, который используется для записи событий и ошибок в индексе. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Устанавливает регистратор, который используется для записи событий и ошибок в индексе. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Инициализирует новый экземпляр класса IndexSettings.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Возвращает значение, указывающее, хранится ли индекс в памяти или на диске.


**Returns:**
boolean - Значение, указывающее, хранится ли индекс в памяти или на диске.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Получает значение, указывающее, использовать ли стоп-слова. Значение по умолчанию —  true .


**Returns:**
boolean - Значение, указывающее, использовать ли стоп-слова.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Устанавливает значение, указывающее, использовать ли стоп-слова. Значение по умолчанию —  true .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, использовать ли стоп-слова. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Получает максимальное количество отчетов индексации. Значение по умолчанию —  5 .


**Returns:**
int - Максимальное количество отчетов индексации.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Устанавливает максимальное количество отчетов индексации. Значение по умолчанию —  5 .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество отчетов индексации. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Получает максимальное количество отчетов поиска. Значение по умолчанию —  10 .


**Returns:**
int - Максимальное количество отчетов поиска.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Устанавливает максимальное количество отчетов поиска. Значение по умолчанию —  10 .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество отчетов поиска. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Получает значение, указывающее, использовать ли замену символов. Значение по умолчанию —  false .


**Returns:**
boolean - Значение, указывающее, использовать ли замену символов.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Устанавливает значение, указывающее, использовать ли замену символов. Значение по умолчанию —  false .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, использовать ли замену символов. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Получает фильтр документов. Класс  DocumentFilter  работает по принципу включения. Используйте класс  DocumentFilter  для создания экземпляра фильтра документов. Значение по умолчанию —  null , что означает, что все добавленные документы индексируются.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Пример демонстрирует, как установить фильтр документов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание фильтра, который пропускает документы с расширениями '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Создание фильтра по расширению файлов
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Инвертирование фильтра по расширению файлов
settings.setDocumentFilter(invertedFilter);
// Создание индекса в указанной папке
Index index = new Index(indexFolder, settings);
// Индексация документов
index.add(documentsFolder);
// Поиск
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Устанавливает фильтр документов. Класс  DocumentFilter  работает по логике включения. Используйте класс  GroupDocs.Search.Options.DocumentFilter  для создания экземпляров фильтра документов. Значение по умолчанию —  null , что означает, что все добавленные документы индексируются.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Фильтр документов. |

Пример демонстрирует, как установить фильтр документов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание фильтра, который пропускает документы с расширениями '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Создание фильтра по расширению файлов
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Инвертирование фильтра по расширению файлов
settings.setDocumentFilter(invertedFilter);
// Создание индекса в указанной папке
Index index = new Index(indexFolder, settings);
// Индексация документов
index.add(documentsFolder);
// Поиск
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Получает настройки хранения текста. Значение по умолчанию —  null , что означает, что тексты документов не сохраняются.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Пример демонстрирует, как установить настройки хранения текста.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание экземпляра настроек индекса
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Установка высокого уровня сжатия для хранения текста индекса
// Создание индекса в указанной папке
Index index = new Index(indexFolder, settings);
// Индексация документов
index.add(documentsFolder);
// Поиск
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Устанавливает настройки хранения текста. Значение по умолчанию —  null , что означает, что тексты документов не сохраняются.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Настройки хранения текста. |

Пример демонстрирует, как установить настройки хранения текста.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание экземпляра настроек индекса
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Установка высокого уровня сжатия для хранения текста индекса
// Создание индекса в указанной папке
Index index = new Index(indexFolder, settings);
// Индексация документов
index.add(documentsFolder);
// Поиск
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Получает тип индекса. Значение по умолчанию —  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Устанавливает тип индекса. Значение по умолчанию —  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Тип индекса. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Получает количество потоков, используемых для поиска. Значение по умолчанию —  GroupDocs.Search.Options.NumberOfThreads.Default , что означает, что поиск будет выполняться с использованием количества потоков, равного количеству ядер процессора.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Устанавливает количество потоков, используемых для поиска. Значение по умолчанию —  GroupDocs.Search.Options.NumberOfThreads.Default , что означает, что поиск будет выполняться с использованием количества потоков, равного количеству ядер процессора.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Количество потоков, используемых для поиска. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Получает коллекцию пользовательских извлекателей. Полный пример реализации пользовательского извлекателя представлен в документации для интерфейса  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Получает логгер, используемый для записи событий и ошибок в индексе. Обратите внимание, что логгер не сохраняется и должен создаваться и назначаться каждый раз при создании или загрузке индекса.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Устанавливает регистратор, который используется для записи событий и ошибок в индексе. Обратите внимание, что регистратор не сохраняется и должен создаваться и назначаться каждый раз при создании или загрузке индекса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Регистратор, который используется для записи событий и ошибок в индексе. |
|

