---
title: OperationProgressChanged
second_title: GroupDocs..NET API 참조 검색
description: 인덱싱 또는 업데이트 작업의 진행률이 변경된 경우 발생합니다.
type: docs
weight: 50
url: /ko/net/groupdocs.search.events/eventhub/operationprogresschanged/
---
## EventHub.OperationProgressChanged event

인덱싱 또는 업데이트 작업의 진행률이 변경된 경우 발생합니다.

```csharp
public event EventHandler<OperationProgressEventArgs> OperationProgressChanged;
```

### 예

예제는 이벤트를 사용하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// 인덱스 생성
Index index = new Index(indexFolder);

// 이벤트 구독
index.Events.OperationProgressChanged += (sender, args) =>
{
    Console.WriteLine("Last processed: " + args.LastDocumentPath);
    Console.WriteLine("Result: " + args.LastDocumentStatus);
    Console.WriteLine("Processed documents: " + args.TotalDocuments);
    Console.WriteLine("Progress percentage: " + args.ProgressPercentage);
};

// 지정된 폴더에서 문서 인덱싱
index.Add(documentsFolder);
```

### 또한보십시오

* class [OperationProgressEventArgs](../../operationprogresseventargs)
* class [EventHub](../../eventhub)
* 네임스페이스 [GroupDocs.Search.Events](../../eventhub)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->