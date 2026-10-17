---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络状态更改事件的参数。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

表示搜索网络状态更改事件的参数。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | 获取旧的搜索网络状态。 |
|
|  | [getNewStatus()](#getNewStatus--) | 获取新的搜索网络状态。 |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


获取旧的搜索网络状态。


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


获取新的搜索网络状态。


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

