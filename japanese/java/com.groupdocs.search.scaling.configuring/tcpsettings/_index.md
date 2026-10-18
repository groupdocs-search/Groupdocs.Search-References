---
title: "TcpSettings"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "TCPネットワーク設定を表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

TCPネットワーク設定を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | 新しい TcpSettings クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | リスニングポートを取得します。 |
|
|  | [getSendTimeout()](#getSendTimeout--) | 送信タイムアウト（ミリ秒）を取得します。 |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | 受信タイムアウト（ミリ秒）を取得します。 |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


新しい TcpSettings クラスのインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | listeningPort | int | リスニングポート。 |
|
|  | sendTimeout | int | ミリ秒単位の送信タイムアウト。 |
|
|  | receiveTimeout | int | ミリ秒単位の受信タイムアウト。 |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


リスニングポートを取得します。


**Returns:**
int - リスニングポート。

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


送信タイムアウト（ミリ秒）を取得します。


**Returns:**
int - ミリ秒単位の送信タイムアウト。

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


受信タイムアウト（ミリ秒）を取得します。


**Returns:**
int - ミリ秒単位の受信タイムアウト。

