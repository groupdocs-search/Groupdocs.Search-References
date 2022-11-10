---
title: CreateFilePathRegularExpression
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. Lexpression régulière est appliquée au chemin complet dun document.
type: docs
weight: 40
url: /fr/net/groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression/
---
## CreateFilePathRegularExpression(string) {#createfilepathregularexpression}

Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pattern | String | Le modèle d'expression régulière. |

### Return_Value

Un filtre de recherche de document par nom de fichier.

### Voir également

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* espace de noms [GroupDocs.Search.Options](../../searchdocumentfilter)
* Assemblée [GroupDocs.Search](../../../)

---

## CreateFilePathRegularExpression(string, RegexOptions) {#createfilepathregularexpression_1}

Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.

```csharp
public static ISearchDocumentFilter CreateFilePathRegularExpression(string pattern, 
    RegexOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pattern | String | Le modèle d'expression régulière. |
| options | RegexOptions | Les options d'expression régulière. |

### Return_Value

Un filtre de recherche de document par nom de fichier.

### Voir également

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchDocumentFilter](../../searchdocumentfilter)
* espace de noms [GroupDocs.Search.Options](../../searchdocumentfilter)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->