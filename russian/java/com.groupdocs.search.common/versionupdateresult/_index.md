---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат операции обновления версии индекса."
type: docs
weight: 42
url: /ru/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Представляет результат операции обновления версии индекса.

## Fields

| Field | Описание |
| --- | --- |
|  | [Updated](#Updated) | Версия индекса обновлена. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Версия индекса уже актуальна. |
|
|  | [Unsupported](#Unsupported) | Версия индекса не поддерживается или каталог не содержит действительных данных индекса. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Версия индекса обновлена.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Версия индекса уже актуальна.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Версия индекса не поддерживается или каталог не содержит действительных данных индекса.


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
