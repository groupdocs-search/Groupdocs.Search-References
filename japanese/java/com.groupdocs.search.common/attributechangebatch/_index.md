---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "属性変更のコンテナを表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

属性変更のコンテナを表します。


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | AttributeChangeBatch クラスの新しいインスタンスを初期化します。 |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | AttributeChangeBatch クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | 指定された属性を指定されたインデックス済みドキュメントに追加します。 |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | 指定された属性を指定されたインデックス済みドキュメント群に追加します。 |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | 指定された属性をインデックス内のすべてのドキュメントに追加します。 |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | 指定された属性を指定されたインデックス済みドキュメントから削除します。 |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | 指定された属性を指定されたインデックス済みドキュメント群から削除します。 |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | 指定されたインデックス済みドキュメントからすべての属性を削除します。 |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | 指定されたインデックス化されたドキュメントからすべての属性を削除します。 |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | インデックス内のすべてのドキュメントから指定された属性を削除します。 |
|
|  | [clear()](#clear--) | インデックス内のすべてのドキュメントからすべての属性を削除します。 |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


AttributeChangeBatch クラスの新しいインスタンスを初期化します。


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


AttributeChangeBatch クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


指定された属性を指定されたインデックス済みドキュメントに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | ドキュメントのパス。 |
|
|  | 属性 | java.lang.String[] | 追加する属性。 |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


指定された属性を指定されたインデックス済みドキュメント群に追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パス | java.lang.String[] | ドキュメントのパス。 |
|
|  | 属性 | java.lang.String[] | 追加する属性。 |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


指定された属性をインデックス内のすべてのドキュメントに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 属性 | java.lang.String[] | 追加する属性。 |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


指定された属性を指定されたインデックス済みドキュメントから削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | ドキュメントのパス。 |
|
|  | 属性 | java.lang.String[] | 削除する属性。 |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


指定された属性を指定されたインデックス済みドキュメント群から削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パス | java.lang.String[] | ドキュメントのパス。 |
|
|  | 属性 | java.lang.String[] | 削除する属性。 |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


指定されたインデックス済みドキュメントからすべての属性を削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | ドキュメントのパス。 |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


指定されたインデックス化されたドキュメントからすべての属性を削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パス | java.lang.String[] | ドキュメントのパス。 |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


インデックス内のすべてのドキュメントから指定された属性を削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 属性 | java.lang.String[] | 削除する属性。 |
|

### clear() {#clear--}
```
public void clear()
```


インデックス内のすべてのドキュメントからすべての属性を削除します。


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
