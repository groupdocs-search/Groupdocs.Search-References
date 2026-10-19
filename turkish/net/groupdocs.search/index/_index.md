---
title: "Index"
second_title: "GroupDocs.Search için .NET API Referansı"
description: "Belgeleri indekslemek ve içinde arama yapmak için ana sınıfı temsil eder."
type: docs
weight: 700
url: /tr/net/groupdocs.search/index/
---
## Index class

Belgeleri indekslemek ve içinde arama yapmak için ana sınıfı temsil eder.

```csharp
public class Index : IDisposable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Index](index#constructor)() | Bellekte yeni bir [`Index`](../index) sınıfının örneğini başlatır. |
| [Index](index#constructor_1)(IndexSettings) | Bellekte, belirli dizin ayarlarıyla yeni bir [`Index`](../index) sınıfının örneğini başlatır. |
| [Index](index#constructor_2)(string) | Yeni bir [`Index`](../index) sınıfının örneğini başlatır. Diskte yeni bir dizin oluşturur veya mevcut bir dizini açar. |
| [Index](index#constructor_3)(string, bool) | Yeni bir [`Index`](../index) sınıfının örneğini başlatır. *overwriteIfExists* `false` ise diskten mevcut bir dizini yükler; aksi takdirde disk üzerinde yeni bir dizin oluşturur. |
| [Index](index#constructor_4)(string, IndexSettings) | Yeni bir [`Index`](../index) sınıfının bir örneğini başlatır. Belirli ayarlarla yeni bir indeks oluşturur veya diskte mevcut bir indeksi açar. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Yeni bir [`Index`](../index) sınıfının bir örneğini başlatır. *overwriteIfExists* `false` ise diskteki mevcut bir indeksi yükler; aksi takdirde belirli indeks ayarlarıyla diskte yeni bir indeks oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Sözlük deposunu alır. |
| [Events](../../groupdocs.search/index/events) { get; } | Olaylara abone olmak için olay hub'ını alır. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | İndeks hakkında temel bilgileri alır. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | İndeks ayarlarını alır. |
| [Repository](../../groupdocs.search/index/repository) { get; } | İndeks içinde bulunuyorsa indeks depo nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Tüm indeksi belleğe yükler. İndekse yapılan değişiklikler otomatik olarak orijinal klasöre kaydedilmez. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Tüm indeksi belleğe yükler. İndekse yapılan değişiklikler otomatik olarak orijinal klasöre kaydedilmez. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile bir dosya veya klasör ekler. Tüm alt klasörlerden belgeler indekslenecektir. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile dosyalar veya klasörler ekler. Tüm alt klasörlerden belgeler indekslenecektir. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | İndeksleme işlemini gerçekleştirir. Dosya sisteminden, akıştan veya yapıyıdan belgeler ekler. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | İndeksleme işlemini gerçekleştirir. Çıkarılan verileri indekse ekler. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile bir dosya veya klasör ekler. Tüm alt klasörlerden belgeler indekslenecektir. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile dosyalar veya klasörler ekler. Tüm alt klasörlerden belgeler indekslenecektir. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Güncelleme işlemi sırasında yeniden indekslemeden, belirtilen öznitelik değişiklikleri topluluğunu indekslenmiş belgelere uygular. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | *fixIndexFunctionality* `true` ise yöntem, hasarlı segmentlerin varlığında indeks işlevselliğini düzeltir; aksi takdirde düzeltmez. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | İndeksten indekslenmiş dosya veya klasörleri siler. Ardından silinen yollar olmadan indeksi günceller. Bir belge, bir klasörün parçası olarak indekse eklenmişse, tek başına indeksden silinemez. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Akışlardan veya yapılardan indekslenen belgeleri siler. Ardından silinen belgeler olmadan indeksi günceller. |
| [Dispose](../../groupdocs.search/index/dispose)() | [`Index`](../index) tarafından kullanılan tüm kaynakları serbest bırakır. |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Belirtilen indekslenmiş belgeyle ilişkili tüm öznitelikleri alır. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | İndekslenmiş bir belgenin metnini oluşturur ve bir çıktı adaptörü aracılığıyla iletir. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | İndekslenmiş belge için HTML biçimlendirilmiş metin oluşturur ve çıktı adaptörü aracılığıyla aktarır. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Belge anahtarına göre bir indekslenmiş belge alır. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Belirtilen belgenin (ZIP, OST, PST gibi kapsayıcı belgeler için) iç içe öğeler dizisini alır. |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Tüm indekslenmiş belgelerin bir dizisini alır. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | İndekslenmiş yolların - belgeler veya klasörler - bir dizisini alır. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | İndeksleme işlemleriyle ilgili raporları alır. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Arama işlemleriyle ilgili raporları alır. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Bulunan terimleri vurgulayarak HTML biçimlendirilmiş metin oluşturur. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Bulunan terimleri vurgulayarak HTML biçimlendirilmiş metin oluşturur. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Belirtilen dizini mevcut dizinle birleştirir. Diğer dizinin değişmeyeceğini unutmayın. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Belirtilen dizin deposundaki dizinleri mevcut dizine birleştirir. Depodaki dizinlerin değişmeyeceğini unutmayın. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Belirtilen bildirim nesnesini bildirimi gerçekleştirmek için dizine iletir. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Dizin segmentlerinin sayısını birbiriyle birleştirerek en aza indirir. Bu işlem arama performansını artırır. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Dizin segmentlerinin sayısını birbiriyle birleştirerek en aza indirir. Bu işlem arama performansını artırır. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Bellek içi dizini diske kaydeder. Ayrıca normal dizini başka bir klasöre kaydeder. Bu dizinin ayarlarını değiştirmez. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Dizinde arama yapar. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Dizinde arama yapar. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Dizinde ters görüntü araması gerçekleştirir. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Dizinde arama yapar. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Dizinde arama yapar. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Search yöntemiyle başlatılan parça aramasına devam eder. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Search yöntemiyle başlatılan parça aramasına devam eder. |
| [Update](../../groupdocs.search/index/update#update)() | Son güncellemeden beri değiştirilen veya silinen belgeleri yeniden dizinler. Dizinlenmiş klasörlere eklenen yeni dosyaları ekler. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Son güncellemeden beri değiştirilen veya silinen belgeleri yeniden dizinler. Dizinlenmiş klasörlere eklenen yeni dosyaları ekler. |

### Açıklamalar

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Örnekler

Bu örnek, sınıfın tipik bir kullanımını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Ayrıca Bakınız

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
