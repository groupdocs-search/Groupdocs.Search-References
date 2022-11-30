---
title: GetIndexedDocumentItems
second_title: .NET API Başvurusu için GroupDocs.Search
description: Belirtilen belgenin iç içe geçmiş öğelerinin bir dizisini alır ZIP OST PST gibi kapsayıcı belgeler için.
type: docs
weight: 130
url: /tr/net/groupdocs.search/index/getindexeddocumentitems/
---
## Index.GetIndexedDocumentItems method

Belirtilen belgenin iç içe geçmiş öğelerinin bir dizisini alır (ZIP, OST, PST gibi kapsayıcı belgeler için).

```csharp
public DocumentInfo[] GetIndexedDocumentItems(DocumentInfo documentInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| documentInfo | DocumentInfo | Belge bilgisi. |

### Geri dönüş değeri

Belge öğeleri dizisi.

### Örnekler

Örnek, bir index. 'den indekslenmiş bir belgenin öğelerinin listesinin nasıl alınacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Belirtilen klasörde bir dizin oluşturma
Index index = new Index(indexFolder);
 
// Belgeleri belirtilen klasörden indeksleme
index.Add(documentsFolder);
 
// İndekslenmiş dokümanların listesini almak
DocumentInfo[] documents = index.GetIndexedDocuments();
for (int i = 0; i < documents.Length; i++)
{
    DocumentInfo document = documents[i];
    Console.WriteLine(document.FilePath);
    DocumentInfo[] items = index.GetIndexedDocumentItems(document); // Belge öğelerinin listesi alınıyor
    for (int j = 0; j < items.Length; j++)
    {
        DocumentInfo item = items[j];
        Console.WriteLine("\t" + item.InnerPath);
    }
}
```

### Ayrıca bakınız

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->