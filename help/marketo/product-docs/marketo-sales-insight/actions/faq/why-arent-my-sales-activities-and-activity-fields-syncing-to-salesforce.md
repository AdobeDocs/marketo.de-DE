---
description: Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? - Marketo-Dokumente - Produktdokumentation
title: Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert?
exl-id: 0836876d-1b89-4464-a841-81320a6e45fd
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Warum werden meine Verkaufsaktivitäten und Aktivitätsfelder nicht mit Salesforce synchronisiert? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Ich sehe keine mit Salesforce synchronisierten E-Mail- oder Aufrufaktivitäten.**

* Stellen Sie sicher, dass Sie mit Salesforce verbunden sind. Jeder Benutzer muss über eine Verbindung verfügen, um seine E-Mails und Aufrufe bei Salesforce zu protokollieren.
* Stellen Sie sicher, dass Sie [Salesforce-Synchronisierungseinstellungen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* E-Mails führen eine Datensatzsuche basierend auf der Salesforce-ID als primärer Suche und der E-Mail-Adresse als sekundärer Adresse durch. Sie können bestätigen, dass ein Personendatensatz über eine Salesforce-ID und eine mit ihm verknüpfte E-Mail-Adresse verfügt in der [Aktionen-Web-App](https://toutapp.com/next#command_center){target="_blank"}.
* Aufrufe führen eine Datensatzsuche nur basierend auf der Salesforce-ID durch. Wenn im Personendatensatz in Aktionen keine Salesforce-ID vorhanden ist, wird der Aufruf nicht protokolliert. Sie können bestätigen, dass einem Personendatensatz in der Variablen [Aktionen-Web-App](https://toutapp.com/next#command_center){target="_blank"}.

**Im Salesforce-Update werden keine Aktivitätsfelder angezeigt.**

Wenn keine E-Mail angezeigt wird [Aktivitätsattributfelder](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} in Salesforce aktualisiert wurde, kann dies auf Einschränkungen der Barrierefreiheit für das Feld in Ihrem Team zurückzuführen sein. Die Sicherheit auf Salesforce-Feldebene gibt Salesforce-Administratoren die Möglichkeit, Einschränkungen dafür vorzunehmen, welche Informationen von Benutzern angezeigt und bearbeitet werden können. Wenn Benutzer von Aktionen keinen Zugriff auf die Ansicht und Bearbeitung dieser Felder haben, schlägt die Synchronisierung von Aktionen-Aktivitäten fehl, um diese Felder zu aktualisieren.

* Arbeiten Sie mit Ihrem Salesforce-Administrator zusammen, um sicherzustellen, dass diese Sicherheitseinstellungen nicht in die [Aktionsfelder Salesforce-Aktivität](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Als Salesforce-Administrator können Sie Ihre Barrierefreiheit für Felder auf der Registerkarte Sicherheitskontrollen anzeigen. Die Hauptobjekte, mit denen Aktionen interagieren, sind: Leads, Kontakte, Konten, Chancen und Aufgaben/Aktivitäten.

>[!NOTE]
>
>Felder, die mit den Objekten &quot;Lead&quot;, &quot;Kontakt&quot;, &quot;Konto&quot;und &quot;Chancen&quot;verknüpft sind, werden mit dem Sales Insight Salesforce-Paket installiert. Felder, die mit dem [Aufgabe/Aktivitäts-Record-Typ muss erstellt werden](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} von einem Salesforce-Administrator.
