---
unique-page-id: 42762519
description: Konfiguration für Bestandskunden - Marketo-Dokumente - Produktdokumentation
title: Konfiguration für Bestandskunden
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 4%

---

# Konfiguration für Bestandskunden {#configuration-for-existing-customers}

Richten Sie die folgende Konfiguration ein, um mit der Verwendung des neuen Insights-Dashboards zu beginnen.

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie Ihr Salesforce-Paket auf die neueste Version aktualisiert haben

## Konfigurieren von Sales Insights in Marketo {#configure-sales-insight-in-marketo}

1. Öffnen Sie eine neue Registerkarte in Ihrem Browser, um die Anmeldedaten für Marketo Sales Insights von Ihrem Marketo-Konto abzurufen.

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Klicken Sie **Sales Insight**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Klicken Sie auf **Anzeigen**, um die REST-API-Anmeldeinformationen zu füllen.

   ![](assets/configuration-for-existing-customers-3.png)

1. Es wird ein Bestätigungs-Popup angezeigt. Klicken Sie auf **OK**.

## Konfigurieren von Sales Insights in Salesforce {#configure-sales-insight-in-salesforce}

1. Klicken Sie in Salesforce auf **Setup**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Suchen Sie nach **Remotestandorteinstellungen** und wählen Sie sie aus.

   ![](assets/configuration-for-existing-customers-5.png)

1. Klicken Sie auf **Neue Remote-Site**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Geben Sie den Namen der Remote-Site (dies kann z. B. „MarketoRestAPI“ sein) und die Remote-Site-URL (Ihre API-URL aus dem Bedienfeld „REST-API-Konfiguration“ in Marketo) ein.

   ![](assets/configuration-for-existing-customers-7.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/configuration-for-existing-customers-8.png)

   Sie haben jetzt die Remote-Site-Einstellung für die Rest-API erstellt.

## Auf Marketo Sales Insight zugreifen {#access-marketo-sales-insight}

1. Kopieren Sie die Anmeldeinformationen aus dem REST-API-Bedienfeld auf der Admin-Seite für Sales Insights in Marketo. Fügen Sie sie in den Abschnitt REST-API auf der Seite Sales Insight-Konfiguration von Salesforce ein.

1. Geben Sie den API-Geheimschlüssel ein.

   ![](assets/configuration-for-existing-customers-9.png)
