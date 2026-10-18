---
title: "EventHandler"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "イベントハンドラのインターフェイスを定義します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.search.events/eventhandler/
---```
public interface EventHandler<T>
```

Defines interface of an event handler.

## Methods

| Method | Description |
| --- | --- |
| [invoke(Object sender, T args)](#invoke-java.lang.Object-T-) | Starts handling of the event.
 |
### invoke(Object sender, T args) {#invoke-java.lang.Object-T-}
```
public abstract void invoke(Object sender, T args)
```


Starts handling of the event.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The sender of the event.
 |
| args | T | Arguments of the event.
 |

