---
title: "NodeConfigurator"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワークノード構成ツールを表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

検索ネットワークノード構成ツールを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | TCPエンドポイントを設定します。 |
|
|  | [addLogSink()](#addLogSink--) | 検索ネットワークノードにログシンクを追加します。 |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | 検索ネットワークノードに検索サービスを追加します。 |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | 検索ネットワークノードにインデクサーサービスを追加します。 |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | 検索ネットワークノードにエクストラクターサービスを追加します。 |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | 検索ネットワークノードにシャードサービスを追加します。 |
|
|  | [completeNode()](#completeNode--) | 検索ネットワークノードの構成を完了します。 |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


TCPエンドポイントを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | ホスト名またはアドレス。 |
|
|  | ポート | int | ポート番号。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


検索ネットワークノードにログシンクを追加します。


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


検索ネットワークノードに検索サービスを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 追加サービスのストレージパス。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


検索ネットワークノードにインデクサーサービスを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 追加サービスのストレージパス。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


検索ネットワークノードにエクストラクターサービスを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 追加サービスのストレージパス。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


検索ネットワークノードにシャードサービスを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 追加サービスのストレージパス。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


検索ネットワークノードの構成を完了します。


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

