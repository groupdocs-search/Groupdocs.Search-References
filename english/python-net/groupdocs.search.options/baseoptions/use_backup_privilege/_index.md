---
title: use_backup_privilege property
second_title: GroupDocs.Search for Python via .NET API References
description: "The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories."
type: docs
url: /python-net/groupdocs.search.options/baseoptions/use_backup_privilege/
is_root: false
weight: 2060
---


## use_backup_privilege property

The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False.

When enabled, this allows the process to bypass file and directory security checks, permitting access to protected resources typically restricted by ACLs — as long as the process has the proper privileges.

This feature is only supported on Windows operating systems. On non-Windows platforms, enabling this property has no effect.

Note that this requires the process to be running with administrative rights.

Use with caution, as it may allow access to sensitive system files and user data.

### Definition:
```python
@property
def use_backup_privilege(self):
    ...
@use_backup_privilege.setter
def use_backup_privilege(self, value):
    ...
```

### See Also
* class [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)
