---
unique-page-id: 3571737
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013 - Dokumentation zu Marketo - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 2%

---

# Installieren und Konfigurieren von [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics 2013] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] ist ein fantastisches Tool, mit dem Sie Ihrem Verkaufsteam einen Einblick in die Fülle der Daten geben können, die das Marketing-Team hat. So installieren und konfigurieren Sie es.

>[!PREREQUISITES]
>
>Abschließen der Marketo-Microsoft-Integration
>
>[Laden Sie die richtige Lösung ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Ihre Version [!DNL Microsoft Dynamics] CRM herunter.

## Lösung importieren {#import-solution}

OK, jetzt ist es Zeit, die [!DNL Marketo Sales Insight] Lösung in [!DNL Microsoft Dynamics] zu importieren.

1. Klicken Sie unter **[!UICONTROL Microsoft Dynamics CRM]** auf **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Anpassungen]**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Klicken Sie auf **[!UICONTROL Lösungen]**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Sie sollten Marketo bereits installiert und konfiguriert haben, bevor Sie fortfahren

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicken Sie im neuen Fenster auf &quot;**[!UICONTROL &quot;]**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Suchen Sie die Lösung, die Sie oben heruntergeladen haben, und wählen Sie sie aus.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt anzeigen, wenn Sie möchten. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Lassen Sie das Kontrollkästchen aktiviert und klicken Sie auf **[!UICONTROL Importieren]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sie können die Protokolldatei gerne herunterladen. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastisch! Sie sollten die Lösung jetzt sehen. Wenn er nicht da ist, aktualisieren Sie Ihren Bildschirm.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Marketo und Sales Insight verbinden {#connect-marketo-and-sales-insight}

Binden wir Ihre Marketo-Instanz an [!DNL Sales Insight] in [!DNL Dynamics].

>[!NOTE]
>
>Administratorrechte erforderlich.

1. Melden Sie sich bei Marketo an und gehen Sie zum Abschnitt **[!UICONTROL Admin]** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt **[!UICONTROL Sales Insight]** auf **[!UICONTROL API-Konfiguration]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **[!UICONTROL Marketo]** Host **[!UICONTROL , die API]** und die **[!UICONTROL API-Benutzer-ID]** zur Verwendung in einem späteren Schritt. Geben Sie einen **[!UICONTROL API-Geheimschlüssel]** Ihrer Wahl ein und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!CAUTION]
   >
   >Verwenden Sie in Ihrem API-Geheimschlüssel kein kaufmännisches Und-Zeichen (&amp;).

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo Insight synchronisiert werden, damit _Lead und Kontakt_ funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Zurück in [!DNL Microsoft Dynamics], gehen Sie zu **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Marketo API-Konfiguration]**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo übernommen haben, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich können Sie bestimmten Benutzern Zugriff auf [!DNL Marketo Sales Insight] gewähren.

1. Navigieren Sie zu **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insight gewähren möchten, und klicken Sie auf **[!UICONTROL Rollen verwalten]**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Wählen Sie die Rolle **[!UICONTROL Marketo Sales Insight]** aus und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Und Sie sollten fertig sein! Um schließlich zu testen, melden Sie sich bei [!DNL Dynamics] als Benutzer an, der Zugriff auf [!DNL Marketo Sales Insight] hat, und sehen Sie sich einen Lead oder Kontakt an.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Jetzt haben Sie die [!DNL Marketo Sales Insight] für Ihr Vertriebsteam freigeschaltet.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
