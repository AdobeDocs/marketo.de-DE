---
unique-page-id: 3571737
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013 - Marketo Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool, mit dem Sie Ihrem Vertriebsteam ein &quot;Fenster&quot;in den Datenbestand des Marketing-Teams geben können. So installieren und konfigurieren Sie es.

>[!PREREQUISITES]
>
>Schließen Sie Ihre Marketo-Microsoft-Integration ab.
>
>[Die richtige Lösung herunterladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) für Ihre Microsoft Dynamics CRM-Version.

## Importlösung {#import-solution}

OK, jetzt ist es an der Zeit, die Marketo Sales Insight-Lösung in Microsoft Dynamics zu importieren.

1. under **Microsoft Dynamics CRM** click **Einstellungen**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. under **Einstellungen** klicken **Anpassungen**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Klicken **Lösungen**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Sie sollten Marketo bereits installiert und konfiguriert haben, bevor Sie fortfahren

1. Klicken **Import**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicken Sie im neuen Fenster auf **Durchsuchen**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Suchen und wählen Sie die Lösung aus, die Sie oben heruntergeladen haben.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicken **Nächste**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt bei Bedarf anzeigen. Klicken **Nächste**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Vergewissern Sie sich, dass das Kästchen markiert ist, und klicken Sie auf **Import**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sie können die Protokolldatei herunterladen. Klicken Sie auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastisch Sie sollten die Lösung jetzt sehen. Wenn er nicht vorhanden ist, aktualisieren Sie den Bildschirm.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Verbinden von Marketo und Sales Insight {#connect-marketo-and-sales-insight}

Verknüpfen wir Ihre Marketo-Instanz mit Sales Insight in Dynamics.

>[!NOTE]
>
>Benötigte Administratorrechte.

1. Melden Sie sich bei Marketo an und wechseln Sie zum **Admin** Abschnitt.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Unter dem **Sales Insight** Abschnittsklick **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie die **Marketo-Host**, **API-URL** und **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie eine **API-Geheimschlüssel** und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden für _Lead und Kontakt_ für Sales Insight funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahrens](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Zurück in Microsoft Dynamics, navigieren Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. under **Einstellungen** klicken **Marketo API-Konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicken **Neu**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo erhalten haben, und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich können Sie bestimmten Benutzern Zugriff auf Marketo Sales Insight gewähren.

1. Navigieren Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Klicken **Benutzer**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insight gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Wählen Sie die **Marketo Sales Insight** Rolle und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Und du solltest fertig sein! Melden Sie sich zum Testen bei Dynamics als Benutzer an, der Zugriff auf Marketo Sales Insight hat, und sehen Sie sich einen Lead oder Kontakt an.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Sie haben jetzt die Möglichkeiten von Marketo Sales Insight für Ihr Vertriebsteam freigeschaltet.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
