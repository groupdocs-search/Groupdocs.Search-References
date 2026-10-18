---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "추출기, 인덱서, 검색기, 샤드와 같은 서비스를 포함할 수 있는 검색 네트워크 노드를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

추출기, 인덱서, 검색기, 샤드와 같은 서비스를 포함할 수 있는 검색 네트워크 노드를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | SearchNetworkNode 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | SearchNetworkNode 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | SearchNetworkNode 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [start()](#start--) | 검색 네트워크 노드의 기능을 시작합니다. |
|
|  | [configureAllNodes()](#configureAllNodes--) | 검색 네트워크의 모든 노드를 구성합니다. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | 검색 네트워크에서 지정된 노드를 구성합니다. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | 사용자 정의 추출기 컬렉션을 가져옵니다. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | OCR 처리를 위해 사용되는 OCR 커넥터를 설정합니다. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | 단어 형태 제공자를 설정합니다. |
|
|  | [close()](#close--) | SearchNetworkNode가 사용하는 모든 리소스를 해제합니다. |
|
|  | [getNodeIndex()](#getNodeIndex--) | 검색 네트워크 노드의 인덱스를 가져옵니다. |
|
|  | [getEvents()](#getEvents--) | 이벤트 구독을 위한 이벤트 허브를 가져옵니다. |
|
|  | [getIndexer()](#getIndexer--) | 인덱서를 가져옵니다. |
|
|  | [getSearcher()](#getSearcher--) | 검색자를 가져옵니다. |
|
|  | [getShardIndices()](#getShardIndices--) | 검색 네트워크의 모든 샤드 인덱스 배열을 가져옵니다. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | 서비스가 위치한 노드의 인덱스를 가져옵니다. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


SearchNetworkNode 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | nodeIndex | int | 노드 인덱스입니다. |
|
|  | storagePath | java.lang.String | 스토리지 경로. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | 네트워크 설정. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


SearchNetworkNode 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | nodeIndex | int | 노드 인덱스입니다. |
|
|  | storagePath | java.lang.String | 스토리지 경로. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | 네트워크 설정. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | 로거. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


SearchNetworkNode 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | nodeIndex | int | 노드 인덱스입니다. |
|
|  | storagePath | java.lang.String | 스토리지 경로. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | 네트워크 설정. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | 로거. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | 구성. |
|

### start() {#start--}
```
public void start()
```


검색 네트워크 노드의 기능을 시작합니다.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


검색 네트워크의 모든 노드를 구성합니다.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


검색 네트워크에서 지정된 노드를 구성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | nodeIndex | int | 노드 인덱스입니다. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


커스텀 추출기 컬렉션을 가져옵니다. 커스텀 추출기 구현에 대한 전체 예제는 GroupDocs.Search.Common.IFieldExtractor 인터페이스 문서에 제시되어 있습니다.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


OCR 처리를 위해 사용되는 OCR 커넥터를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR 커넥터. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


단어 형태 제공자를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | 단어 형태 제공자. |
|

### close() {#close--}
```
public void close()
```


SearchNetworkNode가 사용하는 모든 리소스를 해제합니다.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


검색 네트워크 노드의 인덱스를 가져옵니다.


**Returns:**
int - 검색 네트워크 노드의 인덱스.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


이벤트 구독을 위한 이벤트 허브를 가져옵니다.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


인덱서를 가져옵니다.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


검색자를 가져옵니다.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


검색 네트워크의 모든 샤드 인덱스 배열을 가져옵니다.


**Returns:**
int[] - 검색 네트워크의 모든 샤드 인덱스 배열.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


서비스가 위치한 노드의 인덱스를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | serviceIndex | int | 서비스 인덱스. |
|

**Returns:**
int - 서비스가 위치한 노드의 인덱스. 서비스 인덱스가 올바르지 않으면 -1이 반환됩니다.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
