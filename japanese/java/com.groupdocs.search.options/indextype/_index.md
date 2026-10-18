---
title: "IndexType"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスタイプを指定します。"
type: docs
weight: 49
url: /ja/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

インデックスタイプを指定します。


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | 説明 |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | すべての検索機能をサポートする、ドキュメントのメタデータとコンテンツを含む通常のインデックス。 |
|
|  | [MetadataIndex](#MetadataIndex) | コンテンツを含まず、ドキュメントのメタデータのみを含むインデックス。 |
|
|  | [CompactIndex](#CompactIndex) | ディスク容量を大幅に節約しますが、フレーズ検索や日付範囲検索機能はサポートしないインデックスタイプ。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


すべての検索機能をサポートする、ドキュメントのメタデータとコンテンツを含む通常のインデックス。


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


コンテンツを含まず、ドキュメントのメタデータのみを含むインデックス。


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


ディスク容量を大幅に節約しますが、フレーズ検索や日付範囲検索機能はサポートしないインデックスタイプ。


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
