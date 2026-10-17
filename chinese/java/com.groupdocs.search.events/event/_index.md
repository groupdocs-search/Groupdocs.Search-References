---
title: "事件"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "此类旨在在订阅事件时被继承。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

此类旨在在订阅事件时被继承。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Event()](#Event--) | 初始化 Event 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [add(T delegate)](#add-T-) | 为事件添加监听器。 |
|
|  | [remove(T delegate)](#remove-T-) | 为事件移除监听器。 |
|
|  | [isEmpty()](#isEmpty--) | 检查是否至少存在一个监听器。 |
|
### Event() {#Event--}
```
public Event()
```


初始化 Event 类的新实例。


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


为事件添加监听器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 委托 | T | 要添加的事件监听器。 |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


为事件移除监听器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 委托 | T | 要移除的事件监听器。 |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


检查是否至少存在一个监听器。


**Returns:**
boolean - 一个指示已为该事件添加至少一个监听器的值。

