---
unique-page-id: 42762519
description: Konfiguration für Bestandskunden - Marketo-Dokumente - Produktdokumentation
title: Konfiguration für Bestandskunden
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 4%

---

# Konfiguration für Bestandskunden {#configuration-for-existing-customers}

Richten Sie die folgende Konfiguration ein, um mit der Verwendung des neuen Insights-Dashboards zu beginnen.

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie Ihr [!DNL Salesforce] auf die neueste Version aktualisiert haben

## Konfigurieren von [!DNL Sales Insight] in Marketo {#configure-sales-insight-in-marketo}

1. Öffnen Sie eine neue Registerkarte in Ihrem Browser, um die [!DNL Marketo Sales Insights] Anmeldeinformationen von Ihrem Marketo-Konto abzurufen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Klicken Sie **[!UICONTROL Sales Insight]**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Klicken Sie auf **[!UICONTROL Anzeigen]**, um die REST-API-Anmeldeinformationen zu füllen.

   ![](assets/configuration-for-existing-customers-3.png)

1. Es wird ein Bestätigungs-Popup angezeigt. Klicken Sie auf **[!UICONTROL OK]**.

## Konfigurieren von [!DNL Sales Insight] in [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Klicken Sie in Salesforce auf **[!UICONTROL Setup]**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Suchen Sie nach **[!UICONTROL Remotestandorteinstellungen]** und wählen Sie sie aus.

   ![](assets/configuration-for-existing-customers-5.png)

1. Klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Geben Sie den [!UICONTROL Namen der Remote-Site] (dies kann z. B. „MarketoRestAPI“ sein) und die [!UICONTROL Remote-Site-URL] (Ihre API-URL aus dem Bedienfeld „REST-API-Konfiguration“ in Marketo) ein.

   ![](assets/configuration-for-existing-customers-7.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/configuration-for-existing-customers-8.png)

   Sie haben jetzt die Remote-Site-Einstellung für die Rest-API erstellt.

## Auf Marketo Sales Insight zugreifen {#access-marketo-sales-insight}

1. Kopieren Sie die Anmeldeinformationen aus dem REST-API-Bedienfeld auf [!DNL Marketo’s Sales Insight] Admin-Seite. Fügen Sie sie in den Abschnitt REST-API auf der Seite [!DNL Sales Insight]-Konfiguration von Salesforce ein.

1. Geben Sie den [!UICONTROL API-Geheimschlüssel] ein.

   ![](assets/configuration-for-existing-customers-9.png)
