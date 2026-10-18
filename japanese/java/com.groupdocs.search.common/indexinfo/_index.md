---
title: "IndexInfo"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスに関する基本情報を含みます。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

インデックスに関する基本情報を含みます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | インデックスの一意識別子を取得します。 |
|
|  | [getIndexFolder()](#getIndexFolder--) | インデックスが配置されているフォルダーの完全な名前を取得します。 |
|
|  | [getIndexStatus()](#getIndexStatus--) | インデックスのステータスを取得します。 |
|
|  | [getVersion()](#getVersion--) | インデックスのバージョンを取得します。 |
|
|  | [getSegmentCount()](#getSegmentCount--) | インデックスセグメントの数を取得します。 |
|
|  | [getTermCount()](#getTermCount--) | インデックス内の単語数を取得します。 |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


インデックスの一意識別子を取得します。


**Returns:**
java.util.UUID - インデックスの一意識別子です。

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


インデックスが配置されているフォルダーの完全な名前を取得します。


**Returns:**
java.lang.String - インデックスが配置されているフォルダーの完全な名前です。

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


インデックスのステータスを取得します。


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


インデックスのバージョンを取得します。


**Returns:**
java.lang.String - インデックスのバージョンです。

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


インデックスセグメントの数を取得します。


**Returns:**
int - インデックスセグメントの数です。

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


インデックス内の単語数を取得します。


**Returns:**
int - インデックス内の単語数です。

