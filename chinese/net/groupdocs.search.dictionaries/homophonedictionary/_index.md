---
title: HomophoneDictionary
second_title: GroupDocs.Search for .NET API 参考
description: 表示异形同音字字典
type: docs
weight: 430
url: /zh/net/groupdocs.search.dictionaries/homophonedictionary/
---
## HomophoneDictionary class

表示异形同音字字典。

```csharp
public class HomophoneDictionary : DictionaryBase, IEnumerable<string>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/homophonedictionary/count) { get; } | 获取此包含的单词数[`HomophoneDictionary`](../homophonedictionary). |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | 将指定的同音字组集合添加到[`HomophoneDictionary`](../homophonedictionary). |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange_1)(string[][]) | 将指定的同音字组集合添加到[`HomophoneDictionary`](../homophonedictionary). |
| [Clear](../../groupdocs.search.dictionaries/homophonedictionary/clear)() | 删除所有单词[`HomophoneDictionary`](../homophonedictionary)对象. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | 将字典导出到具有指定名称的文件。 |
| [GetAllHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/getallhomophonegroups)() | 获取该词典中包含的所有同音字组。 |
| [GetEnumerator](../../groupdocs.search.dictionaries/homophonedictionary/getenumerator)() | 返回一个遍历集合的枚举器。 |
| [GetHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/gethomophonegroups)(string) | 获取指定单词所属的所有同音词组 |
| [GetHomophones](../../groupdocs.search.dictionaries/homophonedictionary/gethomophones)(string) | 获取指定单词的同音字。 结果数组不包含原始单词。 |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | 从指定文件导入字典。 |

### 评论

**学到更多**

* [同音字搜索](https://docs.groupdocs.com/display/searchnet/Homophone+search)
* [管理同音字词典](https://docs.groupdocs.com/display/searchnet/Homophone+dictionary)

### 也可以看看

* class [DictionaryBase](../dictionarybase)
* 命名空间 [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
