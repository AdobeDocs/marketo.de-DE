---
unique-page-id: 3571739
description: Installieren und konfigurieren Sie Marketing Sales Insight in Microsoft Dynamics 365 - Marketing Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool, um Ihrem Vertriebsteam ein &quot;Fenster&quot;zu den umfangreichen Daten zu verschaffen, die das Marketing-Team hat. So installieren und konfigurieren Sie.

>[!PREREQUISITES]
>
>Füllen Sie die [Marketing-Microsoft-Integration](http://docs.marketo.com/x/E4A2) aus.
>
>[Laden Sie die richtige ](http://docs.marketo.com/x/LoJo) Lösung für Ihre Version von Microsoft Dynamics CRM herunter.

## Lösung {#import-solution} importieren

1. Melden Sie sich bei [Microsoft Office 365](https://login.microsoftonline.com/) an.

   ![](assets/image2015-3-16-15-58-55.png)

1. Klicken Sie auf das Menü ![—](assets/image2015-3-16-16-1-13.png) und wählen Sie **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Klicken Sie auf das Menü ![—](assets/image2015-5-13-10-5-8.png). Wählen Sie in der Dropdownliste **Einstellungen** und dann **Lösungen**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Sie sollten die Marketing-Lösung [bereits installiert und konfiguriert haben, bevor Sie fortfahren.](../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

   Klicken Sie auf Importieren.
   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicken Sie im neuen Fenster auf **Durchsuchen**. Wählen Sie die [Marketing Sales Insight-Lösung, die Sie in Schritt 1](#msi) heruntergeladen haben. Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt nach Wunsch Ansicht geben. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Vergewissern Sie sich, dass das Feld **markiert** bleibt und klicken Sie auf **Import**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sie können die Protokolldatei herunterladen. Klicken Sie auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastisch! Du solltest die Lösung jetzt sehen. Wenn der Bildschirm nicht vorhanden ist, aktualisieren Sie ihn.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketing and Sales Insight {#connect-marketo-and-sales-insight}

Binden wir Ihre Marketo-Instanz mit Sales Insight in Dynamics zusammen. So:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei Marketing an und gehen Sie zum Abschnitt **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt **Sales Insight** auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie die **Marketo-Host**, **API-URL** und **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen **Geheimschlüssel der API** Ihrer Wahl ein und klicken Sie auf **SAVE**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit *Lead und Kontakt* funktionieren:
   >
   > * Priorität
   > * Dringlichkeit
   > * Relative Bewertung

   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) durch.

1. Klicken Sie in Microsoft Dynamics auf das Symbol ![](assets/image2015-5-13-15-3a49-3a19.png) neben Einstellungen und wählen Sie **Marketing-API-Konfiguration** in der Dropdown-Liste aus.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Klicken Sie auf **Standardkonfiguration**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo kopiert haben.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Klicken Sie auf das Symbol ![](assets/image2015-5-13-16-3a8-3a51.png) in der unteren rechten Ecke, um die Änderungen zu speichern.

## Benutzerzugriff einstellen {#set-user-access}

Sie müssen Benutzern Berechtigungen zur Verwendung von Sales Insight erteilen.

1. Klicken Sie auf das Menü ![](assets/image2015-5-13-10-3a5-3a8.png). Wählen Sie im Dropdown-Menü **Einstellungen** und dann **Sicherheit**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insight gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Wählen Sie die Rolle **Marketo Sales Insight** und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Und Sie sollten alle fertig sein! Zum Testen melden Sie sich bei Dynamics als Benutzer an, der Zugriff auf Marketing Sales Insight hat, und sehen Sie sich einen Interessenten oder Kontakt an.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Sie haben die Leistungsfähigkeit von Marketo Sales Insight für Ihr Vertriebsteam freigegeben.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](http://docs.marketo.com/x/BICMAg)