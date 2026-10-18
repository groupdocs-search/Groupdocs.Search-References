---
title: "TcpSettings"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en TCP-nätverksinställning."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Representerar en TCP-nätverksinställning.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Initierar en ny instans av  TcpSettings  klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Hämtar lyssningsporten. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Hämtar sändningstimeout i millisekunder. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Hämtar mottagningstimeout i millisekunder. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Initierar en ny instans av  TcpSettings  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | listeningPort | int | Lyssningsporten. |
|
|  | sendTimeout | int | Sändningstimeout i millisekunder. |
|
|  | receiveTimeout | int | Mottagningstimeout i millisekunder. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Hämtar lyssningsporten.


**Returns:**
int - Lyssningsporten.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Hämtar sändningstimeout i millisekunder.


**Returns:**
int - Sändningstimeout i millisekunder.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Hämtar mottagningstimeout i millisekunder.


**Returns:**
int - Mottagningstimeout i millisekunder.

