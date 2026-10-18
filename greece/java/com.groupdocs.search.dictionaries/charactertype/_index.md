---
title: "CharacterType"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν τύπο χαρακτήρα ανάλογα με το πώς πρέπει να ευρετηριαστεί."
type: docs
weight: 24
url: /el/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Αναπαριστά έναν τύπο χαρακτήρα, ανάλογα με το πώς πρέπει να ευρετηριαστεί.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Separator](#Separator) | Ο χαρακτήρας διαχωρισμού. |
|
|  | [Letter](#Letter) | Ο έγκυρος χαρακτήρας. |
|
|  | [Blended](#Blended) | Τόσο ο διαχωριστής όσο και ο έγκυρος χαρακτήρας. |
|
|  | [SeparateWord](#SeparateWord) | Ο χαρακτήρας που αντιπροσωπεύει μια ολόκληρη λέξη. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Ο χαρακτήρας διαχωρισμού.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Ο έγκυρος χαρακτήρας.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Τόσο ο διαχωριστής όσο και ο έγκυρος χαρακτήρας.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Ο χαρακτήρας που αντιπροσωπεύει μια ολόκληρη λέξη.


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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
