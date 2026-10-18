---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスエラーが発生したイベントの引数を表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

インデックスエラーが発生したイベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getMessage()](#getMessage--) | エラーメッセージを取得します。 |
|
|  | [isCritical()](#isCritical--) | エラーが重大でインデックスを再起動すべきかを示すフラグを取得します。 |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


エラーメッセージを取得します。


**Returns:**
java.lang.String - エラーメッセージ。

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


エラーが重大でインデックスを再起動すべきかを示すフラグを取得します。


**Returns:**
boolean - エラーが重大でインデックスを再起動すべきかを示すフラグ。

