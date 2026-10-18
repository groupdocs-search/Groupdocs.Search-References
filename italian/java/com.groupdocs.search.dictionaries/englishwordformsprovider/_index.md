---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un provider di forme di parole inglesi."
type: docs
weight: 13
url: /it/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Rappresenta un provider di forme di parole inglesi.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Inizializza una nuova istanza di |
EnglishWordFormsProvider
classe.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Ottiene le forme della parola per la parola specificata. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Inizializza una nuova istanza di
EnglishWordFormsProvider
classe.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Ottiene le forme della parola per la parola specificata.
L'array risultante non contiene la parola originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola | java.lang.String | La parola per suggerire le forme della parola. |
|

**Returns:**
java.lang.String[] - Le forme della parola per la parola specificata o array vuoto se l IWordFormsProvider non fornisce forme della parola per la parola specificata.

