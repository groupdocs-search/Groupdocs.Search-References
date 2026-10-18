---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "カスタム抽出器のコレクションを含みます。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

カスタム抽出器のコレクションを含みます。コレクションに組み込み抽出器がカバーするファイル拡張子用の抽出器が含まれている場合、その抽出器は組み込みのものの代わりに使用されます。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [size()](#size--) | コレクションに含まれる抽出器の数を取得します。 |
|
|  | [isReadOnly()](#isReadOnly--) | コレクションが読み取り専用かどうかを示す値を取得します。 |
|
|  | [iterator()](#iterator--) | このコレクションのイテレータを返します。 |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | 抽出器をコレクションに追加します。 |
|
|  | [clear()](#clear--) | コレクションからすべての抽出器を削除します。 |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | コレクションが特定の抽出器を含むかどうかを判断します。 |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | コレクションの要素を特定の配列インデックスから開始して配列にコピーします。 |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | コレクションから抽出器を削除します。 |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


コレクションに含まれる抽出器の数を取得します。


**Returns:**
int - コレクションに含まれる抽出器の数です。

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


コレクションが読み取り専用かどうかを示す値を取得します。


**Returns:**
boolean - コレクションが読み取り専用かどうかを示す値です。

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


このコレクションのイテレータを返します。


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - コレクションを反復処理するために使用できるイテレータオブジェクトです。

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


抽出器をコレクションに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | コレクションに追加する抽出器です。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


コレクションからすべての抽出器を削除します。


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


コレクションが特定の抽出器を含むかどうかを判断します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | コレクション内で位置付ける抽出器。 |
|

**Returns:**
boolean - アイテムがコレクション内に見つかった場合は true、そうでない場合は false。

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


コレクションの要素を特定の配列インデックスから開始して配列にコピーします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | コレクションからコピーされた要素の宛先となる一次元配列。配列はゼロベースインデックスである必要があります。 |
|
|  | arrayIndex | int | コピーが開始される配列内のゼロベースインデックス。 |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


コレクションから抽出器を削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | コレクションから削除する抽出器。 |
|

**Returns:**
boolean - 抽出器がコレクションから正常に削除された場合は true、そうでない場合は false。このメソッドは、抽出器が元のコレクションに見つからない場合も false を返します。

