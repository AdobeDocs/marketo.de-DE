---
description: Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? - Marketo-Dokumente - Produktdokumentation
title: Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Ich sehe keine mit Salesforce synchronisierten E-Mail- oder Aufrufaktivitäten.**

* Stellen Sie sicher, dass Sie mit Salesforce verbunden sind. Jeder Benutzer muss über eine Verbindung verfügen, um seine E-Mails und Aufrufe bei Salesforce zu protokollieren.
* Stellen Sie sicher, dass Sie die [Salesforce-Synchronisierungseinstellungen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"} konfiguriert haben.
* E-Mails führen eine Datensatzsuche basierend auf der Salesforce-ID als primärer Suche und der E-Mail-Adresse als sekundärer Adresse durch. Sie können in der [Aktionen-Web-App](https://toutapp.com/next#command_center){target="_blank"} bestätigen, dass ein Personendatensatz über eine Salesforce-ID und eine mit ihnen verknüpfte E-Mail-Adresse verfügt.
* Aufrufe führen eine Datensatzsuche nur basierend auf der Salesforce-ID durch. Wenn im Personendatensatz in Aktionen keine Salesforce-ID vorhanden ist, wird der Aufruf nicht protokolliert. Sie können in der [Aktionen-Webanwendung](https://toutapp.com/next#command_center){target="_blank"} bestätigen, dass einem Personendatensatz eine Salesforce-ID zugeordnet ist.

**Ich sehe keine Aktivitätsfelder in der Salesforce-Aktualisierung.**

Wenn Sie in Salesforce keine Aktualisierung der E-Mail-Aktivitätsattributfelder ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} sehen, kann dies auf Einschränkungen der Barrierefreiheit für Felder Ihres Teams zurückzuführen sein. [ Die Sicherheit auf Salesforce-Feldebene gibt Salesforce-Administratoren die Möglichkeit, Einschränkungen dafür vorzunehmen, welche Informationen von Benutzern angezeigt und bearbeitet werden können. Wenn Benutzer von Aktionen keinen Zugriff auf die Ansicht und Bearbeitung dieser Felder haben, schlägt die Synchronisierung von Aktionen-Aktivitäten fehl, um diese Felder zu aktualisieren.

* Arbeiten Sie mit Ihrem Salesforce-Administrator zusammen, um sicherzustellen, dass diese Sicherheitseinstellungen nicht in die [Aktionen Salesforce-Aktivitätsfelder](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} eingreifen.
* Als Salesforce-Administrator können Sie Ihre Barrierefreiheit für Felder auf der Registerkarte Sicherheitskontrollen anzeigen. Die Hauptobjekte, mit denen Aktionen interagieren, sind: Leads, Kontakte, Konten, Chancen und Aufgaben/Aktivitäten.

>[!NOTE]
>
>Felder, die mit den Objekten &quot;Lead&quot;, &quot;Kontakt&quot;, &quot;Konto&quot;und &quot;Chancen&quot;verknüpft sind, werden mit dem Sales Insight Salesforce-Paket installiert. Felder, die mit dem Datensatz [Aufgabe/Aktivität verknüpft sind, müssen von einem Salesforce-Administrator erstellt werden.](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
