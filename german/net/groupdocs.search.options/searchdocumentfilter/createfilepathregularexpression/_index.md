---
title: "CreateFilePathRegularExpression"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet."
type: docs
weight: 40
url: /de/net/groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression/
---
## CreateFilePathRegularExpression(string) {#createfilepathregularexpression}

Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Muster | String | Das reguläre Ausdrucksmuster. |

### Rückgabewert

Ein Suchdokumentfilter nach Dateinamen.

### Siehe auch

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

---

## CreateFilePathRegularExpression(string, RegexOptions) {#createfilepathregularexpression_1}

Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern, 
    RegexOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Muster | String | Das reguläre Ausdrucksmuster. |
| Optionen | RegexOptions | Die Optionen für reguläre Ausdrücke. |

### Rückgabewert

Ein Suchdokumentfilter nach Dateinamen.

### Siehe auch

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
