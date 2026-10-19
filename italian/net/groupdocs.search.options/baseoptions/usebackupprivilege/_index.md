---
title: "UseBackupPrivilege"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene o imposta un valore che indica se il processo deve utilizzare SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS per accedere a file e directory. Il valore predefinito è false."
type: docs
weight: 70
url: /it/net/groupdocs.search.options/baseoptions/usebackupprivilege/
---
## BaseOptions.UseBackupPrivilege property

Ottiene o imposta un valore che indica se il processo deve utilizzare SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS per accedere a file e directory. Il valore predefinito è `false`.

```csharp
public bool UseBackupPrivilege { get; set; }
```

### Property Value

`true` per abilitare l'accesso privilegiato usando SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS; altrimenti, `false`.

### Osservazioni

Quando abilitato, consente al processo di bypassare i controlli di sicurezza su file e directory, permettendo l'accesso a risorse protette tipicamente limitate dagli ACL — purché il processo disponga dei privilegi appropriati. Questa funzionalità è supportata solo sui sistemi operativi Windows. Su piattaforme non Windows, l'abilitazione di questa proprietà non ha effetto. Nota che ciò richiede che il processo sia in esecuzione con diritti amministrativi. Usare con cautela, poiché potrebbe consentire l'accesso a file di sistema sensibili e dati utente.

### Vedi anche

* class [BaseOptions](../../baseoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
