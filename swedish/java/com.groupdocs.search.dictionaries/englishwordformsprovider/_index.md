---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en leverantör av engelska ordformer."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Representerar en leverantör av engelska ordformer.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Initierar en ny instans av |
EnglishWordFormsProvider
klassen.
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Hämtar ordformer för det angivna ordet. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Initierar en ny instans av
EnglishWordFormsProvider
klassen.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Hämtar ordformer för det angivna ordet.
Den resulterande arrayen innehåller inte det ursprungliga ordet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String | Ordet för att föreslå ordformer. |
|

**Returns:**
java.lang.String[] - Ordformerna för det angivna ordet eller en tom array om  IWordFormsProvider  inte tillhandahåller ordformer för det angivna ordet.

