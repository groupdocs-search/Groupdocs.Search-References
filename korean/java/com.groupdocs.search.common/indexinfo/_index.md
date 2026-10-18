---
title: "IndexInfo"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에 대한 기본 정보를 포함합니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

인덱스에 대한 기본 정보를 포함합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | 인덱스 고유 식별자를 가져옵니다. |
|
|  | [getIndexFolder()](#getIndexFolder--) | 인덱스가 위치한 전체 폴더 이름을 가져옵니다. |
|
|  | [getIndexStatus()](#getIndexStatus--) | 인덱스 상태를 가져옵니다. |
|
|  | [getVersion()](#getVersion--) | 인덱스 버전을 가져옵니다. |
|
|  | [getSegmentCount()](#getSegmentCount--) | 인덱스 세그먼트 수를 가져옵니다. |
|
|  | [getTermCount()](#getTermCount--) | 인덱스에 포함된 단어 수를 가져옵니다. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


인덱스 고유 식별자를 가져옵니다.


**Returns:**
java.util.UUID - 인덱스 고유 식별자.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


인덱스가 위치한 전체 폴더 이름을 가져옵니다.


**Returns:**
java.lang.String - 인덱스가 위치한 전체 폴더 이름.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


인덱스 상태를 가져옵니다.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


인덱스 버전을 가져옵니다.


**Returns:**
java.lang.String - 인덱스 버전.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


인덱스 세그먼트 수를 가져옵니다.


**Returns:**
int - 인덱스 세그먼트 수.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


인덱스에 포함된 단어 수를 가져옵니다.


**Returns:**
int - 인덱스에 포함된 단어 수.

