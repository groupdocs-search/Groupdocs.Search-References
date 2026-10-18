---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成操作が完了したイベントの引数を表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

インデックス作成操作が完了したイベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getMessage()](#getMessage--) | メッセージを取得します。 |
|
|  | [getOperationType()](#getOperationType--) | 操作タイプを取得します。 |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


メッセージを取得します。


**Returns:**
java.lang.String - メッセージ。

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


操作タイプを取得します。


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

