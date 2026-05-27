---
unique-page-id: 10100266
description: Überblick über benutzerdefinierte Aktivitäten zum Tracking geschäftsspezifischer Personenaktionen, deren Unterschied zu benutzerdefinierten Objekten und die zweistufige Einrichtung zum Erstellen der Aktivität und der API-Implementierung.
title: Grundlegendes zu benutzerdefinierten Aktivitäten
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
TQID: https://experienceleague.adobe.com/QwH82DomS1BDHbK3wfoP14N8xDBKZ28gOLyZ-L8fAeY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 286
ht-degree: 8%

---

# Grundlegendes zu benutzerdefinierten Aktivitäten {#understanding-custom-activities}

Anhand von benutzerdefinierten Aktivitäten eine für Ihr Unternehmen relevante Aktion nachverfolgen, die eine Person getätigt hat.

## Was sind Aktivitäten {#what-are-activities}

Es gibt mehrere Möglichkeiten, wie eine Person mit Ihrer Organisation interagieren kann. Sie können die Website Ihres Unternehmens besuchen, an einer Ihrer Messen teilnehmen oder auf einen Link in einer E-Mail klicken, die an sie gesendet wird. Bei diesen Aktionen handelt es sich um Aktivitäten. Welche Aktion auch immer sie durchführen, Marketo erfasst sie, damit Ihr Marketing-Team besser verstehen kann, wie es ihnen rechtzeitig relevante Informationen senden kann.

## Eigene Aktivitäten {#custom-activities}

Mithilfe benutzerdefinierter Aktivitäten können Sie eine Aktivität verfolgen, die nicht mit einem Marketo-Formular, einer E-Mail oder einer Landingpage verbunden ist. Verwenden Sie eine benutzerdefinierte Aktivität, um zu verfolgen, wann jemand einen Scheck einzahlt. Verwenden Sie eine benutzerdefinierte Aktivität, um zu verfolgen, wann jemand an einem Webinar teilnimmt.

>[!NOTE]
>
>Benutzerdefinierte Aktivitäten unterscheiden sich von benutzerdefinierten Objekten. Verwenden Sie benutzerdefinierte Objekte, wenn sich der Wert ändern kann (d. h., wenn sich die „Autofarbe“ von Blau in Rot ändert). Verwenden Sie benutzerdefinierte Aktivitäten, wenn Sie aufgetretene Momente verfolgen und deren Details sich nicht ändern können (z. B. „gekauftes Auto„).

## Felder {#fields}

Sie können &quot;[ Felder“ hinzufügen](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md) die Sie mit Ihrer Aktivität verknüpfen möchten. Wie das primäre Feld können sie als Filterkriterien in einer Smart-Liste verwendet werden.

## Erste Schritte {#getting-started}

Benutzerdefinierte Aktivitäten funktionieren genau wie Standardaktivitäten. Ihre Einrichtung ist jedoch ein zweistufiger Prozess.

Schritt 1: [Benutzerdefinierte Aktivität erstellen](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md) in Ihrem Marketo-Konto

Schritt 2: Der Mitarbeiter in Ihrem Unternehmen, der mit der Marketo-API arbeitet, kann dann mit der Implementierung beginnen. Weitere Informationen finden Sie hier: [Custom Activity API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST)
