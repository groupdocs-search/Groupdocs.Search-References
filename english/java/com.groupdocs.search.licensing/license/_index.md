---
title: License
second_title: GroupDocs.Search for Java API Reference
description: Represents the component license.
type: docs
weight: 10
url: /java/com.groupdocs.search.licensing/license/
---
**Inheritance:**
java.lang.Object, com.groupdocs.search.LicenseAssistant
```
public final class License extends LicenseAssistant
```

Represents the component license.

**Learn more**

 *  [Evaluation Limitations and Licensing][]

The example demonstrates how to setup license.

```

 License license = new License();
 license.setLicense("C:\\License.lic");
 
```


[Evaluation Limitations and Licensing]: https://docs.groupdocs.com/display/searchjava/Evaluation+Limitations+and+Licensing
## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initializes a new instance of the  License  class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(String filePath)](#setLicense-java.lang.String-) | Licenses the component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenses the component. |
### License() {#License--}
```
public License()
```


Initializes a new instance of the  License  class.

### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Absolute path to license file. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | License stream. |

