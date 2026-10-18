---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "文書全体のテキスト内で検索結果をハイライトする検索結果ハイライターを表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

文書全体のテキスト内で検索結果をハイライトする検索結果ハイライターを表します。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// 'Theory of Relativity' のフレーズを検索
SearchResult result = index.search("\"Theory of Relativity\"");
// 文書のテキスト内で見つかった単語をハイライト
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | DocumentHighlighter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | コンストラクタで渡された出力アダプタを取得します。 |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


DocumentHighlighter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | ハイライト結果を転送する出力アダプタです。 |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


コンストラクタで渡された出力アダプタを取得します。


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

