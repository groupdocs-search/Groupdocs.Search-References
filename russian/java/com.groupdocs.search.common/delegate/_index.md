---
title: "Delegate"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет делегат, который ссылается на экземпляр класса, имеющий вызываемый метод."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Представляет делегат, который ссылается на экземпляр класса, имеющий метод для вызова.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Возвращает список вызовов. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Объединяет два делегата в один. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Объединяет несколько делегатов в один. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Удаляет делегат-значение из исходного делегата. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Удаляет делегат-значение из исходного делегата. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Проверяет два делегата на равенство. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Проверяет два делегата на неравенство. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Возвращает список вызовов.


**Returns:**
com.groupdocs.search.common.Delegate[] - Список вызовов.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Объединяет два делегата в один.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Первый делегат для объединения. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Второй делегат для объединения. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Объединяет несколько делегатов в один.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Делегаты для объединения. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Удаляет делегат-значение из исходного делегата.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Исходный делегат. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Делегат значения. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Удаляет делегат-значение из исходного делегата.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Исходный делегат. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Делегат значения. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Проверяет два делегата на равенство.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Первый делегат. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Второй делегат. |
|

**Returns:**
boolean - Результат проверки двух делегатов на равенство.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Проверяет два делегата на неравенство.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Первый делегат. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Второй делегат. |
|

**Returns:**
boolean - Результат проверки двух делегатов на неравенство.

