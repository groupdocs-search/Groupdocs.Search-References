---
title: "Уведомление"
second_title: "GroupDocs.Search для Java API Reference"
description: "Базовый класс для всех уведомлений индекса."
type: docs
weight: 22
url: /ru/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

Базовый класс для всех уведомлений в индексе. Этот класс также содержит методы для создания объектов уведомлений.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Notification()](#Notification--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Создаёт объект уведомления для переименования проиндексированного документа, который был переименован и не требует переиндексации. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Создаёт объект уведомления для переименования проиндексированного документа, который был переименован и не требует переиндексации. Переименованный документ не будет переиндексирован во время следующей операции обновления, даже если его содержимое было изменено.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | oldPath | java.lang.String | Старый путь к проиндексированному документу. |
|
|  | newPath | java.lang.String | Новый путь к проиндексированному документу. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

