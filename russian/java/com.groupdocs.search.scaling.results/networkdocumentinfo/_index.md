---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет дескриптор проиндексированного документа в поисковой сети."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Представляет дескриптор проиндексированного документа в поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Получает дескриптор индексированного документа. |
|
|  | [getShardIndex()](#getShardIndex--) | Получает индекс шарда. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Получает дескриптор индексированного документа.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Получает индекс шарда.


**Returns:**
int - Индекс шарда.

