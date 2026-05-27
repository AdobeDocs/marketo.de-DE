---
unique-page-id: 11386358
description: Erfahren Sie mehr über die Marketo Engage-Sandbox zum Testen vor der Produktion. Verwenden Sie eine Sandbox-Instanz, um zu testen, ohne die Produktion zu beeinträchtigen.
title: Marketo-Sandbox
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
TQID: https://experienceleague.adobe.com/Cb1H0PKG-G0c4FkIcjI-erNzR0dwRtj7TwfqtwhFFMI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 3%

---

# Marketo-Sandbox {#marketo-sandbox}

Eine Marketo Engage-Sandbox ist eine zusätzliche Instanz, die zu Testzwecken vor der Implementierung in der Produktionsumgebung verwendet wird.

>[!AVAILABILITY]
>
>Nicht jeder hat diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

Eine Marketo-Sandbox kann nicht mit Ihrem regulären CRM-System synchronisiert werden, wenn sie bereits mit Ihrer Produktionsinstanz synchronisiert wurde. Verwenden Sie die Sandbox Ihres CRM für die Synchronisierung und führen Sie alle Schritte der ursprünglichen Synchronisierung aus.

## Wissenswertes über Sandboxes {#things-to-know-about-sandboxes}

* Wenn Sie Benutzer hinzufügen möchten, ist der Prozess identisch mit dem [Hinzufügen von Benutzern in der Produktion](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user). Auch hier müssen sie eine andere E-Mail-Adresse verwenden, wenn sie bereits über eine Marketo-Anmeldung verfügen.
* Ihre Marketo-Sandbox startet leer, verfügt jedoch über dieselben Funktionen wie Ihre Produktionsinstanz.
* Wenn Sie ein Programm in Ihrer Sandbox erstellen und in die Produktion verschieben möchten, können Sie einen [Programm-Import](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md) durchführen.
* Sandboxes werden gedrosselt, sodass Produktionsinstanzen nicht durch Testumgebungen beeinträchtigt werden. Pro Kampagnenausführung können bis zu 20 E-Mails gesendet werden.

>[!CAUTION]
>
>Die Sandbox-Aktualisierung für Marketo Dynamics _oder_ Salesforce Sync wird derzeit nicht unterstützt. Wenn Sie Ihre CRM-Sandbox aktualisieren müssen, ist eine neue Marketo-Sandbox erforderlich. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

## Instanzkopie {#instance-copy}

Sie können einen Support-Fall senden, in dem eine einmalige Instanzkopie zum Ausfüllen Ihrer Sandbox angefordert wird. Die Instanzkopie bringt jedoch nicht _alles_. Weitere Informationen erhalten Sie beim [Marketo](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de)Support.

>[!NOTE]
>
>Wenn Sie Ihr natives CRM ändern, ist eine neue Marketo-Instanz erforderlich und eine Instanzkopie in die neue Marketo-Instanz ist nicht möglich. Arbeiten Sie stattdessen mit dem Marketo-Support zusammen, um die Funktionalität „Programm importieren“ zu erkunden.
