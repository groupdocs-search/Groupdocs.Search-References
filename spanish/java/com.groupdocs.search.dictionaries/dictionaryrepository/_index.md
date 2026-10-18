---
title: "DictionaryRepository"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un repositorio de todos los diccionarios en el Índice."
type: docs
weight: 12
url: /es/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Representa un repositorio de todos los diccionarios en el Índice.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Obtiene un diccionario de alias. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Obtiene un diccionario de palabras vacías. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Obtiene un diccionario de sinónimos. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Obtiene un diccionario de contraseñas de documentos. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Obtiene un corrector ortográfico. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Obtiene un diccionario de homófonos. |
|
|  | [getAlphabet()](#getAlphabet--) | Obtiene un diccionario de caracteres. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Obtiene un diccionario de reemplazos de caracteres. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Obtiene un proveedor de formas de palabras. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Establece un proveedor de formas de palabras. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Obtiene un diccionario de alias.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Obtiene un diccionario de palabras vacías.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Obtiene un diccionario de sinónimos.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Obtiene un diccionario de contraseñas de documentos.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Obtiene un corrector ortográfico.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Obtiene un diccionario de homófonos.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Obtiene un diccionario de caracteres.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Obtiene un diccionario de reemplazos de caracteres.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Obtiene un proveedor de formas de palabras.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Establece un proveedor de formas de palabras.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Un proveedor de formas de palabras. |
|

