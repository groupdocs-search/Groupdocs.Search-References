---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 메타데이터 필드에 대한 옵션을 제공합니다."
type: docs
weight: 29
url: /ko/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

인덱싱 메타데이터 필드에 대한 옵션을 제공합니다.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | 빈 필드 값을 인덱싱할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | 빈 필드 값을 인덱싱할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | 빈 필드 이름을 인덱싱할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | 빈 필드 이름을 인덱싱할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | 빈 필드 이름을 인덱싱하는 데 사용되는 기본 필드 이름을 가져옵니다. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | 빈 필드 이름을 인덱싱하는 데 사용되는 기본 필드 이름을 설정합니다. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | 필드의 복합 이름에 사용되는 구분자를 가져옵니다. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | 필드의 복합 이름에 사용되는 구분자를 설정합니다. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | 필드를 인덱싱하기 위해 byte 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | 필드를 인덱싱하기 위해 byte 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | 필드를 인덱싱하기 위해 int 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | 필드를 인덱싱하기 위해 int 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | 필드를 인덱싱하기 위해 long 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | 필드를 인덱싱하기 위해 long 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | 필드를 인덱싱하기 위해 double 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | 필드를 인덱싱하기 위해 double 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | 배열 유형 필드에서 값들 사이의 구분자를 가져옵니다. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | 배열 유형 필드에서 값들 사이의 구분자를 설정합니다. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


빈 필드 값을 인덱싱할지 여부를 나타내는 값을 가져옵니다. 기본값은 true 입니다.


**Returns:**
boolean - 빈 필드 값을 인덱싱할지 여부를 나타내는 값.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


빈 필드 값을 인덱싱할지 여부를 나타내는 값을 설정합니다. 기본값은 true 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 빈 필드 값을 인덱싱할지 여부를 나타내는 값입니다. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


빈 필드 이름을 인덱싱할지 여부를 나타내는 값을 가져옵니다. 기본값은 true 입니다.


**Returns:**
boolean - 빈 필드 이름을 인덱싱할지 여부를 나타내는 값입니다.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


빈 필드 이름을 인덱싱할지 여부를 나타내는 값을 설정합니다. 기본값은 true 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 빈 필드 이름을 인덱싱할지 여부를 나타내는 값입니다. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


빈 필드 이름을 인덱싱하는 데 사용되는 기본 필드 이름을 가져옵니다. 기본값은 "unknown" 입니다.


**Returns:**
java.lang.String - 빈 필드 이름을 인덱싱하는 데 사용되는 기본 필드 이름입니다.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


빈 필드 이름을 인덱싱하는 데 사용되는 기본 필드 이름을 설정합니다. 기본값은 "unknown" 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 빈 필드 이름을 인덱싱하는 데 사용되는 기본 필드 이름입니다. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


필드의 복합 이름에 사용되는 구분자를 가져옵니다. 기본값은 "." 입니다.


**Returns:**
java.lang.String - 필드의 복합 이름에 사용되는 구분자입니다.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


필드의 복합 이름에 사용되는 구분자를 설정합니다. 기본값은 "." 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 필드의 복합 이름에 사용되는 구분자입니다. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


필드를 인덱싱하기 위해 byte 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. 기본값은 Integer.MAX_VALUE 입니다.


**Returns:**
int - byte 유형 배열에 포함될 수 있는 최대 값 개수입니다.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


필드를 인덱싱하기 위해 byte 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. 기본값은 Integer.MAX_VALUE 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | byte 유형 배열에 포함될 수 있는 최대 값 개수입니다. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


필드를 인덱싱하기 위해 int 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. 기본값은 Integer.MAX_VALUE 입니다.


**Returns:**
int - int 유형 배열에 포함될 수 있는 최대 값 개수입니다.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


필드를 인덱싱하기 위해 int 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. 기본값은 Integer.MAX_VALUE 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | int 유형 배열에 포함될 수 있는 최대 값 개수입니다. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


필드를 인덱싱하기 위해 long 유형 배열에 포함될 수 있는 최대 값 개수를 가져옵니다. 기본값은 Integer.MAX_VALUE 입니다.


**Returns:**
int - long 유형 배열에 포함될 수 있는 최대 값 개수입니다.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


필드를 인덱싱하기 위해 long 유형 배열에 포함될 수 있는 최대 값 개수를 설정합니다. 기본값은 Integer.MAX_VALUE 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 필드를 인덱싱하기 위해 long 유형 배열의 최대 값 개수입니다. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


필드를 인덱싱하기 위해 double 유형 배열의 최대 값 개수를 가져옵니다. 기본값은 Integer.MAX_VALUE 입니다.


**Returns:**
int - 필드를 인덱싱하기 위한 double 유형 배열의 최대 값 개수.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


필드를 인덱싱하기 위해 double 유형 배열의 최대 값 개수를 설정합니다. 기본값은 Integer.MAX_VALUE 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 필드를 인덱싱하기 위한 double 유형 배열의 최대 값 개수. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


배열 유형 필드에서 값 사이의 구분자를 가져옵니다. 기본값은 공백 문자입니다.


**Returns:**
java.lang.String - 배열 유형 필드에서 값 사이의 구분자.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


배열 유형 필드에서 값 사이의 구분자를 설정합니다. 기본값은 공백 문자입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 배열 유형 필드에서 값 사이의 구분자. |
|

