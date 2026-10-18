---
title: "DataExtractedEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントのデータ抽出が完了したイベントの引数を表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

ドキュメントのデータ抽出が完了したイベントの引数を表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | 抽出器のインデックスを取得します。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | ドキュメントキーを取得します。 |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


抽出器のインデックスを取得します。


**Returns:**
int - 抽出器のインデックス。

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


ドキュメントキーを取得します。


**Returns:**
java.lang.String - ドキュメントキー。

