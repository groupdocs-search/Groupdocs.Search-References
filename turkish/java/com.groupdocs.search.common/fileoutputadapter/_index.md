---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Çıktıyı bir dosyaya toplayan bir çıktı adaptörünü temsil eder."
type: docs
weight: 21
url: /tr/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Çıktıyı bir dosyaya toplayan bir çıktı adaptörünü temsil eder.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
DocumentInfo[] documents = index.getIndexedDocuments(); // Dizinlenmiş belgeler hakkında bilgi alıyor
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Bir dosya çıktı bağdaştırıcısı oluşturuluyor
index.getDocumentText(documents[0], adapter); // Belge metnini çıktı dosyasına oluşturuyor
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | FileOutputAdapter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Bir çıktı dosyası yolunu alır. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


FileOutputAdapter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Çıktı biçimi. |
|
|  | filePath | java.lang.String | Çıktı dosyası yolu. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Bir çıktı dosyası yolunu alır.


**Returns:**
java.lang.String - Çıktı dosyası yolu.

