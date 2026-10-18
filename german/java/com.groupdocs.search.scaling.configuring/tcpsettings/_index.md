---
title: "TcpSettings"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt eine TCP-Netzwerkeinstellung dar."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Stellt eine TCP-Netzwerkeinstellung dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Initialisiert eine neue Instanz der  TcpSettings  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Liest den Listening-Port. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Liest den Sendetimeout in Millisekunden. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Liest den Empfangstimeout in Millisekunden. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Initialisiert eine neue Instanz der  TcpSettings  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | listeningPort | int | Der Listening-Port. |
|
|  | sendTimeout | int | Der Sendetimeout in Millisekunden. |
|
|  | receiveTimeout | int | Der Empfangstimeout in Millisekunden. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Liest den Listening-Port.


**Returns:**
int - Der Listening-Port.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Liest den Sendetimeout in Millisekunden.


**Returns:**
int - Der Sendetimeout in Millisekunden.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Liest den Empfangstimeout in Millisekunden.


**Returns:**
int - Der Empfangstimeout in Millisekunden.

