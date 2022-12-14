---
title: GetIndexingReports
second_title: GroupDocs.Search for .NET API 参考
description: 获取有关索引操作的报告
type: docs
weight: 160
url: /zh/net/groupdocs.search/index/getindexingreports/
---
## Index.GetIndexingReports method

获取有关索引操作的报告。

```csharp
public IndexingReport[] GetIndexingReports()
```

### 返回值

索引报告。

### 例子

该示例演示了如何获取索引报告。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

IndexingReport[] reports = index.GetIndexingReports(); // 获取索引报告
```

### 也可以看看

* class [IndexingReport](../../../groupdocs.search.common/indexingreport)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
