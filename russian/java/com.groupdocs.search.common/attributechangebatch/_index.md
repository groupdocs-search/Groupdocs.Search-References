---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет контейнер для изменений атрибутов."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Представляет контейнер для изменений атрибутов.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Инициализирует новый экземпляр класса  AttributeChangeBatch . |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Инициализирует новый экземпляр класса  AttributeChangeBatch . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Добавляет указанные атрибуты в указанный индексированный документ. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Добавляет указанные атрибуты в указанные индексированные документы. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Добавляет указанные атрибуты ко всем документам в индексе. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Удаляет указанные атрибуты из указанного индексированного документа. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Удаляет указанные атрибуты из указанных индексированных документов. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Удаляет все атрибуты из указанного индексированного документа. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Удаляет все атрибуты из указанных индексированных документов. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Удаляет указанные атрибуты из всех документов в индексе. |
|
|  | [clear()](#clear--) | Удаляет все атрибуты из всех документов в индексе. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Инициализирует новый экземпляр класса  AttributeChangeBatch .


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Инициализирует новый экземпляр класса  AttributeChangeBatch .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Добавляет указанные атрибуты в указанный индексированный документ.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | путь | java.lang.String | Путь к документу. |
|
|  | атрибуты | java.lang.String[] | Атрибуты для добавления. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Добавляет указанные атрибуты в указанные индексированные документы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пути | java.lang.String[] | Пути к документам. |
|
|  | атрибуты | java.lang.String[] | Атрибуты для добавления. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Добавляет указанные атрибуты ко всем документам в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | атрибуты | java.lang.String[] | Атрибуты для добавления. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Удаляет указанные атрибуты из указанного индексированного документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | путь | java.lang.String | Путь к документу. |
|
|  | атрибуты | java.lang.String[] | Атрибуты для удаления. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Удаляет указанные атрибуты из указанных индексированных документов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пути | java.lang.String[] | Пути к документам. |
|
|  | атрибуты | java.lang.String[] | Атрибуты для удаления. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Удаляет все атрибуты из указанного индексированного документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | путь | java.lang.String | Путь к документу. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Удаляет все атрибуты из указанных индексированных документов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пути | java.lang.String[] | Пути к документам. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Удаляет указанные атрибуты из всех документов в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | атрибуты | java.lang.String[] | Атрибуты для удаления. |
|

### clear() {#clear--}
```
public void clear()
```


Удаляет все атрибуты из всех документов в индексе.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
