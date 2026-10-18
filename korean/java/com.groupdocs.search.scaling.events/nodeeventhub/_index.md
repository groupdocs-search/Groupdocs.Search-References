---
title: "NodeEventHub"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "구독을 위한 노드 이벤트를 제공합니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

구독을 위한 노드 이벤트를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## 필드

| 필드 | 설명 |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | 검색 네트워크 구성 프로세스가 완료될 때 발생합니다. |
|
|  | [IndexingCompleted](#IndexingCompleted) | 대기 중인 모든 문서의 인덱싱이 완료될 때 발생합니다. |
|
|  | [DeletionCompleted](#DeletionCompleted) | 대기 중인 모든 문서 삭제가 완료될 때 발생합니다. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | 전체 노드의 최적화가 완료될 때 발생합니다. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | 전체 노드와의 동기화가 완료될 때 발생합니다. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | 대기 중인 모든 속성 변경이 완료될 때 발생합니다. |
|
|  | [StatusChanged](#StatusChanged) | 검색 네트워크 상태가 변경될 때 발생합니다. |
|
|  | [DataExtracted](#DataExtracted) | 문서에서 데이터가 추출될 때 발생합니다. |
|
|  | [DocumentIndexed](#DocumentIndexed) | 문서가 인덱싱될 때 발생합니다. |
|
|  | [DocumentDeleted](#DocumentDeleted) | 문서가 삭제될 때 발생합니다. |
|
|  | [ErrorOccurred](#ErrorOccurred) | 검색 네트워크의 노드 중 하나에서 오류가 발생할 때 발생합니다. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | 인덱싱 작업의 진행 상황이 변경될 때 발생합니다. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | 최적화 작업의 진행 상황이 변경될 때 발생합니다. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


검색 네트워크 구성 프로세스가 완료될 때 발생합니다.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


대기 중인 모든 문서의 인덱싱이 완료될 때 발생합니다.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


대기 중인 모든 문서 삭제가 완료될 때 발생합니다.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


전체 노드의 최적화가 완료될 때 발생합니다.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


전체 노드와의 동기화가 완료될 때 발생합니다.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


대기 중인 모든 속성 변경이 완료될 때 발생합니다.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


검색 네트워크 상태가 변경될 때 발생합니다.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


문서에서 데이터가 추출될 때 발생합니다.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


문서가 인덱싱될 때 발생합니다.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


문서가 삭제될 때 발생합니다.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


검색 네트워크의 노드 중 하나에서 오류가 발생할 때 발생합니다.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


인덱싱 작업의 진행 상황이 변경될 때 발생합니다.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


최적화 작업의 진행 상황이 변경될 때 발생합니다.


