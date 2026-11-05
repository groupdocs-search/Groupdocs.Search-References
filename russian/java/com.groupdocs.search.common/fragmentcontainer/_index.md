---
title: "FragmentContainer"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет контейнер для текстовых фрагментов с выделенными найденными терминами одного поля документа."
type: docs
weight: 22
url: /ru/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Представляет контейнер для текстовых фрагментов с выделенными найденными терминами одного поля документа.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Получает имя поля документа. |
|
|  | [getCount()](#getCount--) | Получает количество содержащихся текстовых фрагментов. |
|
|  | [getFragments()](#getFragments--) | Получает массив содержащихся текстовых фрагментов. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Получает имя поля документа.


**Returns:**
java.lang.String — имя поля документа.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество содержащихся текстовых фрагментов.


**Returns:**
int — количество содержащихся текстовых фрагментов.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Получает массив содержащихся текстовых фрагментов.


**Returns:**
java.lang.String[] — массив содержащихся текстовых фрагментов.

