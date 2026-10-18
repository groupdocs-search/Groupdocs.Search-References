---
title: "SearchNetworkNode"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili node jaringan pencarian yang dapat berisi layanan seperti extractor indexer searcher shard."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Mewakili node jaringan pencarian yang dapat berisi layanan seperti extractor, indexer, searcher, shard.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Menginisialisasi instance baru dari kelas  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Menginisialisasi instance baru dari kelas  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Menginisialisasi instance baru dari kelas  SearchNetworkNode . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [start()](#start--) | Memulai fungsi node jaringan pencarian. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Mengonfigurasi semua node dalam jaringan pencarian. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Mengonfigurasi node yang ditentukan dalam jaringan pencarian. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Mendapatkan koleksi ekstraktor khusus. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Mengatur konektor OCR yang digunakan untuk pemrosesan OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Mengatur penyedia bentuk kata. |
|
|  | [close()](#close--) | Melepaskan semua sumber daya yang digunakan oleh SearchNetworkNode. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Mendapatkan indeks node jaringan pencarian. |
|
|  | [getEvents()](#getEvents--) | Mendapatkan hub acara untuk berlangganan ke acara. |
|
|  | [getIndexer()](#getIndexer--) | Mendapatkan pengindeks. |
|
|  | [getSearcher()](#getSearcher--) | Mendapatkan pencari. |
|
|  | [getShardIndices()](#getShardIndices--) | Mendapatkan array semua indeks shard dalam jaringan pencarian. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Mendapatkan indeks node tempat layanan berada. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Menginisialisasi instance baru dari kelas  SearchNetworkNode .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nodeIndex | int | Indeks node. |
|
|  | storagePath | java.lang.String | Jalur penyimpanan. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Pengaturan jaringan. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Menginisialisasi instance baru dari kelas  SearchNetworkNode .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nodeIndex | int | Indeks node. |
|
|  | storagePath | java.lang.String | Jalur penyimpanan. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Pengaturan jaringan. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Logger. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Menginisialisasi instance baru dari kelas  SearchNetworkNode .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nodeIndex | int | Indeks node. |
|
|  | storagePath | java.lang.String | Jalur penyimpanan. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Pengaturan jaringan. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Logger. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | Konfigurasi. |
|

### start() {#start--}
```
public void start()
```


Memulai fungsi node jaringan pencarian.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Mengonfigurasi semua node dalam jaringan pencarian.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Mengonfigurasi node yang ditentukan dalam jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nodeIndex | int | Indeks node. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Mendapatkan koleksi ekstraktor kustom. Contoh lengkap implementasi ekstraktor kustom disajikan dalam dokumentasi untuk antarmuka GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Mengatur konektor OCR yang digunakan untuk pemrosesan OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Konektor OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Mengatur penyedia bentuk kata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Penyedia bentuk kata. |
|

### close() {#close--}
```
public void close()
```


Melepaskan semua sumber daya yang digunakan oleh SearchNetworkNode.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Mendapatkan indeks node jaringan pencarian.


**Returns:**
int - Indeks node jaringan pencarian.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Mendapatkan hub acara untuk berlangganan ke acara.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Mendapatkan pengindeks.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Mendapatkan pencari.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Mendapatkan array semua indeks shard dalam jaringan pencarian.


**Returns:**
int[] - Sebuah array semua indeks shard dalam jaringan pencarian.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Mendapatkan indeks node tempat layanan berada.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | serviceIndex | int | Indeks layanan. |
|

**Returns:**
int - Indeks node tempat layanan berada. Jika indeks layanan tidak benar, maka -1 dikembalikan.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
