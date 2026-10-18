---
title: "OperationFinishedEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika operasi pengindeksan selesai."
type: docs
weight: 17
url: /id/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa ketika operasi pengindeksan selesai.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getMessage()](#getMessage--) | Mendapatkan pesan. |
|
|  | [getOperationType()](#getOperationType--) | Mendapatkan tipe operasi. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Mendapatkan pesan.


**Returns:**
java.lang.String - Pesan.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Mendapatkan tipe operasi.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

