---
title: "EventHub"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "구독을 위한 인덱스 이벤트를 제공합니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

구독을 위한 인덱스 이벤트를 제공합니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 인덱스에서 검색
SearchResult result = index.search(query);
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## 필드

| 필드 | 설명 |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | 인덱스 작업이 완료될 때 발생합니다. |
|
|  | [ErrorOccurred](#ErrorOccurred) | 인덱스 작업 중 오류가 발생할 때 발생합니다. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | 인덱싱 또는 업데이트 작업의 진행 상황이 변경될 때 발생합니다. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | 최적화 작업의 진행 상황이 변경될 때 발생합니다. |
|
|  | [PasswordRequired](#PasswordRequired) | 문서를 열기 위해 비밀번호가 필요할 때 발생합니다. |
|
|  | [FileIndexing](#FileIndexing) | 문서가 인덱싱될 때 발생합니다. |
|
|  | [ImagePreparing](#ImagePreparing) | 이미지를 인덱싱을 위해 준비할 때 발생합니다. |
|
|  | [StatusChanged](#StatusChanged) | 인덱스 상태가 변경될 때 발생합니다. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | 검색 단계가 완료될 때 발생합니다. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


인덱스 작업이 완료될 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("메시지: " + args.getMessage());
System.out.println("인덱스 폴더: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("시간: " + df.format(args.getTime()));
}
});
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


인덱스 작업 중 오류가 발생할 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 인덱스에서 검색
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


인덱싱 또는 업데이트 작업의 진행 상황이 변경될 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("마지막 처리된: " + args.getLastDocumentPath());
System.out.println("결과: " + args.getLastDocumentStatus());
System.out.println("처리된 문서: " + args.getTotalDocuments());
System.out.println("진행률: " + args.getProgressPercentage());
}
});
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


최적화 작업의 진행 상황이 변경될 때 발생합니다.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


문서를 열기 위해 비밀번호가 필요할 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


문서가 인덱싱될 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Tags", "Protected")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("중요")) {
args.setSkipIndexing(true);
}
}
});
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


이미지를 인덱싱을 위해 준비할 때 발생합니다.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


인덱스 상태가 변경될 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 이벤트 구독
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// 작업 완료에 대한 알림이 여기 있어야 합니다
}
}
});
// 비동기 인덱싱을 위한 플래그 설정
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// 지정된 폴더에서 문서를 비동기 인덱싱
// 작업이 완료되기 전에 메서드가 종료됩니다
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


검색 단계가 완료될 때 발생합니다.

예제는 이벤트 사용 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 이벤트 구독
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("검색 단계: " + args.getSearchPhase());
System.out.println("단어: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search("Einstein", options);
 
```
 
````



