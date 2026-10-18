---
title: "CharacterType"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक अक्षर के प्रकार को दर्शाता है जो इस पर निर्भर करता है कि उसे कैसे अनुक्रमित किया जाना चाहिए।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

एक अक्षर के प्रकार को दर्शाता है, यह इस पर निर्भर करता है कि इसे कैसे अनुक्रमित किया जाना चाहिए।

## Fields

| Field | विवरण |
| --- | --- |
|  | [Separator](#Separator) | विभाजक अक्षर। |
|
|  | [Letter](#Letter) | वैध अक्षर। |
|
|  | [Blended](#Blended) | विभाजक और वैध दोनों अक्षर। |
|
|  | [SeparateWord](#SeparateWord) | वह अक्षर जो पूरे शब्द का प्रतिनिधित्व करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


विभाजक अक्षर।


### Letter {#Letter}
```
public static final CharacterType Letter
```


वैध अक्षर।


### Blended {#Blended}
```
public static final CharacterType Blended
```


विभाजक और वैध दोनों अक्षर।


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


वह अक्षर जो पूरे शब्द का प्रतिनिधित्व करता है।


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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
