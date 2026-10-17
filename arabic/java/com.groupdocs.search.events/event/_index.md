---
title: "Event"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "هذه الفئة مخصصة للوراثة عند الاشتراك في الأحداث."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

هذه الفئة مخصصة للوراثة عند الاشتراك في الأحداث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Event()](#Event--) | يُنشئ مثيلاً جديدًا من الفئة  Event  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [add(T delegate)](#add-T-) | يضيف مستمعًا للحدث. |
|
|  | [remove(T delegate)](#remove-T-) | يزيل مستمعًا للحدث. |
|
|  | [isEmpty()](#isEmpty--) | يتحقق من وجود مستمع واحد على الأقل. |
|
### Event() {#Event--}
```
public Event()
```


يُنشئ مثيلاً جديدًا من الفئة  Event  .


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


يضيف مستمعًا للحدث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المندوب | T | مستمع للحدث للإضافة. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


يزيل مستمعًا للحدث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المندوب | T | مستمع للحدث للإزالة. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


يتحقق من وجود مستمع واحد على الأقل.


**Returns:**
boolean - قيمة تشير إلى أنه تم إضافة مستمع واحد على الأقل للحدث.

