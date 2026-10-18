---
title: "TcpSettings"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет настройки TCP‑сети."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Представляет настройки TCP‑сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Инициализирует новый экземпляр класса  TcpSettings  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Получает порт прослушивания. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Получает тайм‑аут отправки в миллисекундах. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Получает тайм‑аут получения в миллисекундах. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Инициализирует новый экземпляр класса  TcpSettings  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | listeningPort | int | Порт прослушивания. |
|
|  | sendTimeout | int | Тайм‑аут отправки в миллисекундах. |
|
|  | receiveTimeout | int | Тайм‑аут получения в миллисекундах. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Получает порт прослушивания.


**Returns:**
int - Порт прослушивания.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Получает тайм‑аут отправки в миллисекундах.


**Returns:**
int - Тайм‑аут отправки в миллисекундах.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Получает тайм‑аут получения в миллисекундах.


**Returns:**
int - Тайм‑аут получения в миллисекундах.

