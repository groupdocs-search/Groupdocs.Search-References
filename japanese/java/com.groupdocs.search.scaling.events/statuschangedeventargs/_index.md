---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワークのステータス変更イベントの引数を表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

検索ネットワークのステータス変更イベントの引数を表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | 古い検索ネットワークステータスを取得します。 |
|
|  | [getNewStatus()](#getNewStatus--) | 新しい検索ネットワークステータスを取得します。 |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


古い検索ネットワークステータスを取得します。


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


新しい検索ネットワークステータスを取得します。


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

