---
title: "DictionaryRepository"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un référentiel de tous les dictionnaires dans l'Index."
type: docs
weight: 12
url: /fr/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Représente un référentiel de tous les dictionnaires dans l'Index.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Obtient un dictionnaire d'alias. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Obtient un dictionnaire de mots vides. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Obtient un dictionnaire de synonymes. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Obtient un dictionnaire de mots de passe de documents. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Obtient un correcteur orthographique. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Obtient un dictionnaire d'homophones. |
|
|  | [getAlphabet()](#getAlphabet--) | Obtient un dictionnaire de caractères. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Obtient un dictionnaire de remplacements de caractères. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Obtient un fournisseur de formes de mots. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Définit un fournisseur de formes de mots. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Obtient un dictionnaire d'alias.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Obtient un dictionnaire de mots vides.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Obtient un dictionnaire de synonymes.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Obtient un dictionnaire de mots de passe de documents.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Obtient un correcteur orthographique.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Obtient un dictionnaire d'homophones.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Obtient un dictionnaire de caractères.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Obtient un dictionnaire de remplacements de caractères.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Obtient un fournisseur de formes de mots.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Définit un fournisseur de formes de mots.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Un fournisseur de formes de mots. |
|

