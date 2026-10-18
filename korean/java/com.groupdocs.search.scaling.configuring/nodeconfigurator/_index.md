---
title: "NodeConfigurator"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크 노드 구성자를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

검색 네트워크 노드 구성자를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | TCP 엔드포인트를 설정합니다. |
|
|  | [addLogSink()](#addLogSink--) | 검색 네트워크 노드에 로그 싱크를 추가합니다. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | 검색 네트워크 노드에 검색기 서비스를 추가합니다. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | 검색 네트워크 노드에 인덱서 서비스를 추가합니다. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | 검색 네트워크 노드에 추출기 서비스를 추가합니다. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | 검색 네트워크 노드에 샤드 서비스를 추가합니다. |
|
|  | [completeNode()](#completeNode--) | 검색 네트워크 노드의 구성을 완료합니다. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


TCP 엔드포인트를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | 호스트 이름 또는 주소입니다. |
|
|  | port | int | 포트 번호입니다. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


검색 네트워크 노드에 로그 싱크를 추가합니다.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


검색 네트워크 노드에 검색기 서비스를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 추가 서비스의 저장 경로입니다. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


검색 네트워크 노드에 인덱서 서비스를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 추가 서비스의 저장 경로입니다. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


검색 네트워크 노드에 추출기 서비스를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 추가 서비스의 저장 경로입니다. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


검색 네트워크 노드에 샤드 서비스를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 추가 서비스의 저장 경로입니다. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


검색 네트워크 노드의 구성을 완료합니다.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

