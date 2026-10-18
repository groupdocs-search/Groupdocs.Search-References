---
title: "TcpSettings"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "TCP 네트워크 설정을 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

TCP 네트워크 설정을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | TcpSettings 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | 수신 포트를 가져옵니다. |
|
|  | [getSendTimeout()](#getSendTimeout--) | 전송 제한 시간을 밀리초 단위로 가져옵니다. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | 수신 제한 시간을 밀리초 단위로 가져옵니다. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


TcpSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | listeningPort | int | 수신 포트. |
|
|  | sendTimeout | int | 밀리초 단위의 전송 제한 시간. |
|
|  | receiveTimeout | int | 밀리초 단위의 수신 제한 시간. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


수신 포트를 가져옵니다.


**Returns:**
int - 수신 포트.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


전송 제한 시간을 밀리초 단위로 가져옵니다.


**Returns:**
int - 밀리초 단위의 전송 제한 시간.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


수신 제한 시간을 밀리초 단위로 가져옵니다.


**Returns:**
int - 밀리초 단위의 수신 제한 시간.

