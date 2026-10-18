---
title: "WordPattern"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Kelime joker karakter aramasında kullanılacak bir kelime desenini temsil eder."
type: docs
weight: 34
url: /tr/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Kelime joker karakter aramasında kullanılacak bir kelime desenini temsil eder.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | WordPattern sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Bir dizeyi kelime desenine ekler. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Bir karakteri kelime desenine ekler. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Kelime desenine tek karakter joker karakteri ekler. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Kelime desenine sıfır veya bir karakter joker karakteri ekler. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Kelime desenine sıfır veya daha fazla karakter joker karakteri ekler. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Kelime desenine bir veya daha fazla karakter joker karakteri ekler. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Kelime desenine bir joker karakter ekler. |
|
|  | [toString()](#toString--) | Geçerli WordPattern'ı temsil eden bir System.String döndürür. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


WordPattern sınıfının yeni bir örneğini başlatır.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Bir dizeyi kelime desenine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | metin | java.lang.String | Eklenecek dize. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Bir karakteri kelime desenine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | karakter | char | Eklenecek karakter. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Kelime desenine tek karakter joker karakteri ekler.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Kelime desenine sıfır veya bir karakter joker karakteri ekler.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Kelime desenine sıfır veya daha fazla karakter joker karakteri ekler.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Kelime desenine bir veya daha fazla karakter joker karakteri ekler.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Kelime desenine bir joker karakter ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | min | int | Minimum karakter sayısı. |
|
|  | max | int | Maksimum karakter sayısı. |
|

### toString() {#toString--}
```
public String toString()
```


Geçerli WordPattern'ı temsil eden bir System.String döndürür.


**Returns:**
java.lang.String - Geçerli WordPattern'i temsil eden bir System.String.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
