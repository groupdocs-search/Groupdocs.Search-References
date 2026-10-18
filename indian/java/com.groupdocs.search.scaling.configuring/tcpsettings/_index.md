---
title: "TcpSettings"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक TCP नेटवर्क सेटिंग का प्रतिनिधित्व करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.scaling.configuring/tcpsettings/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.scaling.configuring.INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings)
```
public class TcpSettings implements INetworkSettings
```

एक TCP नेटवर्क सेटिंग का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)](#TcpSettings-int-int-int-) | एक नया उदाहरण प्रारंभ करता है TcpSettings वर्ग का। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getListeningPort()](#getListeningPort--) | सुनने वाला पोर्ट को प्राप्त करता है। |
|
|  | [getSendTimeout()](#getSendTimeout--) | भेजने का टाइमआउट मिलीसेकंड में प्राप्त करता है। |
|
|  | [getReceiveTimeout()](#getReceiveTimeout--) | प्राप्त करने का टाइमआउट मिलीसेकंड में प्राप्त करता है। |
|
### TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout) {#TcpSettings-int-int-int-}
```
public TcpSettings(int listeningPort, int sendTimeout, int receiveTimeout)
```


एक नया उदाहरण प्रारंभ करता है TcpSettings वर्ग का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | listeningPort | int | सुनने वाला पोर्ट। |
|
|  | sendTimeout | int | भेजने का टाइमआउट मिलीसेकंड में। |
|
|  | receiveTimeout | int | प्राप्त करने का टाइमआउट मिलीसेकंड में। |
|

### getListeningPort() {#getListeningPort--}
```
public final int getListeningPort()
```


सुनने वाला पोर्ट को प्राप्त करता है।


**Returns:**
int - सुनने वाला पोर्ट।

### getSendTimeout() {#getSendTimeout--}
```
public final int getSendTimeout()
```


भेजने का टाइमआउट मिलीसेकंड में प्राप्त करता है।


**Returns:**
int - भेजने का टाइमआउट मिलीसेकंड में।

### getReceiveTimeout() {#getReceiveTimeout--}
```
public final int getReceiveTimeout()
```


प्राप्त करने का टाइमआउट मिलीसेकंड में प्राप्त करता है।


**Returns:**
int - प्राप्त करने का टाइमआउट मिलीसेकंड में।

