---
title: PasswordRequired
second_title: GroupDocs.Search for .NET API 参考
description: 当文档需要密码才能打开时发生
type: docs
weight: 60
url: /zh/net/groupdocs.search.events/eventhub/passwordrequired/
---
## EventHub.PasswordRequired event

当文档需要密码才能打开时发生。

```csharp
public event EventHandler<PasswordRequiredEventArgs> PasswordRequired;
```

### 例子

示例演示如何使用事件。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// 创建索引
Index index = new Index(indexFolder);

// 订阅事件
index.Events.PasswordRequired += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("ProtectedDocument.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.Password = "123456";
    }
};

// 索引指定文件夹中的文档
index.Add(documentsFolder);
```

### 也可以看看

* class [PasswordRequiredEventArgs](../../passwordrequiredeventargs)
* class [EventHub](../../eventhub)
* 命名空间 [GroupDocs.Search.Events](../../eventhub)
* 部件 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->