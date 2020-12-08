---
unique-page-id: 7513865
description: Installieren und konfigurieren Sie Marketing Sales Insight in Microsoft Dynamics 2015 - Marketing Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2015
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2015 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool, um Ihrem Vertriebsteam ein &quot;Fenster&quot;zu den umfangreichen Daten zu verschaffen, die das Marketing-Team hat. Hier ist, wie Sie es installieren und konfigurieren in Microsoft Dynamics 201

>[!NOTE]
>
>**Voraussetzungen**
>
>Schließen Sie Ihre [Marketing-Microsoft-Integration](http://docs.marketo.com/x/ZwBd)ab.
>
>[Laden Sie die richtige Lösung](http://docs.marketo.com/x/LoJo) für Ihre Version von Microsoft Dynamics CRM herunter.

## Lösung importieren {#import-solution}

OK, jetzt ist es an der Zeit, die Marketo Sales Insight Lösung in Microsoft Dynamics zu importieren. So geht es:

1. Klicken Sie unter Microsoft Dynamics CRM auf **Einstellungen**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Klicken Sie unter &quot;EINSTELLUNGEN&quot;auf **Anpassungen**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Klicken Sie auf **Lösungen**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Sie sollten die Marketing-Lösung bereits installiert und konfiguriert haben, bevor Sie fortfahren.

1. Klicken Sie auf **Importieren**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicken Sie im neuen Fenster auf **Durchsuchen**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Suchen Sie die Lösung, die Sie oben heruntergeladen haben, und wählen Sie sie aus.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt nach Wunsch Ansicht geben. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Achten Sie darauf, das Kontrollkästchen zu aktivieren, und klicken Sie auf **Importieren**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Laden Sie die Protokolldatei herunter und klicken Sie auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastisch! Du solltest die Lösung jetzt sehen. Wenn der Bildschirm nicht vorhanden ist, aktualisieren Sie ihn.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketing and Sales Insight {#connect-marketo-and-sales-insight}

Binden wir Ihre Marketo-Instanz mit Sales Insight in Dynamics zusammen. So geht es:

>[!NOTE]
>
>Administratorrechte erforderlich.

1. Melden Sie sich bei Marketo an und gehen Sie zum Abschnitt **Admin **s.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt Sales Insight auf API-Konfiguration **bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **MarketingTo-Host**, die **API-URL** und die **API-Benutzer-ID** für die Verwendung in einem späteren Schritt. Geben Sie einen geheimen API-Schlüssel Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit *sowohl Lead als auch Kontakt* für Sales Insight funktionieren:
   >
   >    
   >    
   >    * Priorität
   >    * Dringlichkeit
   >    * Relative Bewertung

   >    
   >    
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)aus.

1. Zurück in Microsoft Dynamics, gehen Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Klicken Sie unter **Einstellungen** auf **Marketing API-Konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Geben Sie die Informationen ein, die Sie zuvor von Marketo erhalten haben, und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich müssen Sie bestimmten Benutzern Zugriff auf Marketo Sales Insight gewähren.

1. Gehen Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Gehe zu **Sicherheit**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insight gewähren möchten, und klicken Sie auf Rollen **verwalten**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Wählen Sie die Rolle &quot;Marketo Sales Insight&quot;und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Und Sie sollten alle fertig sein! Zum Testen melden Sie sich bei Dynamics als Benutzer an, der Zugriff auf Marketing Sales Insight hat, und sehen Sie sich einen Interessenten oder Kontakt an.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Sie haben die Leistungsfähigkeit von Marketo Sales Insight für Ihr Vertriebsteam freigegeben.

>[!NOTE]
>
>**Verwandte Artikel**
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](http://docs.marketo.com/x/BICMAg)

