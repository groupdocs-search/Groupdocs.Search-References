---
title: StringOutputAdapter
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta un adattatore di output che raccoglie loutput come aString .
type: docs
weight: 310
url: /it/net/groupdocs.search.common/stringoutputadapter/
---
## StringOutputAdapter class

Rappresenta un adattatore di output che raccoglie l'output come aString .

```csharp
public class StringOutputAdapter : OutputAdapter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [StringOutputAdapter](stringoutputadapter)() | Inizializza una nuova istanza di[`StringOutputAdapter`](../stringoutputadapter) classe. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetResult](../../groupdocs.search.common/stringoutputadapter/getresult)() | Ottiene la stringa risultante. |

### Osservazioni

**Scopri di più**

* [Adattatori di uscita](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata

index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

DocumentInfo[] documents = index.GetIndexedDocuments(); // Ottenere informazioni sui documenti indicizzati

StringOutputAdapter adapter = new StringOutputAdapter(); // Creazione di un adattatore di output di stringa
index.GetDocumentText(documents[0], adapter); // Generazione di un documento di testo nell'adattatore
String result = adapter.GetResult(); // Ottenere un risultato
```

### Guarda anche

* class [OutputAdapter](../outputadapter)
* spazio dei nomi [GroupDocs.Search.Common](../../groupdocs.search.common)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->