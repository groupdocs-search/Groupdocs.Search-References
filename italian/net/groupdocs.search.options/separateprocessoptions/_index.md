---
title: "SeparateProcessOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per l'estrazione dei dati dai documenti in un processo separato."
type: docs
weight: 1110
url: /it/net/groupdocs.search.options/separateprocessoptions/
---
## SeparateProcessOptions class

Fornisce opzioni per l'estrazione dei dati dai documenti in un processo separato.

```csharp
public class SeparateProcessOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AssemblyPath](../../groupdocs.search.options/separateprocessoptions/assemblypath) { get; set; } | Ottiene o imposta il percorso dell'assembly del processo separato. |
| [ExtractInSeparateProcess](../../groupdocs.search.options/separateprocessoptions/extractinseparateprocess) { get; set; } | Ottiene o imposta un valore che indica se un processo separato è utilizzato per estrarre dati dai documenti. Il valore predefinito è `false`. Quando questa opzione è abilitata, l'estrazione dei dati viene eseguita in un processo separato con un solo thread. Il numero specificato di thread viene ignorato durante l'estrazione in un processo separato. |
| [Timeout](../../groupdocs.search.options/separateprocessoptions/timeout) { get; set; } | Ottiene o imposta il tempo massimo di attesa per il risultato dell'estrazione dei dati in un processo separato. Il valore predefinito è 10 minuti. |
| [UseDotnetToStartProcess](../../groupdocs.search.options/separateprocessoptions/usedotnettostartprocess) { get; set; } | Ottiene o imposta il flag per l'uso di `dotnet` per avviare il processo. Il valore predefinito è `true`. Imposta il valore su `false` se desideri avviare un'applicazione autonoma. Nota che `dotnet` non viene mai utilizzato per avviare sul vecchio .NET Framework. |

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
