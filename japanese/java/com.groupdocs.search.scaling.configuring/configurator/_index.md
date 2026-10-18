---
title: "Configurator"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワーク構成ツールを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

検索ネットワーク構成ツールを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Configurator()](#Configurator--) | 新しい Configurator クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | 検索ネットワーク内の各シャードのインデックス設定の構成を開始します。 |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | 検索ネットワーク構成にノードを追加します。 |
|
|  | [completeConfiguration()](#completeConfiguration--) | 構成プロセスを完了し、検索ネットワーク構成のインスタンスを返します。 |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


新しい Configurator クラスのインスタンスを初期化します。


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


検索ネットワーク内の各シャードのインデックス設定の構成を開始します。


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


検索ネットワーク構成にノードを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | nodeIndex | int | ノードインデックス。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


構成プロセスを完了し、検索ネットワーク構成のインスタンスを返します。


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
