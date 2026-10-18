---
title: "SeparateProcessOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour extraire des données des documents dans un processus séparé."
type: docs
weight: 1110
url: /fr/net/groupdocs.search.options/separateprocessoptions/
---
## SeparateProcessOptions class

Fournit des options pour extraire des données des documents dans un processus séparé.

```csharp
public class SeparateProcessOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AssemblyPath](../../groupdocs.search.options/separateprocessoptions/assemblypath) { get; set; } | Obtient ou définit le chemin vers l'assembly du processus séparé. |
| [ExtractInSeparateProcess](../../groupdocs.search.options/separateprocessoptions/extractinseparateprocess) { get; set; } | Obtient ou définit une valeur indiquant si un processus séparé est utilisé pour extraire les données des documents. La valeur par défaut est `false`. Lorsque cette option est activée, l'extraction des données est effectuée dans un processus séparé avec un seul thread. Le nombre de threads spécifié est ignoré lors de l'extraction dans un processus séparé. |
| [Timeout](../../groupdocs.search.options/separateprocessoptions/timeout) { get; set; } | Obtient ou définit le temps maximal d'attente du résultat de l'extraction des données dans un processus séparé. La valeur par défaut est de 10 minutes. |
| [UseDotnetToStartProcess](../../groupdocs.search.options/separateprocessoptions/usedotnettostartprocess) { get; set; } | Obtient ou définit le drapeau d'utilisation de `dotnet` pour démarrer le processus. La valeur par défaut est `true`. Définissez la valeur sur `false` si vous souhaitez démarrer une application autonome. Notez que `dotnet` n'est jamais utilisé pour démarrer sur l'ancienne version du .NET Framework. |

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
