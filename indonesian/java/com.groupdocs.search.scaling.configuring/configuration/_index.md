---
title: "Configuration"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili konfigurasi jaringan pencarian."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Mewakili konfigurasi jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Menyimpan konfigurasi ini ke sebuah file. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Menyimpan konfigurasi ini ke sebuah aliran. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Memuat konfigurasi jaringan pencarian dari sebuah file. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Memuat konfigurasi jaringan pencarian dari sebuah aliran. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Menyimpan konfigurasi ini ke sebuah file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | File untuk disimpan. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Menyimpan konfigurasi ini ke sebuah aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Aliran untuk disimpan. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Memuat konfigurasi jaringan pencarian dari sebuah file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | File untuk dimuat. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Memuat konfigurasi jaringan pencarian dari sebuah aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Aliran untuk dimuat dari. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

