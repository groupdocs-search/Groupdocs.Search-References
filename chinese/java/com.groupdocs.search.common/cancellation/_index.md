---
title: "取消"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示请求取消操作的对象。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

表示请求取消操作的对象。


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | 初始化一个新的实例 |
取消
类。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | 获取指示已请求取消的值。 |
|
|  | [cancel()](#cancel--) | 发出取消请求。 |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | 在指定毫秒数到期后发出取消请求。 |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


初始化一个新的实例
取消
类。


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


获取指示已请求取消的值。


**Returns:**
boolean - 表示已请求取消的值。

### cancel() {#cancel--}
```
public final void cancel()
```


发出取消请求。


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


在指定毫秒数到期后发出取消请求。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 毫秒 | int | 操作将在其后被取消的毫秒数。 |
|

