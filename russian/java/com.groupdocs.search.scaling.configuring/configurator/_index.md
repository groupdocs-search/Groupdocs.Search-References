---
title: "Configurator"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет конфигуратор поисковой сети."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Представляет конфигуратор поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Configurator()](#Configurator--) | Инициализирует новый экземпляр класса  Configurator . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Начинает настройку параметров индекса для каждого шарда в поисковой сети. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Добавляет узел в конфигурацию поисковой сети. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Завершает процесс конфигурации и возвращает экземпляр конфигурации поисковой сети. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Инициализирует новый экземпляр класса  Configurator .


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Начинает настройку параметров индекса для каждого шарда в поисковой сети.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Добавляет узел в конфигурацию поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | nodeIndex | int | Индекс узла. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Завершает процесс конфигурации и возвращает экземпляр конфигурации поисковой сети.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
