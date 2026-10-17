---
title: "MergeOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供合并操作的选项。"
type: docs
weight: 28
url: /zh/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

提供合并操作的选项。


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | 初始化 MergeOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isAsync()](#isAsync--) | 获取异步执行操作的标志。 |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 设置异步执行操作的标志。 |
|
|  | [getCancellation()](#getCancellation--) | 获取操作取消对象。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 设置操作取消对象。 |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


初始化 MergeOptions 类的新实例。


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


获取异步执行操作的标志。默认值为 false。


**Returns:**
boolean - 异步执行操作的标志。

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


设置异步执行操作的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 异步执行操作的标志。 |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


获取操作取消对象。默认值为 null。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


设置操作取消对象。默认值为 null。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 操作取消对象。 |
|

