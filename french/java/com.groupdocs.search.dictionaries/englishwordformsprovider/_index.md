---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un fournisseur de formes de mots anglais."
type: docs
weight: 13
url: /fr/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Représente un fournisseur de formes de mots anglais.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Initialise une nouvelle instance de la |
EnglishWordFormsProvider
classe.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Récupère les formes du mot spécifié. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Initialise une nouvelle instance de la
EnglishWordFormsProvider
classe.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Récupère les formes du mot spécifié.
Le tableau résultant ne contient pas le mot original.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mot | java.lang.String | Le mot pour suggérer les formes du mot. |
|

**Returns:**
java.lang.String[] - Les formes du mot spécifié ou tableau vide si le IWordFormsProvider ne fournit pas de formes du mot pour le mot spécifié.

