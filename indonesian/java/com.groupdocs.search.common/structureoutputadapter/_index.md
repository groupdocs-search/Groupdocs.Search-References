---
title: "StructureOutputAdapter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili adaptor output yang mengumpulkan output sebagai struktur yang berisi setiap bidang secara terpisah."
type: docs
weight: 33
url: /id/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Mewakili adaptor output yang mengumpulkan output sebagai struktur yang berisi setiap bidang secara terpisah.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Menginisialisasi instance baru dari kelas StructureOutputAdapter. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getResult()](#getResult--) | Mendapatkan array bidang yang dihasilkan. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Menginisialisasi instance baru dari kelas StructureOutputAdapter.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Format output. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Mendapatkan array bidang yang dihasilkan.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Array bidang yang dihasilkan.

