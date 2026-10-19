---
title: "CreateFilePathRegularExpression"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento."
type: docs
weight: 40
url: /it/net/groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression/
---
## CreateFilePathRegularExpression(string) {#createfilepathregularexpression}

Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| modello | String | Il modello dell'espressione regolare. |

### Valore di ritorno

Un filtro di ricerca dei documenti per nome file.

### Vedi anche

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

---

## CreateFilePathRegularExpression(string, RegexOptions) {#createfilepathregularexpression_1}

Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern, 
    RegexOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| modello | String | Il modello dell'espressione regolare. |
| opzioni | RegexOptions | Le opzioni dell'espressione regolare. |

### Valore di ritorno

Un filtro di ricerca dei documenti per nome file.

### Vedi anche

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
