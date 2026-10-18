---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İngilizce kelime biçimleri sağlayıcısını temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

İngilizce kelime biçimleri sağlayıcısını temsil eder.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Yeni bir örnek başlatır |
EnglishWordFormsProvider
sınıf.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Belirtilen kelime için kelime biçimlerini alır. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Yeni bir örnek başlatır
EnglishWordFormsProvider
sınıf.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Belirtilen kelime için kelime biçimlerini alır.
Sonuç dizisi orijinal kelimeyi içermez.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelime | java.lang.String | Kelime biçimlerini önermek için kelime. |
|

**Returns:**
java.lang.String[] - Belirtilen kelime için sözcük biçimleri veya IWordFormsProvider belirtilen kelime için sözcük biçimi sağlamıyorsa boş dizi.

