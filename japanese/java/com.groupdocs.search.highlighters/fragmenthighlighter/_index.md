---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "テキストフラグメント内で検索結果をハイライトする検索結果ハイライターを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

テキストフラグメント内で検索結果をハイライトする検索結果ハイライターを表します。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// 'Einstein' の単語を検索
SearchResult result = index.search("Einstein");
// ハイライトオプションを割り当てる
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// 文書のテキスト内で見つかった単語をハイライト
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// 結果を取得
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// HTMLマークアップをコンソールに出力
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | FragmentHighlighter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getResult()](#getResult--) | 結果のフラグメント コンテナの配列を取得します。 |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


FragmentHighlighter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 出力フォーマットです。 |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


結果のフラグメント コンテナの配列を取得します。


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - 結果として得られるフラグメント コンテナの配列。

