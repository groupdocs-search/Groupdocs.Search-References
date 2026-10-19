---
title: "GroupDocs.Search.Common"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Il namespace fornisce classi comuni della libreria."
type: docs
weight: 20
url: /it/net/groupdocs.search.common/
---
Il namespace fornisce classi comuni della libreria.

## Classi

| Classe | Descrizione |
| --- | --- |
| [AttributeChangeBatch](./attributechangebatch) | Rappresenta un contenitore per le modifiche agli attributi. |
| [Cancellation](./cancellation) | Rappresenta un oggetto per richiedere la cancellazione di un'operazione. |
| [ChunkSearchToken](./chunksearchtoken) | Rappresenta un token per la continuazione della ricerca a blocchi (ricerca per pagine). |
| [CustomExtractorCollection](./customextractorcollection) | Contiene una raccolta di estrattori personalizzati. Se la raccolta contiene un estrattore per qualche estensione di file coperta dagli estrattori integrati, allora questo estrattore verrà utilizzato al posto di quello integrato. |
| [Document](./document) | Rappresenta la classe base per i documenti aggiunti a un indice dal file system, dallo stream o dalla struttura. Contiene metodi statici per creare documenti da diversi tipi di sorgenti. |
| [DocumentField](./documentfield) | Rappresenta i dati di un campo del documento. |
| [DocumentImage](./documentimage) | Rappresenta i dati dell'immagine di un documento. |
| [Encodings](./encodings) | Contiene i nomi delle possibili codifiche. |
| [ExtractedData](./extracteddata) | Rappresenta i dati recuperati da un documento e preparati per l'indicizzazione. |
| [ExtractedItemInfo](./extractediteminfo) | Rappresenta le informazioni di un elemento del contenitore. |
| [ExtractorSettings](./extractorsettings) | Contiene le impostazioni per l'estrattore di dati del documento. |
| [FileLogger](./filelogger) | Rappresenta un logger che registra eventi ed errori in un file locale. |
| [FileOutputAdapter](./fileoutputadapter) | Rappresenta un adattatore di output che raccoglie l'output in un file. |
| [FragmentContainer](./fragmentcontainer) | Rappresenta un contenitore per frammenti di testo con i termini trovati evidenziati di un campo del documento. |
| [ImageFrame](./imageframe) | Rappresenta un fotogramma immagine. |
| [IndexInfo](./indexinfo) | Contiene informazioni di base su un indice. |
| [IndexingReport](./indexingreport) | Rappresenta informazioni dettagliate su un'operazione di indicizzazione. |
| [Notification](./notification) | La classe base per tutte le notifiche all'indice. Questa classe contiene anche metodi per creare oggetti di notifica. |
| [OutputAdapter](./outputadapter) | Rappresenta la classe base di un adattatore di output utilizzato per raccogliere un output in forma generalizzata. Gli adattatori attualmente disponibili sono [`FileOutputAdapter`](../groupdocs.search.common/fileoutputadapter), [`StreamOutputAdapter`](../groupdocs.search.common/streamoutputadapter), [`StructureOutputAdapter`](../groupdocs.search.common/structureoutputadapter) e [`StringOutputAdapter`](../groupdocs.search.common/stringoutputadapter). |
| [ResultBuilderFactory](./resultbuilderfactory) | Rappresenta la classe base di una fabbrica di costruttori di risultati. |
| [SearchImage](./searchimage) | Rappresenta un'immagine da cercare. |
| [SearchReport](./searchreport) | Rappresenta informazioni dettagliate su un'operazione di ricerca. |
| [StreamOutputAdapter](./streamoutputadapter) | Rappresenta un adattatore di output che raccoglie l'output in uno stream. |
| [StringOutputAdapter](./stringoutputadapter) | Rappresenta un adattatore di output che raccoglie l'output come stringa. |
| [StructureOutputAdapter](./structureoutputadapter) | Rappresenta un adattatore di output che raccoglie l'output come una struttura contenente ogni campo separatamente. |
| [WordPattern](./wordpattern) | Rappresenta un modello di parola da utilizzare nella ricerca wildcard di parole. |
## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [IContainerItemExtractor](./icontaineritemextractor) | Fornisce metodi per estrarre elementi da documenti contenitori. |
| [IDocumentLoader](./idocumentloader) | Definisce l'interfaccia del caricatore di documenti utilizzata per caricare documenti lazy. |
| [IFieldExtractor](./ifieldextractor) | Fornisce metodi per estrarre campi da un documento. |
| [ILogger](./ilogger) | Definisce l'interfaccia di un logger utilizzato per registrare eventi ed errori in un indice. |
| [IWordSplitter](./iwordsplitter) | Definisce un metodo per suddividere il testo in parole individuali. |
## Enumerazione

| Enumerazione | Descrizione |
| --- | --- |
| [DocumentSourceKind](./documentsourcekind) | Definisce i tipi di sorgenti di documento. |
| [DocumentStatus](./documentstatus) | Rappresenta lo stato di elaborazione di un documento. |
| [IndexStatus](./indexstatus) | Specifica lo stato di un indice. |
| [VersionUpdateResult](./versionupdateresult) | Rappresenta il risultato di un'operazione di aggiornamento della versione dell'indice. |

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
