---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Şifreyle korunan belgenin indekslendiği durumda gerçekleşen olayın argümanlarını temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Şifreyle korunan belgenin indekslendiği durumda gerçekleşen olayın argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Belgenin tam yolunu alır. |
|
|  | [getPassword()](#getPassword--) | Belgeyi açmak için şifreyi alır. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Belgeyi açmak için şifreyi ayarlar. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Belgenin tam yolunu alır.


**Returns:**
java.lang.String - Belgenin tam yolu.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Belgeyi açmak için şifreyi alır.


**Returns:**
java.lang.String - Belgeyi açmak için şifre.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Belgeyi açmak için şifreyi ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Belgeyi açmak için şifre. |
|

