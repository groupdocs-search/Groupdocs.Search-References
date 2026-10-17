---
title: "TcpSettings"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل إعدادات شبكة TCP."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

يمثل إعدادات شبكة TCP.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | يُنشئ مثيلًا جديدًا من الفئة TcpSettings. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | يحصل على منفذ الاستماع. |
|
|  | [getSendTimeout()](#getSendTimeout--) | يحصل على مهلة الإرسال بالميليثانية. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | يحصل على مهلة الاستلام بالميليثانية. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


يُنشئ مثيلًا جديدًا من الفئة TcpSettings.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | listeningPort | int | منفذ الاستماع. |
|
|  | sendTimeout | int | مهلة الإرسال بالمللي ثانية. |
|
|  | receiveTimeout | int | مهلة الاستلام بالمللي ثانية. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


يحصل على منفذ الاستماع.


**Returns:**
int - منفذ الاستماع.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


يحصل على مهلة الإرسال بالميليثانية.


**Returns:**
int - مهلة الإرسال بالمللي ثانية.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


يحصل على مهلة الاستلام بالميليثانية.


**Returns:**
int - مهلة الاستلام بالمللي ثانية.

