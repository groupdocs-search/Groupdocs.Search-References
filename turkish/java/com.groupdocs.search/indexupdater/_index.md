---
title: "IndexUpdater"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir indeks güncelleyiciyi temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Bir indeks güncelleyiciyi temsil eder. Bu sınıf, eski bir sürümün indeksindeki belgeleri yeniden indeksler.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Örnek, sınıfın tipik bir kullanımını gösterir.

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


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | IndexUpdater sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Belirtilen dizinin en son sürümde bir indeks içerip içermediğini kontrol eder. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Belirtilen dizindeki bir indeksin en son sürüme güncellenip güncellenemeyeceğini kontrol eder. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Eski bir sürümdeki indeksteki belgelerin yeniden indekslenmesini gerçekleştirir. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


IndexUpdater sınıfının yeni bir örneğini başlatır.


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Belirtilen dizinin en son sürümde bir indeks içerip içermediğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexPath | java.lang.String | İndeks dizini yolu. |
|

**Returns:**
boolean -  true  eğer belirtilen dizin en son sürümde bir indeks içeriyorsa; aksi takdirde  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Belirtilen dizindeki bir indeksin en son sürüme güncellenip güncellenemeyeceğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexPath | java.lang.String | İndeks dizini yolu. |
|

**Returns:**
boolean -  true  eğer belirtilen dizindeki bir indeks en son sürüme güncellenebiliyorsa; aksi takdirde  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Eski bir sürümdeki indeksteki belgelerin yeniden indekslenmesini gerçekleştirir. Güncellenen indeks,  newIndexPath  dizinine yerleştirilecektir.  indexPath  dizinindeki indeks değiştirilmeyecektir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexPath | java.lang.String | İndeks dizini yolu. |
|
|  | newIndexPath | java.lang.String | Güncellenen indeks için dizin. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

