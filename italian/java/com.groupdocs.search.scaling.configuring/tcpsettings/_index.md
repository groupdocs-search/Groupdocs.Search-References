---
title: "TcpSettings"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta le impostazioni di rete TCP."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Rappresenta le impostazioni di rete TCP.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Inizializza una nuova istanza della  TcpSettings  classe. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Restituisce la porta di ascolto. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Restituisce il timeout di invio in millisecondi. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Restituisce il timeout di ricezione in millisecondi. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Inizializza una nuova istanza della  TcpSettings  classe.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | listeningPort | int | La porta di ascolto. |
|
|  | sendTimeout | int | Il timeout di invio in millisecondi. |
|
|  | receiveTimeout | int | Il timeout di ricezione in millisecondi. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Restituisce la porta di ascolto.


**Returns:**
int - La porta di ascolto.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Restituisce il timeout di invio in millisecondi.


**Returns:**
int - Il timeout di invio in millisecondi.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Restituisce il timeout di ricezione in millisecondi.


**Returns:**
int - Il timeout di ricezione in millisecondi.

