---
title: "CreateFilePathRegularExpression"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document."
type: docs
weight: 40
url: /fr/net/groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression/
---
## CreateFilePathRegularExpression(string) {#createfilepathregularexpression}

Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| modèle | String | Le modèle d'expression régulière. |

### Valeur de retour

Un filtre de recherche de documents par nom de fichier.

### Voir aussi

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

---

## CreateFilePathRegularExpression(string, RegexOptions) {#createfilepathregularexpression_1}

Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern, 
    RegexOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| modèle | String | Le modèle d'expression régulière. |
| options | RegexOptions | Les options d'expression régulière. |

### Valeur de retour

Un filtre de recherche de documents par nom de fichier.

### Voir aussi

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
