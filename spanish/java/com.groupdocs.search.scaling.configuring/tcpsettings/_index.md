---
title: "TcpSettings"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa una configuración de red TCP."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Representa una configuración de red TCP.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Inicializa una nueva instancia de la clase TcpSettings. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Obtiene el puerto de escucha. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Obtiene el tiempo de espera de envío en milisegundos. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Obtiene el tiempo de espera de recepción en milisegundos. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Inicializa una nueva instancia de la clase TcpSettings.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | listeningPort | int | El puerto de escucha. |
|
|  | sendTimeout | int | El tiempo de espera de envío en milisegundos. |
|
|  | receiveTimeout | int | El tiempo de espera de recepción en milisegundos. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Obtiene el puerto de escucha.


**Returns:**
int - El puerto de escucha.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Obtiene el tiempo de espera de envío en milisegundos.


**Returns:**
int - El tiempo de espera de envío en milisegundos.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Obtiene el tiempo de espera de recepción en milisegundos.


**Returns:**
int - El tiempo de espera de recepción en milisegundos.

