---
title: "EnglishWordFormsProvider"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un proveedor de formas de palabras en inglés."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Representa un proveedor de formas de palabras en inglés.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Inicializa una nueva instancia de la |
EnglishWordFormsProvider
clase.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Obtiene las formas de la palabra especificada. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Inicializa una nueva instancia de la
EnglishWordFormsProvider
clase.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Obtiene las formas de la palabra especificada.
La matriz resultante no contiene la palabra original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabra | java.lang.String | La palabra para sugerir las formas de la palabra. |
|

**Returns:**
java.lang.String[] - Las formas de la palabra especificada o una matriz vacía si el  IWordFormsProvider  no proporciona formas de la palabra para la palabra especificada.

