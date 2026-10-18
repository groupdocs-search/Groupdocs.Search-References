---
title: "PasswordRequiredEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa yang terjadi ketika dokumen yang dilindungi kata sandi sedang diindeks."
type: docs
weight: 20
url: /id/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa yang terjadi ketika dokumen yang dilindungi kata sandi sedang diindeks.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Mendapatkan jalur lengkap dokumen. |
|
|  | [getPassword()](#getPassword--) | Mendapatkan kata sandi untuk membuka dokumen. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Menetapkan kata sandi untuk membuka dokumen. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Mendapatkan jalur lengkap dokumen.


**Returns:**
java.lang.String - Jalur lengkap dokumen.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Mendapatkan kata sandi untuk membuka dokumen.


**Returns:**
java.lang.String - Kata sandi untuk membuka dokumen.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Menetapkan kata sandi untuk membuka dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Kata sandi untuk membuka dokumen. |
|

