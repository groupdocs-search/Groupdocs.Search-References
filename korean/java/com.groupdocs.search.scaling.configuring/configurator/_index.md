---
title: "Configurator"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크 구성자를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

검색 네트워크 구성자를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Configurator()](#Configurator--) | 새로운 Configurator 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | 검색 네트워크의 각 샤드에 대한 인덱스 설정 구성을 시작합니다. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | 검색 네트워크 구성에 노드를 추가합니다. |
|
|  | [completeConfiguration()](#completeConfiguration--) | 구성 프로세스를 완료하고 검색 네트워크 구성 인스턴스를 반환합니다. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


새로운 Configurator 클래스 인스턴스를 초기화합니다.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


검색 네트워크의 각 샤드에 대한 인덱스 설정 구성을 시작합니다.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


검색 네트워크 구성에 노드를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | nodeIndex | int | 노드 인덱스입니다. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


구성 프로세스를 완료하고 검색 네트워크 구성 인스턴스를 반환합니다.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
