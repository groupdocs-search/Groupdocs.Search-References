---
title: "CreateMasterNode"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée un nœud maître du réseau de recherche."
type: docs
weight: 10
url: /fr/net/groupdocs.search.scaling/searchnetworknode/createmasternode/
---
## SearchNetworkNode.CreateMasterNode method

Crée un nœud maître du réseau de recherche.

```csharp
public static SearchNetworkNode CreateMasterNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nodeIndex | Int32 | L'index du nœud. |
| storagePath | String | Le chemin de stockage. |
| networkSettings | INetworkSettings | Les paramètres du réseau. |
| logger | ILogger | Le logger. |
| configuration | Configuration | La configuration. |

### Valeur de retour

Le nœud maître.

### Voir aussi

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* interface [ILogger](../../../groupdocs.search.common/ilogger)
* class [Configuration](../../../groupdocs.search.scaling.configuring/configuration)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
