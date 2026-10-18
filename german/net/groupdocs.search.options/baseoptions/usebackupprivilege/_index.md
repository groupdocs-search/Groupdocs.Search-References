---
title: "UseBackupPrivilege"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Liest oder setzt einen Wert, der angibt, ob der Prozess das SeBackupPrivilege und FILE_FLAG_BACKUP_SEMANTICS zum Zugriff auf Dateien und Verzeichnisse verwenden soll. Der Standardwert ist false."
type: docs
weight: 70
url: /de/net/groupdocs.search.options/baseoptions/usebackupprivilege/
---
## BaseOptions.UseBackupPrivilege property

Liest oder setzt einen Wert, der angibt, ob der Prozess das SeBackupPrivilege und FILE_FLAG_BACKUP_SEMANTICS zum Zugriff auf Dateien und Verzeichnisse verwenden soll. Der Standardwert ist `false`.

```csharp
public bool UseBackupPrivilege { get; set; }
```

### Property Value

`true`, um privilegierten Zugriff mit SeBackupPrivilege und FILE_FLAG_BACKUP_SEMANTICS zu aktivieren; andernfalls `false`.

### Hinweise

Wenn aktiviert, ermöglicht dies dem Prozess, Datei- und Verzeichnis‑Sicherheitsprüfungen zu umgehen, wodurch Zugriff auf geschützte Ressourcen gewährt wird, die normalerweise durch ACLs eingeschränkt sind – sofern der Prozess die entsprechenden Berechtigungen besitzt. Diese Funktion wird nur unter Windows‑Betriebssystemen unterstützt. Auf Nicht‑Windows‑Plattformen hat das Aktivieren dieser Eigenschaft keine Wirkung. Beachten Sie, dass dafür der Prozess mit administrativen Rechten ausgeführt werden muss. Verwenden Sie dies mit Vorsicht, da es Zugriff auf sensible Systemdateien und Benutzerdaten ermöglichen kann.

### Siehe auch

* class [BaseOptions](../../baseoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
