---
title: "DocumentDeletedEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントの削除が完了したイベントの引数を表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

ドキュメントの削除が完了したイベントの引数を表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | シャードインデックスを取得します。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | ドキュメントキーを取得します。 |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


シャードインデックスを取得します。


**Returns:**
int - シャードインデックス。

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


ドキュメントキーを取得します。


**Returns:**
java.lang.String - ドキュメントキー。

