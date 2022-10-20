---
title: License
second_title: GroupDocs.Search for .NET API 参考
description: 提供申请许可证的方法
type: docs
weight: 690
url: /zh/net/groupdocs.search/license/
---
## License class

提供申请许可证的方法。

```csharp
public sealed class License
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [License](license)() | 初始化[`License`](../license)类. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense)(Stream) | 许可组件。 |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense_1)(string) | 许可组件。 |

### 评论

**学到更多**

* [评估限制和许可](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### 例子

该示例演示如何设置许可证。

```csharp
License license = new License();
license.SetLicense("C:\\GroupDocs.Search.lic");
```

### 也可以看看

* 命名空间 [GroupDocs.Search](../../groupdocs.search)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->