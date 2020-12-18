---
unique-page-id: 3571735
description: Installieren und konfigurieren Sie Marketing Sales Insight in Microsoft Dynamics 2011 - Marketing Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool für Ihr Vertriebsteam. Hier finden Sie eine schrittweise Anleitung, wie Sie es in Microsoft Dynamics 2011 On-Premises installieren und konfigurieren.

>[!PREREQUISITES]
>
>Füllen Sie die [Marketing-Microsoft-Integration](http://docs.marketo.com/x/DoA2) aus.
>
>[Laden Sie die richtige ](http://docs.marketo.com/x/LoJo) Lösung für Ihre Version von Microsoft Dynamics CRM herunter.

## Lösung {#import-solution} importieren

1. Melden Sie sich bei Microsoft Dynamics CRM an. Klicken Sie im Menü unten links auf **Einstellungen**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen Sie **Lösungen** in der Struktur.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicken Sie auf **Import** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Sie sollten [die Marketing-Lösung bereits installiert und konfiguriert haben, bevor Sie fortfahren.](install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md)

1. Klicken Sie auf **Durchsuchen**. Wählen Sie die Marketing Sales Insight-Lösung aus, die Sie [heruntergeladen haben. ](download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Überprüfen Sie die Details der Lösung und klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Stellen Sie sicher, dass die Option für die SDK-Meldung aktiviert ist. Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Warten Sie jetzt, bis der Import abgeschlossen ist.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicken Sie auf **Schließen**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight wird nun in der Liste zur Lösung angezeigt. Jay!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Wählen Sie Marketing to Sales Insight und klicken Sie auf **Alle Anpassungen veröffentlichen** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketing and Sales Insight {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei Marketing an und klicken Sie auf **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt **Sales Insight **auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie die **Marketo-Host**, **API-URL** und **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen **Geheimschlüssel der API** Ihrer Wahl ein und klicken Sie auf **SAVE**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit *Lead und Kontakt* funktionieren:
   >
   >    
   >    
   >    * Priorität
   >    * Dringlichkeit
   >    * Relative Bewertung

   >    
   >    
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) durch.

1. Gehen Sie zurück zu Dynamik und wählen Sie **Einstellungen**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen Sie **Marketing-API-Konfiguration** in der Struktur.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicken Sie auf **Standardkonfiguration**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Geben Sie die Informationen ein, die Sie zuvor von Marketo erhalten haben.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicken Sie auf **Speichern.**

   ** ![](assets/image2015-5-4-11-3a28-3a13.png)

   **

## Benutzerzugriff einstellen {#set-user-access}

Richten Sie Benutzerrollen ein, um bestimmten Benutzern Zugriff auf Sales Insight zu gewähren.

1. Wählen Sie **Einstellungen**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Wählen Sie **Administration** in der Struktur.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Wählen Sie die Rolle **Marketo Sales Insight** und klicken Sie auf **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Und das ist es! Alle Benutzer, die Zugriff haben, können nun den Abschnitt mit dem Sales Insight in der Ansicht der Interessenten-/Kontaktdetails sehen.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Herzlichen Glückwunsch! Sie haben jetzt die Kraft von Marketo Sales Insight freigesetzt.

>[!NOTE]
>
>**Verwandte Artikel**
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](http://docs.marketo.com/x/BICMAg)

