---
title: AliasDictionary
second_title: GroupDocs.Search for .NET API 参考
description: 表示别名字典
type: docs
weight: 340
url: /zh/net/groupdocs.search.dictionaries/aliasdictionary/
---
## AliasDictionary class

表示别名字典。

```csharp
public class AliasDictionary : DictionaryBase, IEnumerable<string>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/aliasdictionary/count) { get; } | 获取包含在[`AliasDictionary`](../aliasdictionary). |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/aliasdictionary/add)(string, string) | 将指定的别名对和关联文本添加到[`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange)(AliasReplacementPair[]) | 将指定的别名/替换对集合添加到[`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_1)(IEnumerable&lt;AliasReplacementPair&gt;) | 将指定的别名/替换对集合添加到[`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;string, string&gt;&gt;) | 将指定的别名/替换对集合添加到[`AliasDictionary`](../aliasdictionary). |
| [Clear](../../groupdocs.search.dictionaries/aliasdictionary/clear)() | 删除所有别名[`AliasDictionary`](../aliasdictionary)对象. |
| [Contains](../../groupdocs.search.dictionaries/aliasdictionary/contains)(string) | 确定是否[`AliasDictionary`](../aliasdictionary)对象包含指定的别名。 |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | 将字典导出到具有指定名称的文件。 |
| [GetEnumerator](../../groupdocs.search.dictionaries/aliasdictionary/getenumerator)() | 返回一个遍历集合的枚举器。 |
| [GetText](../../groupdocs.search.dictionaries/aliasdictionary/gettext)(string) | 获取与指定别名关联的文本。 |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | 从指定文件导入字典。 |
| [Remove](../../groupdocs.search.dictionaries/aliasdictionary/remove)(string) | 从[`AliasDictionary`](../aliasdictionary)对象. |

### 评论

**学到更多**

* [使用别名](https://docs.groupdocs.com/display/searchnet/Using+aliases)
* [管理别名字典](https://docs.groupdocs.com/display/searchnet/Alias+dictionary)

### 也可以看看

* class [DictionaryBase](../dictionarybase)
* 命名空间 [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->