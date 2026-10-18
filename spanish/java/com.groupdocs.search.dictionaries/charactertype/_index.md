---
title: "CharacterType"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un tipo de carácter dependiendo de cómo debe indexarse."
type: docs
weight: 24
url: /es/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Representa un tipo de carácter, dependiendo de cómo debe indexarse.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Separator](#Separator) | El carácter separador. |
|
|  | [Letter](#Letter) | El carácter válido. |
|
|  | [Blended](#Blended) | Tanto el separador como el carácter válido. |
|
|  | [SeparateWord](#SeparateWord) | El carácter que representa una palabra completa. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


El carácter separador.


### Letter {#Letter}
```
public static final CharacterType Letter
```


El carácter válido.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Tanto el separador como el carácter válido.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


El carácter que representa una palabra completa.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
