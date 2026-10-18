---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスメタデータフィールドのオプションを提供します。"
type: docs
weight: 29
url: /ja/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

インデックスメタデータフィールドのオプションを提供します。


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | 空のフィールド値をインデックスに含めるかどうかを示す値を取得します。 |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | 空のフィールド値をインデックスに含めるかどうかを示す値を設定します。 |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | 空のフィールド名をインデックスするかどうかを示す値を取得します。 |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | 空のフィールド名をインデックスするかどうかを示す値を設定します。 |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | 空のフィールド名をインデックスするために使用されるデフォルトのフィールド名を取得します。 |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | 空のフィールド名をインデックスするために使用されるデフォルトのフィールド名を設定します。 |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | フィールドの複合名における区切り文字を取得します。 |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | フィールドの複合名における区切り文字を設定します。 |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | フィールドをインデックスするための byte 型配列の最大値数を取得します。 |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | フィールドをインデックスするための byte 型配列の最大値数を設定します。 |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | フィールドをインデックスするための int 型配列の最大値数を取得します。 |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | フィールドをインデックスするための int 型配列の最大値数を設定します。 |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | フィールドをインデックスするための long 型配列の最大値数を取得します。 |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | フィールドをインデックスするための long 型配列の最大値数を設定します。 |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | フィールドをインデックスするための double 型配列の最大値数を取得します。 |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | フィールドをインデックスするための double 型配列の最大値数を設定します。 |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | 配列型フィールド内の値間の区切り文字を取得します。 |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | 配列型フィールド内の値間の区切り文字を設定します。 |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


空のフィールド値をインデックスするかどうかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean - 空のフィールド値をインデックスするかどうかを示す値です。

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


空のフィールド値をインデックスするかどうかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 空のフィールド値をインデックスするかどうかを示す値です。 |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


空のフィールド名をインデックスするかどうかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean - 空のフィールド名をインデックスするかどうかを示す値です。

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


空のフィールド名をインデックスするかどうかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 空のフィールド名をインデックスするかどうかを示す値です。 |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


空のフィールド名をインデックスするために使用されるデフォルトのフィールド名を取得します。デフォルト値は \"unknown\" です。


**Returns:**
java.lang.String - 空のフィールド名をインデックス付けする際に使用されるデフォルトのフィールド名です。

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


空のフィールド名をインデックス付けする際に使用されるデフォルトのフィールド名を設定します。デフォルト値は "unknown" です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 空のフィールド名をインデックス付けする際に使用されるデフォルトのフィールド名です。 |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


フィールドの複合名に使用される区切り文字を取得します。デフォルト値は "." です。


**Returns:**
java.lang.String - フィールドの複合名に使用される区切り文字です。

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


フィールドの複合名に使用される区切り文字を設定します。デフォルト値は "." です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | フィールドの複合名に使用される区切り文字です。 |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


フィールドをインデックス付けするための byte 型配列の最大要素数を取得します。デフォルト値は Integer.MAX_VALUE です。


**Returns:**
int - フィールドをインデックス付けするための byte 型配列の最大要素数です。

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


フィールドをインデックス付けするための byte 型配列の最大要素数を設定します。デフォルト値は Integer.MAX_VALUE です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | フィールドをインデックス付けするための byte 型配列の最大要素数です。 |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


フィールドをインデックス付けするための int 型配列の最大要素数を取得します。デフォルト値は Integer.MAX_VALUE です。


**Returns:**
int - フィールドをインデックス付けするための int 型配列の最大要素数です。

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


フィールドをインデックス付けするための int 型配列の最大要素数を設定します。デフォルト値は Integer.MAX_VALUE です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | フィールドをインデックス付けするための int 型配列の最大要素数です。 |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


フィールドをインデックス付けするための long 型配列の最大要素数を取得します。デフォルト値は Integer.MAX_VALUE です。


**Returns:**
int - フィールドをインデックス付けするための long 型配列の最大要素数です。

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


フィールドをインデックス付けするための long 型配列の最大要素数を設定します。デフォルト値は Integer.MAX_VALUE です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | フィールドをインデックス付けするための long 型配列の最大要素数です。 |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


フィールドをインデックス付けするための double 型配列の最大要素数を取得します。デフォルト値は Integer.MAX_VALUE です。


**Returns:**
int - フィールドをインデックス付けするための double 型配列の最大要素数です。

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


フィールドをインデックス付けするための double 型配列の最大要素数を設定します。デフォルト値は Integer.MAX_VALUE です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | フィールドをインデックス付けするための double 型配列の最大要素数です。 |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


配列型フィールドの値間の区切り文字を取得します。デフォルト値はスペースです。


**Returns:**
java.lang.String - 配列型フィールドの値間の区切り文字です。

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


配列型フィールドの値間の区切り文字を設定します。デフォルト値はスペースです。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 配列型フィールドの値間の区切り文字。 |
|

