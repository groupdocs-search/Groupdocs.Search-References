---
title: "Notifikasi"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Kelas dasar untuk semua notifikasi ke indeks."
type: docs
weight: 22
url: /id/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

Kelas dasar untuk semua notifikasi ke indeks. Kelas ini juga berisi metode untuk membuat objek notifikasi.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Notification()](#Notification--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Membuat objek notifikasi untuk mengganti nama dokumen terindeks yang telah diganti namanya dan tidak perlu diindeks ulang. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Membuat objek notifikasi untuk mengganti nama dokumen terindeks yang telah diganti namanya dan tidak perlu diindeks ulang. Dokumen yang telah diganti nama tidak akan diindeks ulang selama operasi pembaruan berikutnya, bahkan jika isinya telah berubah.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | oldPath | java.lang.String | Jalur lama ke dokumen terindeks. |
|
|  | newPath | java.lang.String | Jalur baru ke dokumen terindeks. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

