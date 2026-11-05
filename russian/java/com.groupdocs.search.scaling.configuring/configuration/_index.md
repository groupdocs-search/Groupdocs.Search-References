---
title: "Конфигурация"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет конфигурацию поисковой сети."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Представляет конфигурацию поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Сохраняет эту конфигурацию в файл. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Сохраняет эту конфигурацию в поток. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Загружает конфигурацию поисковой сети из файла. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Загружает конфигурацию поисковой сети из потока. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Сохраняет эту конфигурацию в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Файл для сохранения. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Сохраняет эту конфигурацию в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Поток для сохранения. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Загружает конфигурацию поисковой сети из файла.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Файл для загрузки. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Загружает конфигурацию поисковой сети из потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.InputStream | Поток, из которого загружать. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

