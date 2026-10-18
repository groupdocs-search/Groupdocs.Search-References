---
title: "StreamOutputAdapter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili adaptor output yang mengumpulkan output ke dalam java.io.OutputStream."
type: docs
weight: 31
url: /id/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Mewakili adaptor output yang mengumpulkan output ke dalam java.io.OutputStream.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
DocumentInfo[] documents = index.getIndexedDocuments(); // Mendapatkan informasi tentang dokumen yang diindeks
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Membuat aliran output
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Membuat adaptor output aliran
index.getDocumentText(documents[0], adapter); // Menghasilkan teks dokumen ke dalam aliran
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Menginisialisasi instance baru dari kelas  StreamOutputAdapter . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getStream()](#getStream--) | Mendapatkan aliran output. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Menginisialisasi instance baru dari kelas  StreamOutputAdapter .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Format output. |
|
|  | stream | java.io.OutputStream | Aliran output. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Mendapatkan aliran output.


**Returns:**
java.io.OutputStream - Aliran output.

