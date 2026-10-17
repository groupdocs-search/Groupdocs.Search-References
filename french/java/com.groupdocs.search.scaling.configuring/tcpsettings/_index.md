---
title: "TcpSettings"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente des paramètres réseau TCP."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Représente des paramètres réseau TCP.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Initialise une nouvelle instance de la classe TcpSettings. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Obtient le port d'écoute. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Obtient le délai d'envoi en millisecondes. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Obtient le délai de réception en millisecondes. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Initialise une nouvelle instance de la classe TcpSettings.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | listeningPort | int | Le port d'écoute. |
|
|  | sendTimeout | int | Le délai d'envoi en millisecondes. |
|
|  | receiveTimeout | int | Le délai de réception en millisecondes. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Obtient le port d'écoute.


**Returns:**
int - Le port d'écoute.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Obtient le délai d'envoi en millisecondes.


**Returns:**
int - Le délai d'envoi en millisecondes.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Obtient le délai de réception en millisecondes.


**Returns:**
int - Le délai de réception en millisecondes.

