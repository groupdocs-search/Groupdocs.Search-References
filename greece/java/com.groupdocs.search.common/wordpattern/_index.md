---
title: "WordPattern"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα πρότυπο λέξης για χρήση στην αναζήτηση μπαλαντέρ λέξεων."
type: docs
weight: 34
url: /el/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Αντιπροσωπεύει ένα πρότυπο λέξης για χρήση στην αναζήτηση μπαλαντέρ λέξεων.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Αρχικοποιεί μια νέα παρουσία της  WordPattern  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Προσθέτει μια συμβολοσειρά στο μοτίβο λέξης. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Προσθέτει έναν χαρακτήρα στο μοτίβο λέξης. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Προσθέτει ένα μπαλαντέρ ενός χαρακτήρα στο μοτίβο λέξης. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Προσθέτει ένα μπαλαντέρ μηδέν ή ενός χαρακτήρα στο μοτίβο λέξης. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Προσθέτει ένα μπαλαντέρ μηδέν ή περισσότερων χαρακτήρων στο μοτίβο λέξης. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Προσθέτει ένα μπαλαντέρ ενός ή περισσότερων χαρακτήρων στο μοτίβο λέξης. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Προσθέτει ένα μπαλαντέρ στο μοτίβο λέξης. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα  System.String  που αντιπροσωπεύει το τρέχον  WordPattern . |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Αρχικοποιεί μια νέα παρουσία της  WordPattern  κλάσης.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Προσθέτει μια συμβολοσειρά στο μοτίβο λέξης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | text | java.lang.String | Η συμβολοσειρά για προσθήκη. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Προσθέτει έναν χαρακτήρα στο μοτίβο λέξης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χαρακτήρας | char | Ο χαρακτήρας για προσθήκη. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Προσθέτει ένα μπαλαντέρ ενός χαρακτήρα στο μοτίβο λέξης.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Προσθέτει ένα μπαλαντέρ μηδέν ή ενός χαρακτήρα στο μοτίβο λέξης.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Προσθέτει ένα μπαλαντέρ μηδέν ή περισσότερων χαρακτήρων στο μοτίβο λέξης.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Προσθέτει ένα μπαλαντέρ ενός ή περισσότερων χαρακτήρων στο μοτίβο λέξης.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Προσθέτει ένα μπαλαντέρ στο μοτίβο λέξης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | min | int | Ο ελάχιστος αριθμός χαρακτήρων. |
|
|  | max | int | Ο μέγιστος αριθμός χαρακτήρων. |
|

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει ένα  System.String  που αντιπροσωπεύει το τρέχον  WordPattern .


**Returns:**
java.lang.String - Ένα  System.String  που αντιπροσωπεύει το τρέχον  WordPattern .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
