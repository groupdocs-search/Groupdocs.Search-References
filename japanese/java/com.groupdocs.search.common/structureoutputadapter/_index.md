---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "各フィールドを個別に含む構造体として出力を収集する出力アダプタを表します。"
type: docs
weight: 33
url: /ja/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

各フィールドを個別に含む構造体として出力を収集する出力アダプタを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StructureOutputAdapter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getResult()](#getResult--) | 結果として得られるフィールドの配列を取得します。 |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


StructureOutputAdapter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 出力フォーマットです。 |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


結果として得られるフィールドの配列を取得します。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 結果として得られるフィールドの配列。

