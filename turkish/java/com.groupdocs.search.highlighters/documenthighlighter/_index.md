---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Tüm belge metninde arama sonuçlarını vurgulayan bir arama sonucu vurgulayıcısını temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Tüm belge metninde arama sonuçlarını vurgulayan bir arama sonucu vurgulayıcısını temsil eder.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// 'Theory of Relativity' ifadesini ara
SearchResult result = index.search("\"Theory of Relativity\"");
// Bir belgenin metninde bulunan kelimeleri vurgulama
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | DocumentHighlighter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Yapıcıda geçirilen çıktı adaptörünü alır. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


DocumentHighlighter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Çıktı adaptörü, vurgulamanın sonucunu aktarır. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Yapıcıda geçirilen çıktı adaptörünü alır.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

