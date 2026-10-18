---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "コンテナドキュメントから項目を抽出するメソッドを提供します。"
type: docs
weight: 35
url: /ja/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

コンテナドキュメントから項目を抽出するメソッドを提供します。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | ドキュメント形式ファミリを取得します。 |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | コンテナドキュメントから項目を抽出します。 |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | コンテナドキュメントから項目を抽出します。 |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


ドキュメント形式ファミリを取得します。


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


コンテナドキュメントから項目を抽出します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルパス。 |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - 抽出された項目の配列です。

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


コンテナドキュメントから項目を抽出します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | stream | java.io.InputStream | ドキュメントストリームです。 |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - 抽出された項目の配列です。

