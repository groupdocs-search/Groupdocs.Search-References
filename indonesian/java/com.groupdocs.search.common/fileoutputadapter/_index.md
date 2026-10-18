---
title: "FileOutputAdapter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili adaptor output yang mengumpulkan output ke dalam file."
type: docs
weight: 21
url: /id/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Mewakili adaptor output yang mengumpulkan output ke dalam file.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Membuat adapter output file
index.getDocumentText(documents[0], adapter); // Menghasilkan teks dokumen ke dalam file output
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Menginisialisasi instance baru dari kelas  FileOutputAdapter  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Mendapatkan jalur file output. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Menginisialisasi instance baru dari kelas  FileOutputAdapter  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Format output. |
|
|  | filePath | java.lang.String | Jalur file output. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Mendapatkan jalur file output.


**Returns:**
java.lang.String - Jalur file output.

