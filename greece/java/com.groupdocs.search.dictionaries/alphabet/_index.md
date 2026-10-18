---
title: "Αλφάβητο"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού χαρακτήρων που χρησιμοποιείται κατά τη διάρκεια της ευρετηρίασης για την ανίχνευση του τύπου χαρακτήρα."
type: docs
weight: 15
url: /el/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Ορίζει τη διεπαφή ενός λεξικού χαρακτήρων που χρησιμοποιείται κατά την ευρετηρίαση για την ανίχνευση του τύπου χαρακτήρα. Κάθε χαρακτήρας μπορεί να αντιμετωπιστεί ως διαχωριστικό, ως γράμμα ή και τα δύο.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Λαμβάνει έναν τύπο χαρακτήρα. |
|
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των χαρακτήρων που περιέχονται στο Αλφάβητο. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Ορίζει τον τύπο για κάθε χαρακτήρα της συγκεκριμένης συλλογής σε αυτήν την περίπτωση του Αλφάβητου. |
|
|  | [clear()](#clear--) | Ορίζει τον τύπο CharacterType.Separator για όλους τους χαρακτήρες σε αυτό το Αλφάβητο. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Λαμβάνει έναν τύπο χαρακτήρα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χαρακτήρας | char | Ο χαρακτήρας για λήψη τύπου. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Λαμβάνει τον αριθμό των χαρακτήρων που περιέχονται στο Αλφάβητο.


**Returns:**
int - Ο αριθμός των χαρακτήρων στο λεξικό.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Ορίζει τον τύπο για κάθε χαρακτήρα της συγκεκριμένης συλλογής σε αυτήν την περίπτωση του Αλφάβητου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χαρακτήρες | char[] | Η συλλογή χαρακτήρων για ορισμό του τύπου. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Ο τύπος χαρακτήρα. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Ορίζει τον τύπο CharacterType.Separator για όλους τους χαρακτήρες σε αυτό το Αλφάβητο.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.Character> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

