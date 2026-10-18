---
title: "IndexInfo"
second_title: "GroupDocs.Search для Java API Reference"
description: "Содержит базовую информацию об индексе."
type: docs
weight: 24
url: /ru/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Содержит базовую информацию об индексе.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Получает уникальный идентификатор индекса. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Получает полное имя папки, где находится индекс. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Получает статус индекса. |
|
|  | [getVersion()](#getVersion--) | Получает версию индекса. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Получает количество сегментов индекса. |
|
|  | [getTermCount()](#getTermCount--) | Получает количество слов в индексе. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Получает уникальный идентификатор индекса.


**Returns:**
java.util.UUID - Уникальный идентификатор индекса.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Получает полное имя папки, где находится индекс.


**Returns:**
java.lang.String - Полное имя папки, где находится индекс.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Получает статус индекса.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Получает версию индекса.


**Returns:**
java.lang.String - Версия индекса.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Получает количество сегментов индекса.


**Returns:**
int - Количество сегментов индекса.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Получает количество слов в индексе.


**Returns:**
int - Количество слов в индексе.

