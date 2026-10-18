---
title: "構成"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワーク構成を表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

検索ネットワーク構成を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | この構成をファイルに保存します。 |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | この構成をストリームに保存します。 |
|
|  | [load(String filePath)](#load-java.lang.String-) | ファイルから検索ネットワーク構成を読み込みます。 |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | ストリームから検索ネットワーク構成を読み込みます。 |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


この構成をファイルに保存します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | 保存先のファイル。 |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


この構成をストリームに保存します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | stream | java.io.OutputStream | 保存先のストリーム。 |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


ファイルから検索ネットワーク構成を読み込みます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | 読み込み元のファイル。 |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


ストリームから検索ネットワーク構成を読み込みます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 読み込み元のストリーム。 |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

