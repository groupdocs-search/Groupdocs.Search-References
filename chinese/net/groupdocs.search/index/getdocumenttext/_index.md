---
title: GetDocumentText
second_title: GroupDocs.Search for .NET API 参考
description: 为索引文档生成 HTML 格式的文本并通过输出适配器传输它
type: docs
weight: 120
url: /zh/net/groupdocs.search/index/getdocumenttext/
---
## GetDocumentText(DocumentInfo, OutputAdapter) {#getdocumenttext}

为索引文档生成 HTML 格式的文本并通过输出适配器传输它。

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| documentInfo | DocumentInfo | 索引的文档信息。 |
| adapter | OutputAdapter | 输出适配器。 |

### 例子

该示例演示了如何从索引中获取索引文档的文本。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
 
// 索引指定文件夹中的文档
index.Add(documentsFolder);
 
// 获取索引文档列表
DocumentInfo[] documents = index.GetIndexedDocuments();
 
// 获取文档文本
if (documents.Length > 0)
{
    FileOutputAdapter outputAdapter = new FileOutputAdapter(@"C:\Text.html");
    index.GetDocumentText(documents[0], outputAdapter);
}
```

### 也可以看看

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

---

## GetDocumentText(DocumentInfo, OutputAdapter, TextOptions) {#getdocumenttext_1}

为索引文档生成 HTML 格式的文本并通过输出适配器传输它。

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| documentInfo | DocumentInfo | 索引的文档信息。 |
| adapter | OutputAdapter | 输出适配器。 |
| options | TextOptions | 文本检索选项。 |

### 也可以看看

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [TextOptions](../../../groupdocs.search.options/textoptions)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->