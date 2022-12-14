---
title: StringOutputAdapter
second_title: GroupDocs.Search for .NET API 参考
description: 表示一个输出适配器它将输出收集为String.
type: docs
weight: 310
url: /zh/net/groupdocs.search.common/stringoutputadapter/
---
## StringOutputAdapter class

表示一个输出适配器，它将输出收集为String.

```csharp
public class StringOutputAdapter : OutputAdapter
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [StringOutputAdapter](stringoutputadapter)() | 初始化[`StringOutputAdapter`](../stringoutputadapter)类. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [GetResult](../../groupdocs.search.common/stringoutputadapter/getresult)() | 获取结果字符串。 |

### 评论

**学到更多**

* [输出适配器](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### 例子

该示例演示了类的典型用法。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引

index.Add(documentsFolder); // 索引指定文件夹中的文档

DocumentInfo[] documents = index.GetIndexedDocuments(); // 获取索引文档的信息

StringOutputAdapter adapter = new StringOutputAdapter(); // 创建一个字符串输出适配器
index.GetDocumentText(documents[0], adapter); // 将文档文本生成到适配器中
String result = adapter.GetResult(); // 得到结果
```

### 也可以看看

* class [OutputAdapter](../outputadapter)
* 命名空间 [GroupDocs.Search.Common](../../groupdocs.search.common)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
