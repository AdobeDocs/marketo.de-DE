---
unique-page-id: 37355602
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online - Marketo-Dokumente - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 2%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight ist ein fantastisches Tool, mit dem Sie Ihrem Vertriebsteam einen Einblick in die Fülle der Daten verschaffen können, über die das Marketing-Team verfügt. Im Folgenden wird beschrieben, wie Sie sie in Microsoft Dynamics Online installieren und konfigurieren.

>[!PREREQUISITES]
>
>Abschließen der Marketo-Microsoft-Integration
>
>[Laden Sie die richtige Lösung ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Ihrer Version von Microsoft Dynamics CRM herunter.

## Lösung importieren {#import-solution}

>[!NOTE]
>
>Wenn Sie die einheitliche Benutzeroberfläche verwenden, klicken Sie vor Schritt 1 unten auf das Einstellungssymbol in der oberen rechten Ecke und wählen Sie **Erweiterte Einstellungen**.

1. Klicken Sie unter Microsoft Dynamics CRM **Einstellungen**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Klicken Sie unter Einstellungen auf **Anpassungen**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Klicken Sie auf **Lösungen**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Sie sollten die Marketo-Lösung bereits installiert und konfiguriert haben, bevor Sie fortfahren.

1. Klicken Sie **Importieren**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Klicken Sie im neuen Fenster auf &quot;**&quot;**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Suchen Sie auf Ihrem Computer nach der Lösung, die Sie gerade heruntergeladen haben, und installieren Sie sie.

1. Klicken Sie auf **Weiter**.

   ![](assets/seven.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt anzeigen, wenn Sie möchten. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Lassen Sie das Kontrollkästchen aktiviert und klicken Sie auf **Importieren**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Laden Sie die Protokolldatei herunter und klicken Sie dann auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastisch! Sie sollten die Lösung jetzt sehen. Wenn er nicht da ist, aktualisieren Sie Ihren Bildschirm.

   ![](assets/eleven.png)

1. Klicken Sie auf **Publish-Anpassung**.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie die globale MS Dynamics-Synchronisierung aktivieren.

## Marketo und Sales Insight verbinden {#connect-marketo-and-sales-insight}

Binden wir Ihre Marketo-Instanz an Sales Insights in Dynamics. So geht&#39;s:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei Marketo an und gehen Sie zum Abschnitt **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Klicken Sie im Abschnitt Sales Insights auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Kopieren Sie den **Marketo** Host **, die API** und die **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen API-Geheimschlüssel Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie in Ihrem API-Geheimschlüssel kein kaufmännisches Und-Zeichen (&amp;).

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit _Lead und Kontakt_ Sales Insight funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Zurück in Microsoft Dynamics, gehen Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Klicken **unter „Einstellungen** auf **Marketo API-Konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo übernommen haben, und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/enable-one.png)

1. Wählen Sie unter Integration die Option **Microsoft Dynamics** aus.

   ![](assets/enable-two.png)

1. Klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/enable-three.png)

1. Klicken Sie **Bearbeiten** neben Details zur Feldsynchronisierung.

   ![](assets/enable-four.png)

1. Dadurch _(automatisch_ zuvor deaktivierte MSI-Felder (Dringlichkeit, Relativer Wert und Priorität) ausgewählt. Klicken Sie einfach auf **Speichern**, um mit der Synchronisierung von Daten zu beginnen.

   ![](assets/enable-five.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich müssen Sie bestimmten Benutzenden Zugriff gewähren, um Marketo Sales Insight verwenden zu können.

1. Navigieren Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Navigieren Sie zu **Sicherheit**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insights gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Wählen Sie die Rolle Marketo Sales Insights aus und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Und Sie sollten fertig sein! Melden Sie sich zum Testen bei Dynamics als Benutzer an, der Zugriff auf Marketo Sales Insight hat, und prüfen Sie einen Lead oder Kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
