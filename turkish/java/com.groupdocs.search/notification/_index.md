---
title: "Notification"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndekse gönderilen tüm bildirimler için temel sınıf."
type: docs
weight: 22
url: /tr/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

İndekse gönderilen tüm bildirimlerin temel sınıfı. Bu sınıf ayrıca bildirim nesneleri oluşturmak için yöntemler içerir.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Notification()](#Notification--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Yeniden indekslenmeye gerek olmayan, yeniden adlandırılmış bir indeksli belgeyi yeniden adlandırmak için bir bildirim nesnesi oluşturur. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Yeniden indekslenmeye gerek olmayan, yeniden adlandırılmış bir indeksli belgeyi yeniden adlandırmak için bir bildirim nesnesi oluşturur. Yeniden adlandırılan belge, içeriği değişmiş olsa bile bir sonraki güncelleme işlemi sırasında yeniden indekslenmeyecektir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | oldPath | java.lang.String | İndeksli belgenin eski yolu. |
|
|  | newPath | java.lang.String | İndekslenmiş belgeye yeni yol. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

