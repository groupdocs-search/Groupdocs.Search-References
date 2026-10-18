---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Çıktıyı bir java.io.OutputStream içine toplayan bir çıktı adaptörünü temsil eder."
type: docs
weight: 31
url: /tr/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Çıktıyı bir java.io.OutputStream içine toplayan bir çıktı adaptörünü temsil eder.


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Çıktı akışı oluşturuluyor
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Bir akış çıktı adaptörü oluşturuluyor
index.getDocumentText(documents[0], adapter); // Belge metni akışa oluşturuluyor
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | StreamOutputAdapter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getStream()](#getStream--) | Bir çıktı akışı alır. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


StreamOutputAdapter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Çıktı biçimi. |
|
|  | stream | java.io.OutputStream | Çıktı akışı. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Bir çıktı akışı alır.


**Returns:**
java.io.OutputStream - Çıktı akışı.

