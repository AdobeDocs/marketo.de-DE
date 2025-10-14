---
unique-page-id: 37355602
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online - Marketo-Dokumentation - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 4%

---

# Installieren und Konfigurieren von [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics Online] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

[!DNL Marketo Sales Insight] ist ein fantastisches Tool, mit dem Sie Ihrem Verkaufsteam einen Einblick in die Fülle der Daten geben können, die das Marketing-Team hat. Im Folgenden wird beschrieben, wie Sie es in [!DNL Microsoft Dynamics Online] installieren und konfigurieren.

>[!PREREQUISITES]
>
>Abschließen der Marketo-Microsoft-Integration
>
>[Laden Sie die richtige Lösung &#x200B;](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Ihre Version von [!DNL Microsoft Dynamics CRM] herunter.

## Lösung importieren {#import-solution}

>[!NOTE]
>
>Wenn Sie die einheitliche Benutzeroberfläche verwenden, klicken Sie vor Schritt 1 unten auf das Einstellungssymbol in der oberen rechten Ecke und wählen Sie **[!UICONTROL Erweiterte Einstellungen]**.

1. Klicken Sie unter Microsoft Dynamics CRM **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Klicken Sie unter Einstellungen auf **[!UICONTROL Anpassungen]**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Klicken Sie auf **[!UICONTROL Lösungen]**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Sie sollten die Marketo-Lösung bereits installiert und konfiguriert haben, bevor Sie fortfahren.

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Klicken Sie im neuen Fenster auf &quot;**[!UICONTROL &quot;]**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Suchen Sie auf Ihrem Computer nach der Lösung, die Sie gerade heruntergeladen haben, und installieren Sie sie.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/seven.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt anzeigen, wenn Sie möchten. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Lassen Sie das Kontrollkästchen aktiviert und klicken Sie auf **[!UICONTROL Importieren]**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Laden Sie die Protokolldatei herunter und klicken Sie dann auf **[!UICONTROL Schließen]**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastisch! Sie sollten die Lösung jetzt sehen. Wenn er nicht da ist, aktualisieren Sie Ihren Bildschirm.

   ![](assets/eleven.png)

1. Klicken Sie **[!UICONTROL Anpassung veröffentlichen]**.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie die Synchronisierung globaler [!DNL MS Dynamics] aktivieren.

## Marketo und [!DNL Sales Insight] verbinden {#connect-marketo-and-sales-insight}

Binden wir Ihre Marketo-Instanz an [!DNL Sales Insight] in [!DNL Dynamics]. So geht&#39;s:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei Marketo an und gehen Sie zum Abschnitt **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Klicken Sie im Abschnitt [!UICONTROL Sales Insight] auf **[!UICONTROL API-Konfiguration bearbeiten]**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Kopieren Sie den **[!UICONTROL Marketo]** Host **[!UICONTROL , die API]** und die **[!UICONTROL API-Benutzer-ID]** zur Verwendung in einem späteren Schritt. Geben Sie einen API-Geheimschlüssel Ihrer Wahl ein und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!CAUTION]
   >
   >Verwenden Sie in Ihrem API-Geheimschlüssel kein kaufmännisches Und-Zeichen (&amp;).

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit _Lead und Kontakt_ funktioniert: [!DNL Sales Insight]
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Zurück in [!DNL Microsoft Dynamics], gehen Sie zu **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Marketo API-Konfiguration]**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo übernommen haben, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/enable-one.png)

1. Wählen Sie unter Integration die Option **[!UICONTROL Microsoft Dynamics]** aus.

   ![](assets/enable-two.png)

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-three.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** neben [!UICONTROL Details zur Feldsynchronisierung].

   ![](assets/enable-four.png)

1. Dadurch _(automatisch_ zuvor deaktivierte MSI-Felder ([!UICONTROL Dringlichkeit], [!UICONTROL Relativer Score] und [!UICONTROL Priorität]) ausgewählt. Klicken Sie einfach auf **[!UICONTROL Speichern]**, um mit der Synchronisierung von Daten zu beginnen.

   ![](assets/enable-five.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich müssen Sie bestimmten Benutzern Zugriff gewähren, um [!DNL Marketo Sales Insight] verwenden zu können.

1. Navigieren Sie zu **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Navigieren Sie zu **[!UICONTROL Sicherheit]**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Wählen Sie die Benutzer aus, denen Sie [!DNL Sales Insight] Zugriff gewähren möchten, und klicken Sie auf **[!UICONTROL Rollen verwalten]**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Wählen Sie die Rolle [!DNL Marketo Sales Insight] aus und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Und Sie sollten fertig sein! Melden Sie sich zum Testen bei [!DNL Dynamics] als Benutzer an, der Zugriff auf [!DNL Marketo Sales Insight] hat, und sehen Sie sich einen Lead oder Kontakt an.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
