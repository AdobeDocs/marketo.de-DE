---
description: Fehlerbehebung, wenn Vertriebsaktivitäten und -felder nicht mit Salesforce synchronisiert werden. Überprüfen Sie API-Protokollierung, benutzerdefinierte Felder und Berechtigungen.
title: Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
TQID: https://experienceleague.adobe.com/ATXA1f3wZqC0z-QFjrK2ax0w8-wmf5cjKn4jdZJLtt0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 339
ht-degree: 6%

---

# Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Ich sehe keine mit Salesforce synchronisierten E-Mail- oder Anrufaktivitäten.**

* Stellen Sie sicher, dass Sie mit Salesforce verbunden sind. Jeder Anwender muss über eine Verbindung verfügen, um seine E-Mails und Aufrufe an Salesforce zu protokollieren.
* Stellen Sie sicher, dass Sie [Salesforce-Synchronisierungseinstellungen konfiguriert &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* E-Mails führen eine Datensatzsuche anhand der Salesforce-ID als primäre Suche und der E-Mail-Adresse als sekundäre Adresse durch. Sie können bestätigen, dass einem Personendatensatz in der (Web-App für [&#x200B; Aktionen) eine Salesforce-ID und eine E-Mail](https://toutapp.com/next#command_center){target="_blank"}Adresse zugeordnet sind.
* Aufrufe führen nur eine Datensatzsuche durch, die auf der Salesforce-ID basiert. Wenn im Personendatensatz in Aktionen keine Salesforce-ID vorhanden ist, wird der Aufruf nicht protokolliert. Sie können bestätigen, dass einem Personendatensatz in der ([-Web-App) eine Salesforce-ID &#x200B;](https://toutapp.com/next#command_center){target="_blank"} ist.

**Aktivitätsfelder werden in Salesforce Update nicht angezeigt.**

Wenn E-Mail-[Aktivitätsattributfelder) in Salesforce nicht &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} werden, kann dies auf Einschränkungen der Feldzugriffsmöglichkeiten für Ihr Team zurückzuführen sein. Die Sicherheit auf Salesforce-Feldebene bietet Salesforce-Administratoren die Möglichkeit, Einschränkungen hinsichtlich der Informationen vorzunehmen, die von Benutzenden angezeigt und bearbeitet werden können. Wenn Benutzende von Aktionen keinen Zugriff auf das Anzeigen und Bearbeiten dieser Felder haben, kann die Synchronisierung der Aktionsaktivität diese Felder nicht aktualisieren.

* Arbeiten Sie mit Ihrem Salesforce-Administrator zusammen, um sicherzustellen, dass diese Sicherheitseinstellungen die Aktionsfelder [Salesforce-Aktivität“ nicht &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Wenn Sie Salesforce-Administrator sind, können Sie Ihr Feld Barrierefreiheit auf der Registerkarte Sicherheitskontrollen anzeigen. Die Hauptobjekte, mit denen Aktionen interagieren werden, sind: Leads, Kontakte, Konten, Chancen und Aufgaben/Aktivitäten.

>[!NOTE]
>
>Die mit den Lead-, Kontakt-, Konto- und Opportunity-Objekten verknüpften Felder werden mit dem Sales Insight Salesforce Package installiert. Felder, die mit dem Datensatztyp [Aufgabe/Aktivität verknüpft sind, müssen &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} Salesforce-Admin erstellt werden.
