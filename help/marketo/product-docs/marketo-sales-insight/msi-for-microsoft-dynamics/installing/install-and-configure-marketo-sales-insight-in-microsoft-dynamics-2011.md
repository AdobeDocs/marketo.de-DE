---
unique-page-id: 3571735
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 - Marketo Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool für Ihr Verkaufsteam. Hier finden Sie die schrittweise Anleitung zum Installieren und Konfigurieren in Microsoft Dynamics 2011 On-Premises.

>[!PREREQUISITES]
>
>Schließen Sie Ihre Marketo-Microsoft-Integration ab.
>
>[Laden Sie die richtige Lösung herunter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) für Ihre Version von Microsoft Dynamics CRM.

## Importlösung {#import-solution}

1. Melden Sie sich bei Microsoft Dynamics CRM an. Klicken Sie unten links im Menü auf **Einstellungen** .

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen Sie **Lösungen** im Baum aus.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicken Sie auf **Import** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Sie sollten die Marketo-Lösung bereits mit [installiert und konfiguriert](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) haben, bevor Sie fortfahren.

1. Klicken Sie auf **Durchsuchen**. Wählen Sie die Marketo Sales Insight-Lösung aus, die Sie [heruntergeladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) haben. Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Überprüfen Sie die Details der Lösung und klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Stellen Sie sicher, dass die Option SDK-Nachricht aktiviert ist. Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Warten Sie nun, bis der Import abgeschlossen ist.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicken Sie auf **Schließen**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight wird nun in der Lösungsliste angezeigt. Ja!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Wählen Sie Marketo Sales Insight und klicken Sie auf **Publish All Customizations** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Verbinden von Marketo und Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie unter dem Abschnitt **Sales Insight** auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **Marketo-Host**, die **API-URL** und die **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen **API-geheimen Schlüssel** Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit _Lead und Kontakt_ funktionieren, damit Sales Insight funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [diesen Vorgang](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Gehen Sie zurück zu Dynamics und wählen Sie **Einstellungen** aus.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen Sie **Marketo API Config** im Baum aus.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicken Sie auf **Standardkonfiguration**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo erhalten haben.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Benutzerzugriff festlegen {#set-user-access}

Richten Sie Benutzerrollen ein, um bestimmten Benutzern Zugriff auf Sales Insight zu gewähren.

1. Wählen Sie **Einstellungen** aus.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Wählen Sie **Administration** im Baum aus.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Wählen Sie die Rolle **Marketo Sales Insight** aus und klicken Sie auf **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Und das ist es! Alle Benutzer, die Zugriff haben, können jetzt den Abschnitt mit den Einblicken aus dem Vertrieb in der Detailansicht des Leads/Kontakts sehen.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Herzlichen Glückwunsch. Sie haben jetzt die Leistung von Marketo Sales Insight freigesetzt.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
