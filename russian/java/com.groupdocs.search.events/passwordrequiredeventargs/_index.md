---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события, которое происходит, когда защищённый паролем документ индексируется."
type: docs
weight: 20
url: /ru/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события, которое происходит, когда защищённый паролем документ индексируется.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Получает полный путь к документу. |
|
|  | [getPassword()](#getPassword--) | Получает пароль для открытия документа. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для открытия документа. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Получает полный путь к документу.


**Returns:**
java.lang.String - Полный путь к документу.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Получает пароль для открытия документа.


**Returns:**
java.lang.String - Пароль для открытия документа.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Устанавливает пароль для открытия документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Пароль для открытия документа. |
|

