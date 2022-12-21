---
unique-page-id: 3571735
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 - Marketo Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool für Ihr Verkaufsteam. Hier finden Sie die schrittweise Anleitung zum Installieren und Konfigurieren in Microsoft Dynamics 2011 On-Premises.

>[!PREREQUISITES]
>
>Schließen Sie Ihre Marketo-Microsoft-Integration ab.
>
>[Die richtige Lösung herunterladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) für Ihre Microsoft Dynamics CRM-Version.

## Importlösung {#import-solution}

1. Melden Sie sich bei Microsoft Dynamics CRM an. Klicken **Einstellungen** im Menü unten links.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Auswählen **Lösungen** im Baum.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicken **Import** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Sie sollten bereits [installiert und konfiguriert](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) die Marketo-Lösung, bevor Sie fortfahren.

1. Klicken **Durchsuchen**. Wählen Sie die Marketo Sales Insight-Lösung aus. [heruntergeladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Klicken **Nächste**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Überprüfen Sie die Details der Lösung und klicken Sie auf **Nächste**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Stellen Sie sicher, dass die Option SDK-Nachricht aktiviert ist. Klicken **Nächste**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Warten Sie nun, bis der Import abgeschlossen ist.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicken Sie auf **Schließen**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight wird nun in der Lösungsliste angezeigt. Ja!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Wählen Sie Marketo Sales Insight und klicken Sie auf **Alle Anpassungen veröffentlichen** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Verbinden von Marketo und Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Unter dem **Sales Insight** Abschnittsklick **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie die **Marketo-Host**, **API-URL** und **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie eine **API-Geheimschlüssel** und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden für _Lead und Kontakt_ für Sales Insight funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung

   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahrens](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Kehren Sie zu Dynamics zurück, wählen Sie **Einstellungen**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Auswählen **Marketo API-Konfiguration** im Baum.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicken **Standardkonfiguration**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo erhalten haben.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicken **Speichern**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Benutzerzugriff festlegen {#set-user-access}

Richten Sie Benutzerrollen ein, um bestimmten Benutzern Zugriff auf Sales Insight zu gewähren.

1. Auswählen **Einstellungen**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Auswählen **Administration** im Baum.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicken **Benutzer**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Wählen Sie die **Marketo Sales Insight** Rolle und klicken Sie auf **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Und das ist es! Alle Benutzer, die Zugriff haben, können jetzt den Abschnitt mit den Einblicken aus dem Vertrieb in der Detailansicht des Leads/Kontakts sehen.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Beifall. Sie haben jetzt die Leistung von Marketo Sales Insight freigesetzt.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
