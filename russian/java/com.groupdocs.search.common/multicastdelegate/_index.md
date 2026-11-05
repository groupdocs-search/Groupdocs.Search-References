---
title: "MulticastDelegate"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет делегат, который ссылается на экземпляры классов, имеющих вызываемый метод."
type: docs
weight: 26
url: /ru/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Представляет делегат, который ссылается на экземпляры классов, имеющие метод для вызова.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Возвращает список вызовов. |
|
|  | [getDelegateId()](#getDelegateId--) | Возвращает идентификатор делегата. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Проверяет два делегата на равенство. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Проверяет два делегата на неравенство. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Возвращает список вызовов.


**Returns:**
com.groupdocs.search.common.Delegate[] - Список вызовов.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Возвращает идентификатор делегата.


**Returns:**
java.lang.String - Идентификатор делегата.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Проверяет два делегата на равенство.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Первый делегат. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Второй делегат. |
|

**Returns:**
boolean - Результат проверки двух делегатов на равенство.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Проверяет два делегата на неравенство.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Первый делегат. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Второй делегат. |
|

**Returns:**
boolean - Результат проверки двух делегатов на неравенство.

