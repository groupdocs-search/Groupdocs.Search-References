---
title: "TcpSettings"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示 TCP 网络设置。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

表示 TCP 网络设置。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | 初始化 TcpSettings 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | 获取监听端口。 |
|
|  | [getSendTimeout()](#getSendTimeout--) | 获取以毫秒为单位的发送超时。 |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | 获取以毫秒为单位的接收超时。 |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


初始化 TcpSettings 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | listeningPort | int | 监听端口。 |
|
|  | sendTimeout | int | 发送超时（毫秒）。 |
|
|  | receiveTimeout | int | 接收超时（毫秒）。 |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


获取监听端口。


**Returns:**
int - 监听端口。

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


获取以毫秒为单位的发送超时。


**Returns:**
int - 发送超时（毫秒）。

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


获取以毫秒为单位的接收超时。


**Returns:**
int - 接收超时（毫秒）。

