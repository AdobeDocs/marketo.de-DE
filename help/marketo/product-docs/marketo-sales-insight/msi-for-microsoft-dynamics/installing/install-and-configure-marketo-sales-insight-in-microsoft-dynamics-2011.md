---
unique-page-id: 3571735
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 - Marketo-Dokumentation - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 2%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool für Ihr Vertriebsteam. Hier finden Sie eine schrittweise Anleitung zur Installation und Konfiguration vor Ort in Microsoft Dynamics 2011.

>[!PREREQUISITES]
>
>Abschließen der Marketo-Microsoft-Integration
>
>[Laden Sie die richtige Lösung ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Ihrer Version von Microsoft Dynamics CRM herunter.

## Lösung importieren {#import-solution}

1. Beim Microsoft Dynamics CRM anmelden. Klicken **im** Menü unten links auf „Einstellungen“.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen **in** Struktur „Lösungen“ aus.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicken Sie **Importieren** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Sie sollten die Marketo[Lösung bereits installiert und ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) haben, bevor Sie fortfahren.

1. Klicken Sie **Durchsuchen**. Wählen Sie die Marketo Sales Insight-Lösung aus, die Sie [heruntergeladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Überprüfen Sie die Details der Lösung und klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Stellen Sie sicher, dass die Option SDK-Nachricht aktiviert ist. Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Warten Sie nun, bis der Import abgeschlossen ist.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicken Sie auf **Schließen**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight wird jetzt in der Lösungsliste angezeigt. Juhu!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Wählen Sie Marketo Sales Insight aus und klicken Sie auf **Publish All Customizations** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Marketo und Sales Insight verbinden  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt **Sales Insights** auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **Marketo** Host **, die API** und die **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen **API-Geheimschlüssel** Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie in Ihrem API-Geheimschlüssel kein kaufmännisches Und-Zeichen (&amp;).

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit _Lead und Kontakt_ Sales Insight funktioniert:
   >
   >* Priorität
   >* Dringlichkeit
   >* Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [dieses Verfahren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Wechseln Sie zurück zu Dynamics und wählen Sie **Einstellungen** aus.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Wählen Sie **Marketo-API** Konfiguration“ in der Baumstruktur aus.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicken Sie **Standardkonfiguration**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo übernommen haben.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Benutzerzugriff festlegen {#set-user-access}

Richten Sie Benutzerrollen ein, um bestimmten Benutzern Zugriff auf Sales Insights zu gewähren.

1. Wählen Sie **Einstellungen** aus.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Wählen Sie **Struktur** Administration“ aus.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Wählen Sie die Rolle **Marketo Sales Insight** aus und klicken Sie auf **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Und das war&#39;s! Alle Benutzer, die Zugriff haben, können jetzt den Abschnitt „Vertriebserkenntnisse“ in der Lead-/Kontaktdetailansicht sehen.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Glückwunsch. Sie haben jetzt die Leistungsfähigkeit von Marketo Sales Insight freigesetzt.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
