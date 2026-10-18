---
title: "TcpSettings"
second_title: "GroupDocs.Search for Java API Referansı"
description: "TCP ağ ayarlarını temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

TCP ağ ayarlarını temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | TcpSettings sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Dinleme bağlantı noktasını alır. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Gönderme zaman aşımını milisaniye cinsinden alır. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Alma zaman aşımını milisaniye cinsinden alır. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


TcpSettings sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | listeningPort | int | Dinleme bağlantı noktası. |
|
|  | sendTimeout | int | Milisaniye cinsinden gönderim zaman aşımı. |
|
|  | receiveTimeout | int | Milisaniye cinsinden alım zaman aşımı. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Dinleme bağlantı noktasını alır.


**Returns:**
int - Dinleme bağlantı noktası.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Gönderme zaman aşımını milisaniye cinsinden alır.


**Returns:**
int - Milisaniye cinsinden gönderim zaman aşımı.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Alma zaman aşımını milisaniye cinsinden alır.


**Returns:**
int - Milisaniye cinsinden alım zaman aşımı.

