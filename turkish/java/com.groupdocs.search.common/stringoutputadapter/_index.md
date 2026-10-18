---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Çıktıyı System.String olarak toplayan bir çıktı adaptörünü temsil eder."
type: docs
weight: 32
url: /tr/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Çıktıyı bir System.String olarak toplayan bir çıktı adaptörünü temsil eder.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // Bir string çıktı adaptörü oluşturma
index.getDocumentText(documents[0], adapter); // Belge metnini adaptöre oluşturma
String result = adapter.getResult(); // Sonuç alınıyor
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StringOutputAdapter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getResult()](#getResult--) | Sonuç dizesini alır. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


StringOutputAdapter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Çıktı biçimi. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Sonuç dizesini alır.


**Returns:**
java.lang.String - Sonuç dizesi.

