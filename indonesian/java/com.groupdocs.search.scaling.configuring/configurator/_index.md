---
title: "Configurator"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili konfigurator jaringan pencarian."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Mewakili konfigurator jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Configurator()](#Configurator--) | Menginisialisasi instance baru dari kelas Configurator. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Memulai konfigurasi pengaturan indeks untuk setiap shard dalam jaringan pencarian. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Menambahkan node ke konfigurasi jaringan pencarian. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Menyelesaikan proses konfigurasi dan mengembalikan instance dari konfigurasi jaringan pencarian. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Menginisialisasi instance baru dari kelas Configurator.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Memulai konfigurasi pengaturan indeks untuk setiap shard dalam jaringan pencarian.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Menambahkan node ke konfigurasi jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nodeIndex | int | Indeks node. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Menyelesaikan proses konfigurasi dan mengembalikan instance dari konfigurasi jaringan pencarian.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
