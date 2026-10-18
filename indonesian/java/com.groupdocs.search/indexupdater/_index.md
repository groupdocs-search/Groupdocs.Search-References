---
title: "IndexUpdater"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili pembaruan indeks."
type: docs
weight: 20
url: /id/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Mewakili pembaruan indeks. Kelas ini melakukan pengindeksan ulang dokumen dalam indeks versi lama.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String sourceIndexFolder = "c:\\MyOldIndex\\";
String targetIndexFolder = "c:\\MyNewIndex\\";
IndexUpdater updater = new IndexUpdater();
if (updater.canUpdateVersion(sourceIndexFolder)) {
int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
}
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Menginisialisasi instance baru dari kelas  IndexUpdater  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Memeriksa apakah direktori yang ditentukan berisi indeks versi terbaru. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Memeriksa apakah indeks dalam direktori yang ditentukan dapat diperbarui ke versi terbaru. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Melakukan pengindeksan ulang dokumen dalam indeks versi lama. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Menginisialisasi instance baru dari kelas  IndexUpdater  .


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Memeriksa apakah direktori yang ditentukan berisi indeks versi terbaru.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexPath | java.lang.String | Jalur direktori indeks. |
|

**Returns:**
boolean -  true  jika direktori yang ditentukan berisi indeks versi terbaru; jika tidak  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Memeriksa apakah indeks dalam direktori yang ditentukan dapat diperbarui ke versi terbaru.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexPath | java.lang.String | Jalur direktori indeks. |
|

**Returns:**
boolean -  true  jika indeks dalam direktori yang ditentukan dapat diperbarui ke versi terbaru; jika tidak  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Melakukan pengindeksan ulang dokumen dalam indeks versi lama. Indeks yang diperbarui akan ditempatkan di direktori  newIndexPath . Indeks di direktori  indexPath  tidak akan diubah.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexPath | java.lang.String | Jalur direktori indeks. |
|
|  | newIndexPath | java.lang.String | Direktori untuk indeks yang diperbarui. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

