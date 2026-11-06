---
title: "HighlightOptions"
second_title: "GroupDocs.Search için .NET API Referansı"
description: "Bulunan terimleri vurgulamak için seçenekler sağlar."
type: docs
weight: 910
url: /tr/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Bulunan terimleri vurgulamak için seçenekler sağlar.

```csharp
public class HighlightOptions : TextOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Yeni bir [`HighlightOptions`](../highlightoptions) sınıf örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Dizineleme için kullanılan ek belge alanlarını alır veya ayarlar. Varsayılan değer `null`dır. Bu değerin yalnızca belge metni dizine kaydedilmemişse kullanıldığını unutmayın. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Kodlamanın otomatik olarak algılanıp algılanmayacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer `false`dır. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | İptal nesnesini alır veya ayarlar. Varsayılan değer `null`dır. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Dizineleme için kullanılan özel metin çıkarıcıyı alır veya ayarlar. Varsayılan değer `null`dır. Bu değerin yalnızca belge metni dizine kaydedilmemişse kullanıldığını unutmayın. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Metin belgelerinden metin çıkarmak için kullanılan kodlamayı alır veya ayarlar. Varsayılan değer `null`dır, bu da varsayılan kodlama UTF-8'in kullanıldığı anlamına gelir. AutoDetectEncoding `true` ise bu değer varsayılan kodlama olarak kullanılır. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Çıktı HTML'de Head etiketinin oluşturulup oluşturulmayacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer `true`dır. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Oluşumları vurgulamak için kullanılan bir rengi alır veya ayarlar. Varsayılan değer #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Ters görüntü araması için görüntü indeksleme seçeneklerini alır. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Meta veri alanlarını indeksleme seçeneklerini alır. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | OCR işleme ve tanınan metni indeksleme seçeneklerini alır. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Bulunan kelimenin vurgulanmasının son etiketini alır veya ayarlar. Bu etiket yalnızca düz metinde vurgulama yapıldığında kullanılır. Varsayılan değer boş bir dizedir. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Bulunan kelimenin vurgulanmasının başlangıç etiketini alır veya ayarlar. Bu etiket yalnızca düz metinde vurgulama yapıldığında kullanılır. Varsayılan değer boş bir dizedir. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Vurgulanan kelimenin ardından bir metin parçasındaki maksimum kelime sayısını alır veya ayarlar. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Vurgulanan kelimenin öncesinde bir metin parçasındaki maksimum kelime sayısını alır veya ayarlar. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Bir metin parçasındaki maksimum kelime sayısını alır veya ayarlar. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | İşlemin dosya ve dizinlere erişmek için SeBackupPrivilege ve FILE_FLAG_BACKUP_SEMANTICS kullanıp kullanmayacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Olayların vurgulanması için satır içi stillerin kullanılıp kullanılmadığını gösteren bir değeri alır veya ayarlar. Varsayılan değer `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Mümkünse metin çıkarımı için ham modun kullanılıp kullanılmadığını gösteren bir değeri alır veya ayarlar. Varsayılan değer `false`. Ham mod indeksleme hızını önemli ölçüde artırabilir, ancak normal mod çıkarılan metnin biçimlendirmesini iyileştirir. |

### Açıklamalar

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Ayrıca Bakınız

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
