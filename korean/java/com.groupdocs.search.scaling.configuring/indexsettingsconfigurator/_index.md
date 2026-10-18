---
title: "IndexSettingsConfigurator"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크의 각 샤드에 대한 인덱스 설정 구성자를 나타냅니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

검색 네트워크의 각 샤드에 대한 인덱스 설정 구성자를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | 불용어 사용 플래그를 설정합니다. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | 문자 교체 사용 플래그를 설정합니다. |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | 텍스트 저장 설정을 설정합니다. |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | 인덱스 유형을 설정합니다. |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | 검색 스레드 수를 설정합니다. |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | 인덱스 설정 구성을 완료합니다. |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


불용어 사용 플래그를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 플래그 값입니다. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


문자 교체 사용 플래그를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 플래그 값입니다. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


텍스트 저장 설정을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | isUsed | boolean | 인덱스에서 텍스트 저장소 사용 플래그입니다. |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | 압축 수준. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


인덱스 유형을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | 인덱스 유형. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


검색 스레드 수를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | 검색 스레드 수. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


인덱스 설정 구성을 완료합니다.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

