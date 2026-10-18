---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "イベント引数の基底クラスを表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

イベント引数の基底クラスを表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTime()](#getTime--) | イベントの時間を取得します。 |
|
|  | [getIndexId()](#getIndexId--) | インデックスIDを取得します。 |
|
|  | [getIndexFolder()](#getIndexFolder--) | インデックスフォルダーを取得します。 |
|
|  | [getStatus()](#getStatus--) | インデックスのステータスを取得します。 |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


イベントの時間を取得します。


**Returns:**
java.util.Date - イベントの時間。

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


インデックスIDを取得します。


**Returns:**
java.util.UUID - インデックスID。

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


インデックスフォルダーを取得します。


**Returns:**
java.lang.String - インデックスフォルダー。

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


インデックスのステータスを取得します。


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

