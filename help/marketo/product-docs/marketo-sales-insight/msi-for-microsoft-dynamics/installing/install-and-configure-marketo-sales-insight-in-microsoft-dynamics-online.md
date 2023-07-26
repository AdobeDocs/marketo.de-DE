---
unique-page-id: 37355602
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online - Marketo Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight ist ein fantastisches Tool, mit dem Sie Ihrem Vertriebsteam ein &quot;Fenster&quot;in den Datenbestand des Marketing-Teams geben können. Hier erfahren Sie, wie Sie es in Microsoft Dynamics Online installieren und konfigurieren.

>[!PREREQUISITES]
>
>Schließen Sie Ihre Marketo-Microsoft-Integration ab.
>
>[Die richtige Lösung herunterladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) für Ihre Microsoft Dynamics CRM-Version.

## Importlösung {#import-solution}

>[!NOTE]
>
>Wenn Sie die einheitliche Oberfläche verwenden, klicken Sie vor Schritt 1 unten auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen**.

1. Klicken Sie unter Microsoft Dynamics CRM auf **Einstellungen**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Klicken Sie unter Einstellungen auf **Anpassungen**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Klicks **Lösungen**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Sie sollten die Marketo-Lösung bereits installiert und konfiguriert haben, bevor Sie fortfahren.

1. Klicks **Import**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Klicken Sie im neuen Fenster auf **Durchsuchen**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Suchen und installieren Sie auf Ihrem Computer die soeben heruntergeladene Lösung.

1. Klicks **Nächste**.

   ![](assets/seven.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt bei Bedarf anzeigen. Klicks **Nächste**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Vergewissern Sie sich, dass das Kästchen markiert ist, und klicken Sie auf **Import**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Sie können die Protokolldatei herunterladen und dann auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastisch Sie sollten die Lösung jetzt sehen. Wenn er nicht vorhanden ist, aktualisieren Sie den Bildschirm.

   ![](assets/eleven.png)

1. Klicks **Veröffentlichungsanpassung**.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie die Synchronisierung mit Global MS Dynamics aktivieren.

## Verbinden von Marketo und Sales Insight {#connect-marketo-and-sales-insight}

Verknüpfen wir Ihre Marketo-Instanz mit Sales Insight in Dynamics. So geht&#39;s:

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Melden Sie sich bei Marketo an und wechseln Sie zum **Admin** Abschnitt.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Klicken Sie unter dem Abschnitt Sales Insight auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Kopieren Sie die **Marketo-Host**, **API-URL**, und **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen API-Geheimschlüssel Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden _Lead und Kontakt_ für Sales Insight funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahrens](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Wechseln Sie in Microsoft Dynamics zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. under **Einstellungen** klicken **Marketo API-Konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Klicks **Neu**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo erhalten haben, und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/enable-one.png)

1. Wählen Sie unter Integration die Option **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Klicks **Synchronisierung aktivieren**.

   ![](assets/enable-three.png)

1. Klicks **Bearbeiten** neben &quot;Feldsynchronisierungsdetails&quot;.

   ![](assets/enable-four.png)

1. Dies wird _automatisch_ Wählen Sie MSI-Felder aus, die zuvor deaktiviert waren (Dringlichkeit, Relativer Wert und Priorität). Einfaches Klicken **Speichern** , um die Synchronisierung der Daten zu starten.

   ![](assets/enable-five.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich müssen Sie bestimmten Benutzern Zugriff auf Marketo Sales Insight gewähren.

1. Navigieren Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Navigieren Sie zu **Sicherheit**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Klicks **Benutzer**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insight gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Wählen Sie die Rolle Marketo Sales Insight aus und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Und du solltest fertig sein! Melden Sie sich zum Testen bei Dynamics als Benutzer an, der Zugriff auf Marketo Sales Insight hat, und sehen Sie sich einen Lead oder Kontakt an.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
