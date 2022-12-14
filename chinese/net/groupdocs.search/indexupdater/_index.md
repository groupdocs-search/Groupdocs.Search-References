---
title: IndexUpdater
second_title: GroupDocs.Search for .NET API 参考
description: 表示索引更新器 该类在旧版本的索引中执行重新索引文档
type: docs
weight: 680
url: /zh/net/groupdocs.search/indexupdater/
---
## IndexUpdater class

表示索引更新器。 该类在旧版本的索引中执行重新索引文档。

```csharp
public class IndexUpdater
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [IndexUpdater](indexupdater)() | 初始化[`IndexUpdater`](../indexupdater)类. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | 检查指定目录中的索引是否可以更新到最新版本。 |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | 检查指定目录是否包含最新版本的索引。 |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | 在旧版本的索引中执行重新索引文档。 更新后的索引将放置在*newIndexPath*directory. 中的索引*indexPath*目录不会改变。 |

### 评论

**学到更多**

* [更新索引](https://docs.groupdocs.com/display/searchnet/Update+index)

### 例子

该示例演示了类的典型用法。

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### 也可以看看

* 命名空间 [GroupDocs.Search](../../groupdocs.search)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
