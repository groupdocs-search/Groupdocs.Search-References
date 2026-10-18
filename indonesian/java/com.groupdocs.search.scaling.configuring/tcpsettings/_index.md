---
title: "TcpSettings"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili pengaturan jaringan TCP."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Mewakili pengaturan jaringan TCP.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Menginisialisasi sebuah instance baru dari kelas TcpSettings. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Mendapatkan port pendengaran. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Mendapatkan batas waktu pengiriman dalam milidetik. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Mendapatkan batas waktu penerimaan dalam milidetik. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Menginisialisasi sebuah instance baru dari kelas TcpSettings.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | listeningPort | int | Port pendengaran. |
|
|  | sendTimeout | int | Batas waktu pengiriman dalam milidetik. |
|
|  | receiveTimeout | int | Batas waktu penerimaan dalam milidetik. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Mendapatkan port pendengaran.


**Returns:**
int - Port pendengaran.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Mendapatkan batas waktu pengiriman dalam milidetik.


**Returns:**
int - Batas waktu pengiriman dalam milidetik.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Mendapatkan batas waktu penerimaan dalam milidetik.


**Returns:**
int - Batas waktu penerimaan dalam milidetik.

