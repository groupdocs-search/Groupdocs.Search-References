---
title: StatusChanged
second_title: GroupDocs..NET API 참조 검색
description: 인덱스 상태가 변경되면 발생합니다.
type: docs
weight: 80
url: /ko/net/groupdocs.search.events/eventhub/statuschanged/
---
## EventHub.StatusChanged event

인덱스 상태가 변경되면 발생합니다.

```csharp
public event EventHandler<BaseIndexEventArgs> StatusChanged;
```

### 예

예제는 이벤트를 사용하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// 인덱스 생성
Index index = new Index(indexFolder);

// 이벤트 구독
index.Events.StatusChanged += (sender, args) =>
{
    if (args.Status != IndexStatus.InProgress)
    {
        // 작업 완료 알림이 여기에 있어야 합니다.
    }
};

// 비동기 인덱싱을 위한 플래그 설정
IndexingOptions options = new IndexingOptions();
options.IsAsync = true;

// 지정된 폴더의 비동기 색인 문서
// 작업이 완료되기 전에 메서드가 종료됩니다.
index.Add(documentsFolder, options);
```

### 또한보십시오

* class [BaseIndexEventArgs](../../baseindexeventargs)
* class [EventHub](../../eventhub)
* 네임스페이스 [GroupDocs.Search.Events](../../eventhub)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->