---
title: "ImageLocation"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "画像の場所を指定します。"
type: docs
weight: 48
url: /ja/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

画像の場所を指定します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [Separate](#Separate) | 別ファイルの画像。 |
|
|  | [Embedded](#Embedded) | 別のドキュメントに埋め込まれた画像。 |
|
|  | [ContainerItem](#ContainerItem) | コンテナファイル内の要素である画像です。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


別ファイルの画像。


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


別のドキュメントに埋め込まれた画像。


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


コンテナファイル内の要素である画像です。


### values() {#values--}
```
public static ImageLocation[] values()
```




**Returns:**
com.groupdocs.search.options.ImageLocation[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ImageLocation valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
