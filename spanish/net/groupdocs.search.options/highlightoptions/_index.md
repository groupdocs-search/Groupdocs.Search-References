---
title: "HighlightOptions"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Proporciona opciones para resaltar los términos encontrados."
type: docs
weight: 910
url: /es/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Proporciona opciones para resaltar los términos encontrados.

```csharp
public class HighlightOptions : TextOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Inicializa una nueva instancia de la clase [`HighlightOptions`](../highlightoptions). |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Obtiene o establece los campos de documento adicionales que se usaron para indexar. El valor predeterminado es `null`. Tenga en cuenta que este valor se usa solo si el texto del documento no se guardó en el índice. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Obtiene o establece un valor que indica si se debe detectar la codificación automáticamente o no. El valor predeterminado es `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Obtiene o establece el objeto de cancelación. El valor predeterminado es `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Obtiene o establece el extractor de texto personalizado que se usó para indexar. El valor predeterminado es `null`. Tenga en cuenta que este valor se usa solo si el texto del documento no se guardó en el índice. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Obtiene o establece la codificación utilizada para extraer texto de documentos de texto. El valor predeterminado es `null`, lo que significa que se usa la codificación predeterminada UTF-8. Si AutoDetectEncoding es `true`, entonces este valor se usa como la codificación predeterminada. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Obtiene o establece un valor que indica si la etiqueta Head se genera en el HTML de salida. El valor predeterminado es `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Obtiene o establece un color que se usa para resaltar ocurrencias. El valor predeterminado es #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Obtiene las opciones de indexación de imágenes para búsqueda inversa de imágenes. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Obtiene las opciones para indexar campos de metadatos. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Obtiene las opciones para el procesamiento OCR y la indexación del texto reconocido. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Obtiene o establece la etiqueta de cierre del resaltado de la palabra encontrada. Esta etiqueta se usa solo al resaltar en texto plano. El valor predeterminado es una cadena vacía. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Obtiene o establece la etiqueta de inicio del resaltado de la palabra encontrada. Esta etiqueta se usa solo al resaltar en texto plano. El valor predeterminado es una cadena vacía. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Obtiene o establece el número máximo de palabras en un fragmento de texto después de la palabra resaltada. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Obtiene o establece el número máximo de palabras en un fragmento de texto antes de la palabra resaltada. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Obtiene o establece el número máximo de palabras en un fragmento de texto. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Obtiene o establece un valor que indica si el proceso debe usar SeBackupPrivilege y FILE_FLAG_BACKUP_SEMANTICS para acceder a archivos y directorios. El valor predeterminado es `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Obtiene o establece un valor que indica si se usan estilos en línea para resaltar ocurrencias. El valor predeterminado es `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Obtiene o establece un valor que indica si se usa el modo sin procesar para la extracción de texto cuando sea posible. El valor predeterminado es `false`. El modo sin procesar puede aumentar significativamente la velocidad de indexación, pero el modo normal mejora el formato del texto extraído. |

### Observaciones

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Ver también

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
