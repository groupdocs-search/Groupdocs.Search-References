---
title: EventHub
second_title: GroupDocs.Search for .NET API 参考
description: 为订阅提供索引事件
type: docs
weight: 500
url: /zh/net/groupdocs.search.events/eventhub/
---
## EventHub class

为订阅提供索引事件。

```csharp
public class EventHub
```

## 活动

| 姓名 | 描述 |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search.events/eventhub/erroroccurred) | 在索引操作期间发生错误时发生。 |
| event [FileIndexing](../../groupdocs.search.events/eventhub/fileindexing) | 当文档要被索引时发生。 |
| event [ImagePreparing](../../groupdocs.search.events/eventhub/imagepreparing) | 在准备索引图像时发生。 |
| event [OperationFinished](../../groupdocs.search.events/eventhub/operationfinished) | 在索引操作完成时发生。 |
| event [OperationProgressChanged](../../groupdocs.search.events/eventhub/operationprogresschanged) | 在索引或更新操作的进度发生变化时发生。 |
| event [PasswordRequired](../../groupdocs.search.events/eventhub/passwordrequired) | 当文档需要密码才能打开时发生。 |
| event [SearchPhaseCompleted](../../groupdocs.search.events/eventhub/searchphasecompleted) | 在搜索阶段完成时发生。 |
| event [StatusChanged](../../groupdocs.search.events/eventhub/statuschanged) | 当索引状态改变时发生。 |

### 评论

**学到更多**

* [搜索索引事件](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### 例子

示例演示了接口的典型用法。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// 创建索引
Index index = new Index(indexFolder);

// 订阅事件
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// 索引指定文件夹中的文档
index.Add(documentsFolder);

// 在索引中搜索
SearchResult result = index.Search(query);
```

### 也可以看看

* 命名空间 [GroupDocs.Search.Events](../../groupdocs.search.events)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->