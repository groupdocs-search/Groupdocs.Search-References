---
title: "MulticastDelegate"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक डेलीगेट का प्रतिनिधित्व करता है जो क्लास इंस्टेंस को संदर्भित करता है जिनमें कॉल करने के लिए मेथड होता है।"
type: docs
weight: 26
url: /hi/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

एक डेलीगेट का प्रतिनिधित्व करता है, जो क्लास इंस्टेंस को संदर्भित करता है जिनमें कॉल करने के लिए मेथड है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | एक इनवोकेशन सूची लौटाता है। |
|
|  | [getDelegateId()](#getDelegateId--) | एक डेलीगेट आईडी लौटाता है। |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | दो डेलीगेट की समानता की जाँच करता है। |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | दो डेलीगेट की असमानता की जाँच करता है। |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


एक इनवोकेशन सूची लौटाता है।


**Returns:**
com.groupdocs.search.common.Delegate[] - एक इनवोकेशन सूची।

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


एक डेलीगेट आईडी लौटाता है।


**Returns:**
java.lang.String - एक डेलीगेट आईडी।

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


दो डेलीगेट की समानता की जाँच करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | पहला प्रतिनिधि। |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | दूसरा प्रतिनिधि। |
|

**Returns:**
boolean - दो प्रतिनिधियों की समानता की जाँच का परिणाम।

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


दो डेलीगेट की असमानता की जाँच करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | पहला प्रतिनिधि। |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | दूसरा प्रतिनिधि। |
|

**Returns:**
boolean - दो प्रतिनिधियों की असमानता की जाँच का परिणाम।

