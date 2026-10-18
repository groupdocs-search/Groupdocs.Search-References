---
title: "Delegate"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक डेलीगेट का प्रतिनिधित्व करता है जो ऐसी क्लास इंस्टेंस को संदर्भित करता है जिसमें बुलाए जाने वाला मेथड होता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

एक डेलीगेट का प्रतिनिधित्व करता है, जो एक क्लास इंस्टेंस को संदर्भित करता है जिसमें कॉल करने के लिए एक मेथड है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | एक इनवोकेशन सूची लौटाता है। |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | दो डेलीगेट को एक में संयोजित करता है। |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | कई डेलीगेट को एक में संयोजित करता है। |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | स्रोत डेलीगेट से वैल्यू डेलीगेट को हटाता है। |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | स्रोत डेलीगेट से वैल्यू डेलीगेट को हटाता है। |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | दो डेलीगेट की समानता की जाँच करता है। |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | दो डेलीगेट की असमानता की जाँच करता है। |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


एक इनवोकेशन सूची लौटाता है।


**Returns:**
com.groupdocs.search.common.Delegate[] - एक इनवोकेशन सूची।

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


दो डेलीगेट को एक में संयोजित करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | संयोजित करने के लिए पहला डेलीगेट। |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | संयोजन के लिए दूसरा प्रतिनिधि। |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


कई डेलीगेट को एक में संयोजित करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | संयोजन के लिए प्रतिनिधि। |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


स्रोत डेलीगेट से वैल्यू डेलीगेट को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | स्रोत प्रतिनिधि। |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | मान प्रतिनिधि। |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


स्रोत डेलीगेट से वैल्यू डेलीगेट को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | स्रोत प्रतिनिधि। |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | मान प्रतिनिधि। |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


दो डेलीगेट की समानता की जाँच करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | पहला प्रतिनिधि। |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | दूसरा प्रतिनिधि। |
|

**Returns:**
boolean - दो प्रतिनिधियों की समानता की जाँच का परिणाम।

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


दो डेलीगेट की असमानता की जाँच करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | पहला प्रतिनिधि। |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | दूसरा प्रतिनिधि। |
|

**Returns:**
boolean - दो प्रतिनिधियों की असमानता की जाँच का परिणाम।

