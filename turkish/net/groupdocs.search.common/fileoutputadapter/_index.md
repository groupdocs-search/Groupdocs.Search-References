---
title: FileOutputAdapter
second_title: .NET API Başvurusu için GroupDocs.Search
description: Çıktıyı bir dosyada toplayan bir çıktı bağdaştırıcısını temsil eder.
type: docs
weight: 150
url: /tr/net/groupdocs.search.common/fileoutputadapter/
---
## FileOutputAdapter class

Çıktıyı bir dosyada toplayan bir çıktı bağdaştırıcısını temsil eder.

```csharp
public class FileOutputAdapter : OutputAdapter
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [FileOutputAdapter](fileoutputadapter#constructor)(OutputFormat, string) | Yeni bir örneğini başlatır.[`FileOutputAdapter`](../fileoutputadapter) sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [FilePath](../../groupdocs.search.common/fileoutputadapter/filepath) { get; } | Bir çıktı dosyası yolu alır. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Çıktı biçimini alır. |

### Notlar

**Daha fazla bilgi edin**

* [Çıkış adaptörleri](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Örnekler

Örnek, sınıfın tipik bir kullanımını göstermektedir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Belirtilen klasörde bir dizin oluşturma

index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

DocumentInfo[] documents = index.GetIndexedDocuments(); // Dizinlenmiş belgeler hakkında bilgi alma

FileOutputAdapter adapter = new FileOutputAdapter(@"c:\DocumentText.htm"); // Bir dosya çıkış bağdaştırıcısı oluşturma
index.GetDocumentText(documents[0], adapter); // Çıktı dosyasına bir belge metni oluşturma
```

### Ayrıca bakınız

* class [OutputAdapter](../outputadapter)
* ad alanı [GroupDocs.Search.Common](../../groupdocs.search.common)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
