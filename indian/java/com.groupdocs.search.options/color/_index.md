---
title: "Color"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक ARGB (अल्फा, रेड, ग्रीन, ब्लू) रंग का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

ARGB (अल्फा, लाल, हरा, नीला) रंग को दर्शाता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Color क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Color क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Color क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | इस इंस्टेंस का अल्फा घटक मान प्राप्त करता है। |
|
|  | [getRed()](#getRed--) | इस उदाहरण का लाल घटक मान प्राप्त करता है। |
|
|  | [getGreen()](#getGreen--) | इस उदाहरण का हरा घटक मान प्राप्त करता है। |
|
|  | [getBlue()](#getBlue--) | इस उदाहरण का नीला घटक मान प्राप्त करता है। |
|
|  | [toString()](#toString--) | वर्तमान  Color  को दर्शाने वाली  String  लौटाता है। |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Color क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | अल्फा | int | 0 से 255 तक का अल्फा घटक। |
|
|  | लाल | int | 0 से 255 तक का लाल घटक। |
|
|  | हरा | int | 0 से 255 तक का हरा घटक। |
|
|  | नीला | int | 0 से 255 तक का नीला घटक। |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Color क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | लाल | int | 0 से 255 तक का लाल घटक। |
|
|  | हरा | int | 0 से 255 तक का हरा घटक। |
|
|  | नीला | int | 0 से 255 तक का नीला घटक। |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Color क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


इस इंस्टेंस का अल्फा घटक मान प्राप्त करता है।


**Returns:**
int - इस उदाहरण का अल्फा घटक मान।

### getRed() {#getRed--}
```
public int getRed()
```


इस उदाहरण का लाल घटक मान प्राप्त करता है।


**Returns:**
int - इस उदाहरण का लाल घटक मान।

### getGreen() {#getGreen--}
```
public int getGreen()
```


इस उदाहरण का हरा घटक मान प्राप्त करता है।


**Returns:**
int - इस उदाहरण का हरा घटक मान।

### getBlue() {#getBlue--}
```
public int getBlue()
```


इस उदाहरण का नीला घटक मान प्राप्त करता है।


**Returns:**
int - इस उदाहरण का नीला घटक मान।

### toString() {#toString--}
```
public String toString()
```


वर्तमान  Color  को दर्शाने वाली  String  लौटाता है।


**Returns:**
java.lang.String - वर्तमान  Color  को दर्शाने वाली  String ।

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
