---
title: GetIndexedDocuments
second_title: GroupDocs.Search for .NET API 参考
description: 获取所有索引文档的数组
type: docs
weight: 140
url: /zh/net/groupdocs.search/index/getindexeddocuments/
---
## Index.GetIndexedDocuments method

获取所有索引文档的数组。

```csharp
public DocumentInfo[] GetIndexedDocuments()
```

### 返回值

所有索引文档的数组。

### 例子

该示例演示了如何从索引中获取索引文档列表。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
 
// 索引指定文件夹中的文档
index.Add(documentsFolder);
 
// 获取索引文档列表
DocumentInfo[] documents = index.GetIndexedDocuments();
```

### 也可以看看

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->