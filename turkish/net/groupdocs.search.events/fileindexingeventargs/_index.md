---
title: FileIndexingEventArgs
second_title: .NET API Başvurusu için GroupDocs.Search
description: Bir belge indeksleme başlangıcı olayı için bağımsız değişkenleri temsil eder.
type: docs
weight: 520
url: /tr/net/groupdocs.search.events/fileindexingeventargs/
---
## FileIndexingEventArgs class

Bir belge indeksleme başlangıcı olayı için bağımsız değişkenleri temsil eder.

```csharp
public class FileIndexingEventArgs : BaseIndexEventArgs
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.events/fileindexingeventargs/additionalfields) { get; set; } | Belge için ek alanları alır veya ayarlar. |
| [Attributes](../../groupdocs.search.events/fileindexingeventargs/attributes) { get; set; } | Belgenin özniteliklerini alır veya ayarlar. |
| [CustomExtractor](../../groupdocs.search.events/fileindexingeventargs/customextractor) { get; set; } | Özel metin çıkarıcıyı alır veya ayarlar. |
| [Document](../../groupdocs.search.events/fileindexingeventargs/document) { get; } | Belgeyi alır. |
| [DocumentFullPath](../../groupdocs.search.events/fileindexingeventargs/documentfullpath) { get; } | Belgenin tam yolunu alır. |
| [DocumentKey](../../groupdocs.search.events/fileindexingeventargs/documentkey) { get; } | Belge anahtarını alır. |
| [Encoding](../../groupdocs.search.events/fileindexingeventargs/encoding) { get; set; } | Belgenin kodlamasını alır veya ayarlar. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Dizin klasörünü alır. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Dizin kimliğini alır. |
| [SkipIndexing](../../groupdocs.search.events/fileindexingeventargs/skipindexing) { get; set; } | Belgenin indekslenmesinin atlanması gerektiğini belirten bir değer alır veya ayarlar. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Dizin durumunu alır. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Bir olayın zamanını alır. |

### Notlar

**Daha fazla bilgi edin**

* [Dizin etkinliklerini ara](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Ayrıca bakınız

* class [BaseIndexEventArgs](../baseindexeventargs)
* ad alanı [GroupDocs.Search.Events](../../groupdocs.search.events)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
