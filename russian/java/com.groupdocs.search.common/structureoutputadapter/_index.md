---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет выходной адаптер, который собирает вывод в виде структуры, содержащей каждое поле отдельно."
type: docs
weight: 33
url: /ru/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Представляет выходной адаптер, который собирает вывод в виде структуры, содержащей каждое поле отдельно.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Инициализирует новый экземпляр класса StructureOutputAdapter. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getResult()](#getResult--) | Получает результирующий массив полей. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Инициализирует новый экземпляр класса StructureOutputAdapter.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Формат вывода. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Получает результирующий массив полей.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Результирующий массив полей.

