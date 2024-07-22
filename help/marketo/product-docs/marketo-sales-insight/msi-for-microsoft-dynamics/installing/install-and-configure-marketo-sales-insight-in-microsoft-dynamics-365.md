---
unique-page-id: 3571739
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 365 - Marketo Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 1%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool, mit dem Sie Ihrem Vertriebsteam ein &quot;Fenster&quot;in den Datenbestand des Marketing-Teams geben können. So installieren und konfigurieren Sie Folgendes:

>[!PREREQUISITES]
>
>Schließen Sie Ihre Marketo-Microsoft-Integration ab.
>
>[Laden Sie die richtige Lösung herunter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) für Ihre Version von Microsoft Dynamics CRM.

## Importlösung {#import-solution}

1. Melden Sie sich bei [Microsoft Office 365](https://login.microsoftonline.com/) an.

   ![](assets/image2015-3-16-15-58-55.png)

1. Klicken Sie auf das Menü ![—](assets/image2015-3-16-16-1-13.png) und wählen Sie **CRM** aus.

   ![](assets/image2015-3-16-16-0-10.png)

1. Klicken Sie auf das Menü ![—](assets/image2015-5-13-10-5-8.png) . Wählen Sie in der Dropdown-Liste **Einstellungen** und dann **Lösungen** aus.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Sie sollten bereits [die Marketo-Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) installiert und konfiguriert haben, bevor Sie fortfahren.

1. Klicken Sie auf **Importieren**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicken Sie im neuen Fenster auf **Durchsuchen**. Wählen Sie die in Schritt 1.1 heruntergeladene Lösung [Marketo Sales Insight . ](#msi) Klicken Sie auf **Weiter**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt bei Bedarf anzeigen. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Stellen Sie sicher, dass Sie das Feld **markiert** lassen und auf **Importieren** klicken.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sie können die Protokolldatei herunterladen. Klicken Sie auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastisch! Sie sollten die Lösung jetzt sehen. Wenn er nicht vorhanden ist, aktualisieren Sie den Bildschirm.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Klicken Sie auf **Alle Anpassungen Publish**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Verbinden von Marketo und Sales Insight {#connect-marketo-and-sales-insight}

Verknüpfen wir Ihre Marketo-Instanz mit Sales Insight in Dynamics. Gehen Sie wie folgt vor:

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Melden Sie sich bei Marketo an und wechseln Sie zum Abschnitt **Admin** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie unter dem Abschnitt **Sales Insight** auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **Marketo-Host**, die **API-URL** und die **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen **API-geheimen Schlüssel** Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Die folgenden Felder müssen mit Marketo synchronisiert werden, damit _Lead und Kontakt_ funktionieren, damit Sales Insight funktioniert:
   >
   > * Priorität
   > * Dringlichkeit
   > * Relative Bewertung
   >
   >Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, führen Sie [diesen Vorgang](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) aus.

1. Klicken Sie in Microsoft Dynamics auf das Symbol ![](assets/image2015-5-13-15-3a49-3a19.png) neben Einstellungen und wählen Sie dann im Dropdown-Menü **Marketo API Config** aus.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Klicken Sie auf **Standardkonfiguration**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo kopiert haben.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Klicken Sie unten rechts auf das Symbol &quot;![](assets/image2015-5-13-16-3a8-3a51.png)&quot;, um die Änderungen zu speichern.

## Benutzerzugriff festlegen {#set-user-access}

Sie müssen Benutzern Berechtigungen zur Verwendung von Sales Insight erteilen.

1. Klicken Sie auf das Menü ![](assets/image2015-5-13-10-3a5-3a8.png) . Wählen Sie im Dropdown-Menü **Einstellungen** und dann **Sicherheit** aus.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insight gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Wählen Sie die Rolle **Marketo Sales Insight** aus und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Und du solltest fertig sein! Melden Sie sich zum Testen bei Dynamics als Benutzer an, der Zugriff auf Marketo Sales Insight hat, und sehen Sie sich einen Lead oder Kontakt an.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Sie haben jetzt die Möglichkeiten von Marketo Sales Insight für Ihr Vertriebsteam freigeschaltet.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
