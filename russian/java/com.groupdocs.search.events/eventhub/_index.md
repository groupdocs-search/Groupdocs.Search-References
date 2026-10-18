---
title: "EventHub"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет события индекса для подписки."
type: docs
weight: 12
url: /ru/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Предоставляет события индекса для подписки.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Индексация документов из указанной папки
index.add(documentsFolder);
// Поиск в индексе
SearchResult result = index.search(query);
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | Описание |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Происходит, когда операция индекса завершена. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Происходит, когда во время операции индекса происходит ошибка. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Происходит, когда изменяется прогресс операции индексации или обновления. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Происходит, когда изменяется прогресс операции оптимизации. |
|
|  | [PasswordRequired](#PasswordRequired) | Происходит, когда документ требует пароль для открытия. |
|
|  | [FileIndexing](#FileIndexing) | Происходит, когда документ будет проиндексирован. |
|
|  | [ImagePreparing](#ImagePreparing) | Происходит, когда изображение готовится к индексации. |
|
|  | [StatusChanged](#StatusChanged) | Происходит, когда статус индекса изменяется. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Происходит, когда фаза поиска завершена. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Происходит, когда операция индекса завершена.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Сообщение: " + args.getMessage());
System.out.println("Папка индекса: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Время: " + df.format(args.getTime()));
}
});
// Индексация документов из указанной папки
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Происходит, когда во время операции индекса происходит ошибка.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Индексация документов из указанной папки
index.add(documentsFolder);
// Поиск в индексе
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Происходит, когда изменяется прогресс операции индексации или обновления.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Последний обработанный: " + args.getLastDocumentPath());
System.out.println("Результат: " + args.getLastDocumentStatus());
System.out.println("Обработанные документы: " + args.getTotalDocuments());
System.out.println("Процент выполнения: " + args.getProgressPercentage());
}
});
// Индексация документов из указанной папки
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Происходит, когда изменяется прогресс операции оптимизации.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Происходит, когда документ требует пароль для открытия.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Индексация документов из указанной папки
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Происходит, когда документ будет проиндексирован.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Теги", "Защищено")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("важный")) {
args.setSkipIndexing(true);
}
}
});
// Индексация документов из указанной папки
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Происходит, когда изображение готовится к индексации.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Происходит, когда статус индекса изменяется.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Подписка на событие
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Здесь должно быть уведомление о завершении операции
}
}
});
// Установка флага для асинхронного индексирования
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Асинхронное индексирование документов из указанной папки
// Метод завершается до завершения операции
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Происходит, когда фаза поиска завершена.

Пример демонстрирует, как использовать событие.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Подписка на событие
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Search phase: " + args.getSearchPhase());
System.out.println("Words: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search("Einstein", options);
 
```
 
````



