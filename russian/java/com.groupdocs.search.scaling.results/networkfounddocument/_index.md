---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет найденный документ в поисковой сети."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Представляет найденный документ в поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Получает найденный документ. |
|
|  | [getShardIndex()](#getShardIndex--) | Получает индекс шарда. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Получает найденный документ.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Получает индекс шарда.


**Returns:**
int - Индекс шарда.

