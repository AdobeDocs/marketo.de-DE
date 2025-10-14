---
description: Warum werden meine Vertriebsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? – Marketo-Dokumente – Produktdokumentation
title: Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 7%

---

# Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Ich sehe keine mit Salesforce synchronisierten E-Mail- oder Anrufaktivitäten.**

* Stellen Sie sicher, dass Sie mit Salesforce verbunden sind. Jeder Anwender muss über eine Verbindung verfügen, um seine E-Mails und Aufrufe an Salesforce zu protokollieren.
* Stellen Sie sicher, dass Sie [Salesforce-Synchronisierungseinstellungen konfiguriert &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* E-Mails führen eine Datensatzsuche anhand der Salesforce-ID als primäre Suche und der E-Mail-Adresse als sekundäre Adresse durch. Sie können bestätigen, dass einem Personendatensatz in der (Web-App für [&#x200B; Aktionen) eine Salesforce-ID und eine E-Mail](https://toutapp.com/next#command_center){target="_blank"}Adresse zugeordnet sind.
* Aufrufe führen nur eine Datensatzsuche durch, die auf der Salesforce-ID basiert. Wenn im Personendatensatz in Aktionen keine Salesforce-ID vorhanden ist, wird der Aufruf nicht protokolliert. Sie können bestätigen, dass einem Personendatensatz in der ([-Web-App) eine Salesforce-ID &#x200B;](https://toutapp.com/next#command_center){target="_blank"} ist.

**Aktivitätsfelder werden in Salesforce Update nicht angezeigt.**

Wenn in Salesforce keine Aktualisierung der E[Mail-Attributfelder](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} angezeigt wird, kann dies auf Einschränkungen der Barrierefreiheit von Feldern Ihres Teams zurückzuführen sein. Die Sicherheit auf Salesforce-Feldebene bietet Salesforce-Administratoren die Möglichkeit, Einschränkungen hinsichtlich der Informationen vorzunehmen, die von Benutzenden angezeigt und bearbeitet werden können. Wenn Benutzende von Aktionen keinen Zugriff auf das Anzeigen und Bearbeiten dieser Felder haben, kann die Synchronisierung der Aktionsaktivität diese Felder nicht aktualisieren.

* Arbeiten Sie mit Ihrem Salesforce-Administrator zusammen, um sicherzustellen, dass diese Sicherheitseinstellungen die Aktionsfelder [Salesforce-Aktivität“ nicht &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Wenn Sie Salesforce-Administrator sind, können Sie Ihr Feld Barrierefreiheit auf der Registerkarte Sicherheitskontrollen sehen. Die Hauptobjekte, mit denen Aktionen interagieren werden, sind: Leads, Kontakte, Konten, Chancen und Aufgaben/Aktivitäten.

>[!NOTE]
>
>Die mit den Lead-, Kontakt-, Konto- und Opportunity-Objekten verknüpften Felder werden mit dem Sales Insight Salesforce Package installiert. Felder, die mit dem Datensatztyp [Aufgabe/Aktivität verknüpft sind, müssen &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} Salesforce-Admin erstellt werden.
