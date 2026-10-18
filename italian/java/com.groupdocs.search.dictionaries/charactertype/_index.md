---
title: "CharacterType"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un tipo di carattere a seconda di come dovrebbe essere indicizzato."
type: docs
weight: 24
url: /it/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Rappresenta un tipo di carattere, a seconda di come dovrebbe essere indicizzato.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Separator](#Separator) | Il carattere separatore. |
|
|  | [Letter](#Letter) | Il carattere valido. |
|
|  | [Blended](#Blended) | Sia il separatore che il carattere valido. |
|
|  | [SeparateWord](#SeparateWord) | Il carattere che rappresenta una parola intera. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Il carattere separatore.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Il carattere valido.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Sia il separatore che il carattere valido.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Il carattere che rappresenta una parola intera.


### values() {#values--}
```
public static CharacterType[] values()
```




**Returns:**
com.groupdocs.search.dictionaries.CharacterType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static CharacterType valueOf(String name)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
