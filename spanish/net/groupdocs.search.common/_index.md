---
title: "GroupDocs.Search.Common"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "El espacio de nombres proporciona clases comunes de la biblioteca."
type: docs
weight: 20
url: /es/net/groupdocs.search.common/
---
El espacio de nombres proporciona clases comunes de la biblioteca.

## Clases

| Clase | Descripción |
| --- | --- |
| [AttributeChangeBatch](./attributechangebatch) | Representa un contenedor para cambios de atributos. |
| [Cancellation](./cancellation) | Representa un objeto para solicitar la cancelación de una operación. |
| [ChunkSearchToken](./chunksearchtoken) | Representa un token para la continuación de la búsqueda por fragmentos (búsqueda por páginas). |
| [CustomExtractorCollection](./customextractorcollection) | Contiene una colección de extractores personalizados. Si la colección contiene un extractor para alguna extensión de archivo que está cubierta por extractores incorporados, entonces este extractor se usará en lugar del incorporado. |
| [Document](./document) | Representa la clase base para documentos añadidos a un índice desde el sistema de archivos, flujo o estructura. Contiene métodos estáticos para crear documentos a partir de diferentes tipos de fuentes. |
| [DocumentField](./documentfield) | Representa los datos de un campo de documento. |
| [DocumentImage](./documentimage) | Representa los datos de imagen de un documento. |
| [Encodings](./encodings) | Contiene nombres de codificaciones posibles. |
| [ExtractedData](./extracteddata) | Representa los datos obtenidos de un documento y preparados para la indexación. |
| [ExtractedItemInfo](./extractediteminfo) | Representa la información de un elemento de contenedor. |
| [ExtractorSettings](./extractorsettings) | Contiene la configuración del extractor de datos del documento. |
| [FileLogger](./filelogger) | Representa un registrador que registra eventos y errores en un archivo local. |
| [FileOutputAdapter](./fileoutputadapter) | Representa un adaptador de salida que recopila la salida en un archivo. |
| [FragmentContainer](./fragmentcontainer) | Representa un contenedor para fragmentos de texto con los términos encontrados resaltados de un campo de documento. |
| [ImageFrame](./imageframe) | Representa un marco de imagen. |
| [IndexInfo](./indexinfo) | Contiene información básica sobre un índice. |
| [IndexingReport](./indexingreport) | Representa información detallada sobre una operación de indexación. |
| [Notification](./notification) | La clase base para todas las notificaciones al índice. Esta clase también contiene métodos para crear objetos de notificación. |
| [OutputAdapter](./outputadapter) | Representa la clase base de un adaptador de salida que se utiliza para recopilar una salida en forma generalizada. Los adaptadores disponibles actualmente son [`FileOutputAdapter`](../groupdocs.search.common/fileoutputadapter), [`StreamOutputAdapter`](../groupdocs.search.common/streamoutputadapter), [`StructureOutputAdapter`](../groupdocs.search.common/structureoutputadapter) y [`StringOutputAdapter`](../groupdocs.search.common/stringoutputadapter). |
| [ResultBuilderFactory](./resultbuilderfactory) | Representa la clase base de una fábrica de constructores de resultados. |
| [SearchImage](./searchimage) | Representa una imagen para buscar. |
| [SearchReport](./searchreport) | Representa información detallada sobre una operación de búsqueda. |
| [StreamOutputAdapter](./streamoutputadapter) | Representa un adaptador de salida que recopila la salida en un flujo. |
| [StringOutputAdapter](./stringoutputadapter) | Representa un adaptador de salida que recopila la salida como una cadena. |
| [StructureOutputAdapter](./structureoutputadapter) | Representa un adaptador de salida que recopila la salida como una estructura que contiene cada campo por separado. |
| [WordPattern](./wordpattern) | Representa un patrón de palabra para usar en la búsqueda de comodines de palabras. |
## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [IContainerItemExtractor](./icontaineritemextractor) | Proporciona métodos para extraer elementos de documentos contenedores. |
| [IDocumentLoader](./idocumentloader) | Define la interfaz del cargador de documentos que se utiliza para cargar documentos perezosos. |
| [IFieldExtractor](./ifieldextractor) | Proporciona métodos para extraer campos de un documento. |
| [ILogger](./ilogger) | Define la interfaz de un registrador que se utiliza para registrar eventos y errores en un índice. |
| [IWordSplitter](./iwordsplitter) | Define un método para dividir el texto en palabras individuales. |
## Enumeración

| Enumeración | Descripción |
| --- | --- |
| [DocumentSourceKind](./documentsourcekind) | Define los tipos de fuentes de documentos. |
| [DocumentStatus](./documentstatus) | Representa el estado de procesamiento de un documento. |
| [IndexStatus](./indexstatus) | Especifica el estado de un índice. |
| [VersionUpdateResult](./versionupdateresult) | Representa el resultado de una operación de actualización de versión de índice. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
