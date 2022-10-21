---
title: Metered
second_title: GroupDocs.Search for Java API Reference
description: Provides methods to set metered key.
type: docs
weight: 11
url: /java/com.groupdocs.search.licensing/metered/
---
**Inheritance:**
java.lang.Object, com.groupdocs.search.MeteredAssistant
```
public class Metered extends MeteredAssistant
```

Provides methods to set metered key.

**Learn more**

 *  [Evaluation Limitations and Licensing][]

The example demonstrates a typical usage of the class.

```

```

try \{ Metered metered = new Metered(); metered.setMeteredKey("PublicKey", "PrivateKey"); \} catch (java.lang.Exception ex) \{ // ... \}


[Evaluation Limitations and Licensing]: https://docs.groupdocs.com/display/searchjava/Evaluation+Limitations+and+Licensing
## Constructors

| Constructor | Description |
| --- | --- |
| [Metered()](#Metered--) | Initializes a new instance of this class. |
## Methods

| Method | Description |
| --- | --- |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Sets metered public and private key |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Gets consumption file size |
| [getConsumptionCredit()](#getConsumptionCredit--) | Gets consumption credit |
### Metered() {#Metered--}
```
public Metered()
```


Initializes a new instance of this class.

### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public void setMeteredKey(String publicKey, String privateKey)
```


Sets metered public and private key

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | public key |
| privateKey | java.lang.String | private key |

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Gets consumption file size

**Returns:**
double - consumption quantity
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Gets consumption credit

**Returns:**
double - consumption quantity
