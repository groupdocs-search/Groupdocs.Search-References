---
title: "DocumentHighlighter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili penyorot hasil pencarian yang menyorot hasil pencarian dalam seluruh teks dokumen."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Mewakili penyorot hasil pencarian yang menyorot hasil pencarian dalam seluruh teks dokumen.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Cari fase 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Menyorot kata yang ditemukan dalam teks dokumen
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Menginisialisasi sebuah instance baru dari kelas DocumentHighlighter. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Mendapatkan output adapter yang diberikan dalam konstruktor. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Menginisialisasi sebuah instance baru dari kelas DocumentHighlighter.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Output adapter yang mentransfer hasil penyorotan. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Mendapatkan output adapter yang diberikan dalam konstruktor.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

