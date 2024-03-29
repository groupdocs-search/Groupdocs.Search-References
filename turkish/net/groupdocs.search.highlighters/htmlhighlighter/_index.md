---
title: HtmlHighlighter
second_title: .NET API Başvurusu için GroupDocs.Search
description: HTMLde biçimlendirilmiş bir belge metninin tamamındaki arama sonuçlarını vurgulayan bir arama sonucu vurgulayıcıyı temsil eder.
type: docs
weight: 670
url: /tr/net/groupdocs.search.highlighters/htmlhighlighter/
---
## HtmlHighlighter class

HTML'de biçimlendirilmiş bir belge metninin tamamındaki arama sonuçlarını vurgulayan bir arama sonucu vurgulayıcıyı temsil eder.

```csharp
[Obsolete("Please, use the DocumentHighlighter class instead.")]
public class HtmlHighlighter : Highlighter
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Çıktı biçimini alır. |

### Notlar

**Daha fazla bilgi edin**

* [Arama sonuçlarını vurgulama](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Örnekler

Örnek, sınıfın tipik bir kullanımını göstermektedir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Bir dizin oluşturma
Index index = new Index(indexFolder);

// Belgeleri belirtilen klasörden indeksleme
index.Add(documentsFolder);

// 'Görelilik Teorisi' aşamasını arayın
SearchResult result = index.Search("\"Theory of Relativity\"");

// Bir belge metninde bulunan kelimeleri vurgulama
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new HtmlHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Ayrıca bakınız

* class [Highlighter](../highlighter)
* ad alanı [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
