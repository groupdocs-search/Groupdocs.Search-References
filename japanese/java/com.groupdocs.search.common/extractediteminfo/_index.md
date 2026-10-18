---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "コンテナ項目情報を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

コンテナ項目情報を表します。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | ExtractedItemInfo クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | ドキュメントのタイプを取得します。 |
|
|  | [getFields()](#getFields--) | 抽出されたフィールドを取得します。 |
|
|  | [getItemInfo()](#getItemInfo--) | アイテム情報を取得します。 |
|
|  | [getInnerPath()](#getInnerPath--) | 内部パスを取得します。 |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


ExtractedItemInfo クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | ドキュメント形式ファミリ。 |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 抽出されたフィールド。 |
|
|  | itemInfo | java.lang.String | アイテム情報。 |
|
|  | innerPath | java.lang.String | コンテナ内のアイテムへのパス。 |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


ドキュメントのタイプを取得します。


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


抽出されたフィールドを取得します。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 抽出されたフィールド。

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


アイテム情報を取得します。


**Returns:**
java.lang.String - アイテム情報。

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


内部パスを取得します。


**Returns:**
java.lang.String - 内部パス。

