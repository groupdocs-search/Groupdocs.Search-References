---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "抽出器、インデクサ、検索者、シャードなどのサービスを含むことができる検索ネットワークノードを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

抽出器、インデクサ、検索者、シャードなどのサービスを含むことができる検索ネットワークノードを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | SearchNetworkNode クラスの新しいインスタンスを初期化します。 |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | SearchNetworkNode クラスの新しいインスタンスを初期化します。 |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | SearchNetworkNode クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [start()](#start--) | 検索ネットワークノードの動作を開始します。 |
|
|  | [configureAllNodes()](#configureAllNodes--) | 検索ネットワーク内のすべてのノードを構成します。 |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | 検索ネットワーク内の指定されたノードを構成します。 |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | カスタム抽出器コレクションを取得します。 |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | OCR 処理に使用される OCR コネクタを設定します。 |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | 単語形態プロバイダーを設定します。 |
|
|  | [close()](#close--) | SearchNetworkNode が使用するすべてのリソースを解放します。 |
|
|  | [getNodeIndex()](#getNodeIndex--) | 検索ネットワークノードのインデックスを取得します。 |
|
|  | [getEvents()](#getEvents--) | イベントの購読用ハブを取得します。 |
|
|  | [getIndexer()](#getIndexer--) | インデクサを取得します。 |
|
|  | [getSearcher()](#getSearcher--) | 検索者を取得します。 |
|
|  | [getShardIndices()](#getShardIndices--) | 検索ネットワーク内のすべてのシャードインデックスの配列を取得します。 |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | サービスが配置されているノードのインデックスを取得します。 |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


SearchNetworkNode クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | nodeIndex | int | ノードインデックス。 |
|
|  | storagePath | java.lang.String | ストレージパス。 |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | ネットワーク設定。 |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


SearchNetworkNode クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | nodeIndex | int | ノードインデックス。 |
|
|  | storagePath | java.lang.String | ストレージパス。 |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | ネットワーク設定。 |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | ロガー。 |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


SearchNetworkNode クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | nodeIndex | int | ノードインデックス。 |
|
|  | storagePath | java.lang.String | ストレージパス。 |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | ネットワーク設定。 |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | ロガー。 |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | 構成。 |
|

### start() {#start--}
```
public void start()
```


検索ネットワークノードの動作を開始します。


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


検索ネットワーク内のすべてのノードを構成します。


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


検索ネットワーク内の指定されたノードを構成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | nodeIndex | int | ノードインデックス。 |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


カスタムエクストラクタコレクションを取得します。 カスタムエクストラクタの実装例は  GroupDocs.Search.Common.IFieldExtractor  インターフェイスのドキュメントに示されています。


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


OCR 処理に使用される OCR コネクタを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCRコネクタ。 |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


単語形態プロバイダーを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | 単語形態プロバイダー。 |
|

### close() {#close--}
```
public void close()
```


SearchNetworkNode が使用するすべてのリソースを解放します。


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


検索ネットワークノードのインデックスを取得します。


**Returns:**
int - 検索ネットワークノードのインデックス。

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


イベントの購読用ハブを取得します。


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


インデクサを取得します。


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


検索者を取得します。


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


検索ネットワーク内のすべてのシャードインデックスの配列を取得します。


**Returns:**
int[] - 検索ネットワーク内のすべてのシャードインデックスの配列。

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


サービスが配置されているノードのインデックスを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | serviceIndex | int | サービスインデックス。 |
|

**Returns:**
int - サービスが配置されているノードのインデックス。サービスインデックスが正しくない場合、-1 が返されます。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
