---
title: "NodeConfigurator"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет конфигуратор узла поисковой сети."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Представляет конфигуратор узла поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Устанавливает TCP‑конечную точку. |
|
|  | [addLogSink()](#addLogSink--) | Добавляет приемник журналов в узел поисковой сети. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Добавляет сервис поиска в узел поисковой сети. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Добавляет сервис индексатора в узел поисковой сети. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Добавляет сервис извлечения в узел поисковой сети. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Добавляет сервис шарда в узел поисковой сети. |
|
|  | [completeNode()](#completeNode--) | Завершает настройку узла поисковой сети. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Устанавливает TCP‑конечную точку.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Имя хоста или адрес. |
|
|  | port | int | Номер порта. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Добавляет приемник журналов в узел поисковой сети.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Добавляет сервис поиска в узел поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | storagePath | java.lang.String | Путь к хранилищу добавляемого сервиса. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Добавляет сервис индексатора в узел поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | storagePath | java.lang.String | Путь к хранилищу добавляемого сервиса. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Добавляет сервис извлечения в узел поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | storagePath | java.lang.String | Путь к хранилищу добавляемого сервиса. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Добавляет сервис шарда в узел поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | storagePath | java.lang.String | Путь к хранилищу добавляемого сервиса. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Завершает настройку узла поисковой сети.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

