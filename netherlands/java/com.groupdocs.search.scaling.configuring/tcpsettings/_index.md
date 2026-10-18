---
title: "TcpSettings"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt TCP‑netwerkinstellingen voor."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Stelt TCP‑netwerkinstellingen voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Initialiseert een nieuw exemplaar van de  TcpSettings  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Haalt de luisterpoort op. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Haalt de verzendtijdslimiet op in milliseconden. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Haalt de ontvangsttijdslimiet op in milliseconden. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Initialiseert een nieuw exemplaar van de  TcpSettings  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | listeningPort | int | De luisterpoort. |
|
|  | sendTimeout | int | De verzendtijdslimiet in milliseconden. |
|
|  | receiveTimeout | int | De ontvangsttijdslimiet in milliseconden. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Haalt de luisterpoort op.


**Returns:**
int - De luisterpoort.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Haalt de verzendtijdslimiet op in milliseconden.


**Returns:**
int - De verzendtijdslimiet in milliseconden.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Haalt de ontvangsttijdslimiet op in milliseconden.


**Returns:**
int - De ontvangsttijdslimiet in milliseconden.

