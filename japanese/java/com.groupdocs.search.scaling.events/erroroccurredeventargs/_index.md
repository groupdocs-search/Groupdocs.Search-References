---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワークのノードの一つでエラーが発生したイベントの引数を表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

検索ネットワークのノードの一つでエラーが発生したイベントの引数を表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 検索ネットワークノードのインデックスを取得します。 |
|
|  | [getServiceIndex()](#getServiceIndex--) | 検索ネットワークノードサービスのインデックスを取得します。 |
|
|  | [getMessage()](#getMessage--) | エラーメッセージを取得します。 |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


検索ネットワークノードのインデックスを取得します。


**Returns:**
int - 検索ネットワークノードのインデックス。

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


検索ネットワークノードサービスのインデックスを取得します。


**Returns:**
int - 検索ネットワークノードサービスのインデックス。

### getMessage() {#getMessage--}
```
public final String getMessage()
```


エラーメッセージを取得します。


**Returns:**
java.lang.String - エラーメッセージ。

