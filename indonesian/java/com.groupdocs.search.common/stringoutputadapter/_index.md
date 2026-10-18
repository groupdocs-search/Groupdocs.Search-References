---
title: "StringOutputAdapter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili adaptor output yang mengumpulkan output sebagai System.String."
type: docs
weight: 32
url: /id/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Mewakili adaptor output yang mengumpulkan output sebagai System.String.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Membuat adaptor output string
index.getDocumentText(documents[0], adapter); // Menghasilkan teks dokumen ke adaptor
String result = adapter.getResult(); // Mendapatkan hasil
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Menginisialisasi instance baru dari kelas StringOutputAdapter. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getResult()](#getResult--) | Mendapatkan string hasil. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Menginisialisasi instance baru dari kelas StringOutputAdapter.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Format output. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Mendapatkan string hasil.


**Returns:**
java.lang.String - String hasil.

