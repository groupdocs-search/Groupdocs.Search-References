---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Metin parçalarında arama sonuçlarını vurgulayan bir arama sonucu vurgulayıcısını temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Metin parçalarında arama sonuçlarını vurgulayan bir arama sonucu vurgulayıcısını temsil eder.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// 'Einstein' kelimesini ara
SearchResult result = index.search("Einstein");
// Vurgulama seçeneklerini atama
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Bir belgenin metninde bulunan kelimeleri vurgulama
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Sonucu alıyor
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// HTML işaretlemesini konsola yazdırma
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | FragmentHighlighter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getResult()](#getResult--) | Sonuç fragment konteynerlerinin bir dizisini alır. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


FragmentHighlighter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Çıktı biçimi. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Sonuç fragment konteynerlerinin bir dizisini alır.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Sonuç fragment konteynerlerinin bir dizisi.

