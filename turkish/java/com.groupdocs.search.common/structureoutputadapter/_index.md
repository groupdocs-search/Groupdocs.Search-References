---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Çıktıyı her alanı ayrı ayrı içeren bir yapı olarak toplayan bir çıktı adaptörünü temsil eder."
type: docs
weight: 33
url: /tr/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Çıktıyı her alanı ayrı ayrı içeren bir yapı olarak toplayan bir çıktı adaptörünü temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StructureOutputAdapter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getResult()](#getResult--) | Sonuçta oluşan alanlar dizisini alır. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


StructureOutputAdapter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Çıktı biçimi. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Sonuçta oluşan alanlar dizisini alır.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Sonuçta oluşan alanlar dizisi.

