---
title: "UseBackupPrivilege"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient ou définit une valeur indiquant si le processus doit utiliser SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS pour accéder aux fichiers et répertoires. La valeur par défaut est false."
type: docs
weight: 70
url: /fr/net/groupdocs.search.options/baseoptions/usebackupprivilege/
---
## BaseOptions.UseBackupPrivilege property

Obtient ou définit une valeur indiquant si le processus doit utiliser SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS pour accéder aux fichiers et répertoires. La valeur par défaut est `false`.

```csharp
public bool UseBackupPrivilege { get; set; }
```

### Property Value

`true` pour activer l'accès privilégié en utilisant SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS ; sinon, `false`.

### Remarques

Lorsqu'il est activé, cela permet au processus de contourner les contrôles de sécurité des fichiers et répertoires, autorisant l'accès à des ressources protégées généralement restreintes par les ACL — tant que le processus possède les privilèges appropriés. Cette fonctionnalité n'est prise en charge que sur les systèmes d'exploitation Windows. Sur les plateformes non Windows, l'activation de cette propriété n'a aucun effet. Notez que cela nécessite que le processus s'exécute avec des droits administratifs. Utilisez avec prudence, car cela peut permettre l'accès à des fichiers système sensibles et aux données utilisateur.

### Voir aussi

* class [BaseOptions](../../baseoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
