---
unique-page-id: 3571735
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 - Marketo-Dokumentation - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 5%

---

# Installieren und Konfigurieren von [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics 2011] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] ist ein fantastisches Tool für Ihr Vertriebsteam. Im Folgenden finden Sie eine schrittweise Anleitung zur Installation und Konfiguration [!DNL Microsoft Dynamics 2011] On-Premise.

>[!PREREQUISITES]
>
>Abschließen der Marketo-Microsoft-Integration
>
>[Laden Sie die richtige Lösung &#x200B;](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Ihre Version [!DNL Microsoft Dynamics] CRM herunter.

## Lösung importieren {#import-solution}

1. Beim [!DNL Microsoft Dynamics] CRM anmelden. Klicken **[!UICONTROL im]** Menü unten links auf „Einstellungen“.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen **[!UICONTROL in]** Struktur „Lösungen“ aus.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicken Sie **Importieren** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Sie sollten die Marketo[Lösung bereits installiert und &#x200B;](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) haben, bevor Sie fortfahren.

1. Klicken Sie **[!UICONTROL Durchsuchen]**. Wählen Sie die [!DNL Marketo Sales Insight] Lösung aus[&#x200B; die Sie heruntergeladen &#x200B;](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Überprüfen Sie die Details der Lösung und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Stellen Sie sicher, dass die Option SDK-Nachricht aktiviert ist. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Warten Sie nun, bis der Import abgeschlossen ist.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight] wird jetzt in der Liste Lösung angezeigt. Juhu!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Wählen Sie [!DNL Marketo Sales Insight] und klicken Sie auf **Alle Anpassungen veröffentlichen** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Marketo und Sales Insight verbinden  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt **[!UICONTROL Sales Insight]** auf **[!UICONTROL API-Konfiguration]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **[!UICONTROL Marketo]** Host **[!UICONTROL , die API]** und die **[!UICONTROL API-Benutzer-ID]** zur Verwendung in einem späteren Schritt. Geben Sie einen **[!UICONTROL API-Geheimschlüssel]** Ihrer Wahl ein und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!CAUTION]
   >
   >Verwenden Sie in Ihrem API-Geheimschlüssel kein kaufmännisches Und-Zeichen (&amp;).

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo Insight synchronisiert werden, damit _Lead und Kontakt_ funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Wechseln Sie zurück zu Dynamics und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen Sie **[!UICONTROL Marketo-API]** Konfiguration“ in der Baumstruktur aus.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicken Sie **[!UICONTROL Standardkonfiguration]**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo übernommen haben.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Benutzerzugriff festlegen {#set-user-access}

Richten Sie Benutzerrollen ein, um bestimmten Benutzern Zugriff auf [!DNL Sales Insight] zu gewähren.

1. Wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Wählen Sie **[!UICONTROL Struktur]** Administration“ aus.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff gewähren möchten, und klicken Sie auf **[!UICONTROL Rollen verwalten]**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Wählen Sie die Rolle **[!UICONTROL Marketo Sales Insight]** aus und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Und das war&#39;s! Alle Benutzenden, die Zugriff haben, können jetzt den Abschnitt Vertriebs-insight in der Lead-/Kontaktdetailansicht sehen.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Glückwunsch. Sie haben jetzt die Macht der [!DNL Marketo Sales Insight] entfesselt.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
