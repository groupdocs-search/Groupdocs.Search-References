---
title: "PathDeleteResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат операции удаления проиндексированного файла или папки из индекса."
type: docs
weight: 18
url: /ru/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Представляет результат операции удаления проиндексированного файла или папки из индекса.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Методы

| Метод | Описание |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Возвращает индикатор успешности операции удаления. |
|
|  | [getError()](#getError--) | Возвращает описание ошибки удаления. |
|
|  | [getPath()](#getPath--) | Возвращает путь к файлу или папке для удаления. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Возвращает индикатор успешности операции удаления.


**Returns:**
boolean -  true  если операция удаления была успешной; в противном случае возвращает  false .

### getError() {#getError--}
```
public final String getError()
```


Возвращает описание ошибки удаления.


**Returns:**
java.lang.String - Описание ошибки удаления.

### getPath() {#getPath--}
```
public final String getPath()
```


Возвращает путь к файлу или папке для удаления.


**Returns:**
java.lang.String - Путь к файлу или папке для удаления.

