---
title: "Extractor"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет инструмент для предварительного извлечения данных из документов, позволяющий отделить этап последующей быстрой индексации."
type: docs
weight: 16
url: /ru/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Представляет инструмент для предварительного извлечения данных из документов, позволяющий отделить этап последующей быстрой индексации.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Extractor()](#Extractor--) | Инициализирует новый экземпляр класса  Extractor . |
|
## Fields

| Field | Описание |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Происходит, когда ошибка возникает во время операции извлечения. |
|
|  | [ImagePreparing](#ImagePreparing) | Происходит, когда изображение готовится к индексации. |
|
|  | [PasswordRequired](#PasswordRequired) | Происходит, когда документ требует пароль для открытия. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getSettings()](#getSettings--) | Получает настройки извлечения. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Извлекает данные из документа. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Инициализирует новый экземпляр класса  Extractor .


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Происходит, когда ошибка возникает во время операции извлечения.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Происходит, когда изображение готовится к индексации.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Происходит, когда документ требует пароль для открытия.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Получает настройки извлечения.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Извлекает данные из документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Документ из файловой системы, потока или структуры. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Параметры извлечения. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| сообщение | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| stream | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
