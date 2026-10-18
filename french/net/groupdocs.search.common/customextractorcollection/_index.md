---
title: "CustomExtractorCollection"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Contient une collection d'extracteurs personnalisés. Si la collection contient un extracteur pour une extension de fichier qui est couverte par les extracteurs intégrés, alors cet extracteur sera utilisé à la place de celui intégré."
type: docs
weight: 40
url: /fr/net/groupdocs.search.common/customextractorcollection/
---
## CustomExtractorCollection class

Contient une collection d'extracteurs personnalisés. Si la collection contient un extracteur pour une extension de fichier prise en charge par les extracteurs intégrés, alors cet extracteur sera utilisé à la place de celui intégré.

```csharp
public class CustomExtractorCollection : ICollection<IFieldExtractor>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.common/customextractorcollection/count) { get; } | Obtient le nombre d'extracteurs contenus dans la collection. |
| [IsReadOnly](../../groupdocs.search.common/customextractorcollection/isreadonly) { get; } | Obtient une valeur indiquant si la collection est en lecture seule. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../groupdocs.search.common/customextractorcollection/add)(IFieldExtractor) | Ajoute un extracteur à la collection. |
| [Clear](../../groupdocs.search.common/customextractorcollection/clear)() | Supprime tous les extracteurs de la collection. |
| [Contains](../../groupdocs.search.common/customextractorcollection/contains)(IFieldExtractor) | Détermine si la collection contient un extracteur spécifique. |
| [CopyTo](../../groupdocs.search.common/customextractorcollection/copyto)(IFieldExtractor[], int) | Copie les éléments de la collection dans un tableau, en commençant à un indice de tableau particulier. |
| [GetEnumerator](../../groupdocs.search.common/customextractorcollection/getenumerator)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../groupdocs.search.common/customextractorcollection/remove)(IFieldExtractor) | Supprime un extracteur de la collection. |

### Remarques

**Learn more**

* [Custom text extractors](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Voir aussi

* interface [IFieldExtractor](../ifieldextractor)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
