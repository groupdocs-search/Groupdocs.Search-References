---
title: "HighlightOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bulunan terimleri vurgulamak için seçenekler sağlar."
type: docs
weight: 22
url: /tr/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Bulunan terimleri vurgulamak için seçenekler sağlar.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | HighlightOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | TextOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Vurgulanan kelime öncesindeki metin parçacığındaki maksimum kelime sayısını alır. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Vurgulanan kelime öncesindeki metin parçacığındaki maksimum kelime sayısını ayarlar. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Vurgulanan kelime sonrasındaki metin parçacığındaki maksimum kelime sayısını alır. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Vurgulanan kelime sonrasındaki metin parçacığındaki maksimum kelime sayısını ayarlar. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Metin parçacığındaki maksimum kelime sayısını alır. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Metin parçacığındaki maksimum kelime sayısını ayarlar. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Varlıkları vurgulamak için satır içi stillerin kullanılıp kullanılmadığını gösteren değeri alır. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Varlıkları vurgulamak için satır içi stillerin kullanılıp kullanılmadığını gösteren değeri ayarlar. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Varlıkları vurgulamak için kullanılan bir rengi alır. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Varlıkları vurgulamak için kullanılan bir rengi ayarlar. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Bulunan kelimenin vurgulanmasının başlangıç etiketini alır. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Bulunan kelimenin vurgulanmasının başlangıç etiketini ayarlar. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Bulunan kelimenin vurgulanmasının bitiş etiketini alır. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Bulunan kelimenin vurgulanmasının bitiş etiketini ayarlar. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


HighlightOptions sınıfının yeni bir örneğini başlatır.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


TextOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Vurgulanan kelimenin öncesindeki bir metin alıntısındaki maksimum kelime sayısını alır. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer 7'dir.


**Returns:**
int - Vurgulanan kelimenin öncesindeki bir metin alıntısındaki maksimum kelime sayısı.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Vurgulanan kelimenin öncesindeki bir metin alıntısındaki maksimum kelime sayısını ayarlar. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer 7'dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Vurgulanan kelimenin öncesindeki bir metin alıntısındaki maksimum kelime sayısı. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Vurgulanan kelimenin sonrasındaki bir metin alıntısındaki maksimum kelime sayısını alır. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer 7'dir.


**Returns:**
int - Vurgulanan kelimenin sonrasındaki bir metin alıntısındaki maksimum kelime sayısı.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Vurgulanan kelimenin sonrasındaki bir metin alıntısındaki maksimum kelime sayısını ayarlar. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer 7'dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Vurgulanan kelimenin sonrasındaki bir metin alıntısındaki maksimum kelime sayısı. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Bir metin alıntısındaki maksimum kelime sayısını alır. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer 21'dir.


**Returns:**
int - Bir metin alıntısındaki maksimum kelime sayısı.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Bir metin alıntısındaki maksimum kelime sayısını ayarlar. Değer 0 ile 10000 arasında olmalıdır. Varsayılan değer 21'dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Bir metin alıntısındaki maksimum kelime sayısı. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Olayların vurgulanması için satır içi stillerin kullanılıp kullanılmadığını gösteren bir değeri alır. Varsayılan değer true'dur.


**Returns:**
boolean - Olayların vurgulanması için satır içi stillerin kullanılıp kullanılmadığını gösteren bir değer.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Olayların vurgulanması için satır içi stillerin kullanılıp kullanılmadığını gösteren bir değeri ayarlar. Varsayılan değer true'dur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Olayların vurgulanması için satır içi stillerin kullanılıp kullanılmadığını gösteren bir değer. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Olayların vurgulanması için kullanılan bir rengi alır. Varsayılan değer #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Olayların vurgulanması için kullanılan bir rengi ayarlar. Varsayılan değer #FFD800.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Olayların vurgulanması için kullanılan bir renk. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Bulunan kelimenin vurgulanmasının başlangıç etiketini alır. Bu etiket yalnızca düz metinde vurgulama yapıldığında kullanılır. Varsayılan değer boş bir dizedir.


**Returns:**
java.lang.String - Bulunan kelimenin vurgulanmasının başlangıç etiketi.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Bulunan kelimenin vurgulanmasının başlangıç etiketini ayarlar. Bu etiket yalnızca düz metinde vurgulama yapıldığında kullanılır. Varsayılan değer boş bir dizedir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Bulunan kelimenin vurgulanmasının başlangıç etiketi. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Bulunan kelimenin vurgulanmasının bitiş etiketini alır. Bu etiket yalnızca düz metinde vurgulama yapıldığında kullanılır. Varsayılan değer boş bir dizedir.


**Returns:**
java.lang.String - Bulunan kelimenin vurgulanmasının bitiş etiketi.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Bulunan kelimenin vurgulanmasının son etiketini ayarlar. Bu etiket yalnızca düz metinde vurgulama yapıldığında kullanılır. Varsayılan değer boş bir dizedir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Bulunan kelimenin vurgulanmasının son etiketi. |
|

