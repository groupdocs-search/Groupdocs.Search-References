---
title: "CharacterReplacementDictionary"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Representa un diccionario de reemplazo de caracteres que se utiliza durante el proceso de indexación. El reemplazo de caracteres puede usarse, por ejemplo, para eliminar acentos de caracteres acentuados o para crear un índice que no distinga entre mayúsculas y minúsculas."
type: docs
weight: 390
url: /es/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Representa un diccionario de sustitución de caracteres que se utiliza durante el proceso de indexación. La sustitución de caracteres puede usarse, por ejemplo, para eliminar acentos de caracteres acentuados o para crear un índice que no distinga entre mayúsculas y minúsculas.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Obtiene el número de puntos de código Unicode contenidos en este [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Obtiene el tipo de diccionario. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Añade la colección especificada de reemplazos de caracteres a esta instancia de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Añade la colección especificada de reemplazos de caracteres a esta instancia de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Añade la colección especificada de reemplazos de caracteres a esta instancia de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Añade la colección especificada de reemplazos de puntos de código Unicode a esta instancia de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Elimina todos los reemplazos de caracteres de un objeto [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Determina si un objeto [`CharacterReplacementDictionary`](../characterreplacementdictionary) contiene un reemplazo para el punto de código Unicode especificado. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporta el diccionario a un archivo con el nombre especificado. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Devuelve un enumerador que itera a través de la colección. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Obtiene un reemplazo para el punto de código Unicode especificado. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un diccionario del archivo especificado. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Elimina la colección especificada de reemplazos de caracteres de esta instancia del [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Elimina la colección especificada de reemplazos de caracteres de esta instancia del [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Elimina la colección especificada de reemplazos de puntos de código Unicode de esta instancia del [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Elimina la colección especificada de reemplazos de puntos de código Unicode de esta instancia del [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Observaciones

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Ver también

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
