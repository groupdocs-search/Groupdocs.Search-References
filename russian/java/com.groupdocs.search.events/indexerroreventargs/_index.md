---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события возникновения ошибки индекса."
type: docs
weight: 16
url: /ru/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события возникновения ошибки индекса.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getMessage()](#getMessage--) | Получает сообщение об ошибке. |
|
|  | [isCritical()](#isCritical--) | Возвращает флаг, указывающий, что произошедшая ошибка критична и индекс следует перезапустить. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Получает сообщение об ошибке.


**Returns:**
java.lang.String - Сообщение об ошибке.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Возвращает флаг, указывающий, что произошедшая ошибка критична и индекс следует перезапустить.


**Returns:**
boolean - Флаг, указывающий, что произошедшая ошибка критична и индекс следует перезапустить.

