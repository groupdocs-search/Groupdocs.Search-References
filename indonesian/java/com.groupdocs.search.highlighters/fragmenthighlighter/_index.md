---
title: "FragmentHighlighter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili penyorot hasil pencarian yang menyorot hasil pencarian dalam fragmen teks."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Mewakili penyorot hasil pencarian yang menyorot hasil pencarian dalam fragmen teks.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Cari kata 'Einstein'
SearchResult result = index.search("Einstein");
// Menetapkan opsi sorotan
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Menyorot kata yang ditemukan dalam teks dokumen
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Mendapatkan hasil
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Mencetak markup HTML ke konsol
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Menginisialisasi sebuah instance baru dari kelas  FragmentHighlighter  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getResult()](#getResult--) | Mendapatkan sebuah array dari kontainer fragmen yang dihasilkan. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Menginisialisasi sebuah instance baru dari kelas  FragmentHighlighter  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Format output. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Mendapatkan sebuah array dari kontainer fragmen yang dihasilkan.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Sebuah array dari kontainer fragmen yang dihasilkan.

