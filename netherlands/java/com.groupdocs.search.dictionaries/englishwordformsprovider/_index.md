---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een provider van Engelse woordvormen voor."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Stelt een provider van Engelse woordvormen voor.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Initialiseert een nieuw exemplaar van de |
EnglishWordFormsProvider
klasse.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Haalt de woordvormen op voor het opgegeven woord. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Initialiseert een nieuw exemplaar van de
EnglishWordFormsProvider
klasse.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Haalt de woordvormen op voor het opgegeven woord.
De resulterende array bevat het oorspronkelijke woord niet.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woord | java.lang.String | Het woord om de woordvormen voor te suggereren. |
|

**Returns:**
java.lang.String[] - De woordvormen voor het opgegeven woord of een lege array als de  IWordFormsProvider  geen woordvormen levert voor het opgegeven woord.

