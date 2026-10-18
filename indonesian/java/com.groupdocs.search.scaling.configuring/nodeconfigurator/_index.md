---
title: "NodeConfigurator"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili konfigurator node jaringan pencarian."
type: docs
weight: 13
url: /id/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Mewakili konfigurator node jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Mengatur endpoint TCP. |
|
|  | [addLogSink()](#addLogSink--) | Menambahkan log sink ke node jaringan pencarian. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Menambahkan layanan pencari ke node jaringan pencarian. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Menambahkan layanan pengindeks ke node jaringan pencarian. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Menambahkan layanan pengekstrak ke node jaringan pencarian. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Menambahkan layanan shard ke node jaringan pencarian. |
|
|  | [completeNode()](#completeNode--) | Menyelesaikan konfigurasi node jaringan pencarian. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Mengatur endpoint TCP.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Nama host atau alamat. |
|
|  | port | int | Nomor port. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Menambahkan log sink ke node jaringan pencarian.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Menambahkan layanan pencari ke node jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | storagePath | java.lang.String | Jalur penyimpanan layanan penambahan. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Menambahkan layanan pengindeks ke node jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | storagePath | java.lang.String | Jalur penyimpanan layanan penambahan. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Menambahkan layanan pengekstrak ke node jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | storagePath | java.lang.String | Jalur penyimpanan layanan penambahan. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Menambahkan layanan shard ke node jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | storagePath | java.lang.String | Jalur penyimpanan layanan penambahan. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Menyelesaikan konfigurasi node jaringan pencarian.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

