---
title: TcpSettings
second_title: GroupDocs.Search for Java API Reference
description: Represents a TCP network settings.
type: docs
weight: 13
url: /java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Represents a TCP network settings.
## Constructors

| Constructor | Description |
| --- | --- |
| [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Initializes a new instance of the  TcpSettings  class. |
## Methods

| Method | Description |
| --- | --- |
| [getListeningPort()](#getListeningPort--) | Gets the listening port. |
| [getSendTimeout()](#getSendTimeout--) | Gets the send timeout in milliseconds. |
| [getReceiveTimeout()](#getReceiveTimeout--) | Gets the receive timeout in milliseconds. |
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Initializes a new instance of the  TcpSettings  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| listeningPort | int | The listening port. |
| sendTimeout | int | The send timeout in milliseconds. |
| receiveTimeout | int | The receive timeout in milliseconds. |

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Gets the listening port.

**Returns:**
int - The listening port.
### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Gets the send timeout in milliseconds.

**Returns:**
int - The send timeout in milliseconds.
### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Gets the receive timeout in milliseconds.

**Returns:**
int - The receive timeout in milliseconds.
