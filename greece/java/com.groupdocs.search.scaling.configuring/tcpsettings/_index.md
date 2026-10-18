---
title: "TcpSettings"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά ρυθμίσεις δικτύου TCP."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

Αναπαριστά ρυθμίσεις δικτύου TCP.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης  TcpSettings . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | Λαμβάνει τη θύρα ακρόασης. |
|
|  | [getSendTimeout()](#getSendTimeout--) | Λαμβάνει το χρονικό όριο αποστολής σε χιλιοστά του δευτερολέπτου. |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | Λαμβάνει το χρονικό όριο λήψης σε χιλιοστά του δευτερολέπτου. |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  TcpSettings .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | listeningPort | int | Η θύρα ακρόασης. |
|
|  | sendTimeout | int | Το χρονικό όριο αποστολής σε χιλιοστά του δευτερολέπτου. |
|
|  | receiveTimeout | int | Το χρονικό όριο λήψης σε χιλιοστά του δευτερολέπτου. |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


Λαμβάνει τη θύρα ακρόασης.


**Returns:**
int - Η θύρα ακρόασης.

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


Λαμβάνει το χρονικό όριο αποστολής σε χιλιοστά του δευτερολέπτου.


**Returns:**
int - Το χρονικό όριο αποστολής σε χιλιοστά του δευτερολέπτου.

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


Λαμβάνει το χρονικό όριο λήψης σε χιλιοστά του δευτερολέπτου.


**Returns:**
int - Το χρονικό όριο λήψης σε χιλιοστά του δευτερολέπτου.

