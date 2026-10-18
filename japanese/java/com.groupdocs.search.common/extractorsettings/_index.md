---
title: "ExtractorSettings"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントデータ抽出器の設定を含みます。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

ドキュメントデータ抽出器の設定を含みます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | 抽出器が使用されるインデックスタイプを取得します。 |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | 抽出器が使用されるインデックスタイプを設定します。 |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


抽出器が使用されるインデックスタイプを取得します。デフォルト値は GroupDocs.Search.Options.IndexType.NormalIndex です。


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


抽出器が使用されるインデックスタイプを設定します。デフォルト値は GroupDocs.Search.Options.IndexType.NormalIndex です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | 抽出器が使用されるインデックスタイプ。 |
|

