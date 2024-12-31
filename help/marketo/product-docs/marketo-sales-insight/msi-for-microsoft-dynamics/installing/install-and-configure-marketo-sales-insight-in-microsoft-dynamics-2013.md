---
unique-page-id: 3571737
description: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013 - Marketo-Dokumentation - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 2%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight ist ein fantastisches Tool, mit dem Sie Ihrem Vertriebsteam einen Einblick in die Fülle der Daten gewähren können, über die das Marketing-Team verfügt. So installieren und konfigurieren Sie es.

>[!PREREQUISITES]
>
>Abschließen der Marketo-Microsoft-Integration
>
>[Laden Sie die richtige Lösung ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) Ihrer Version von Microsoft Dynamics CRM herunter.

## Lösung importieren {#import-solution}

Jetzt ist es an der Zeit, die Marketo Sales Insight-Lösung in Microsoft Dynamics zu importieren.

1. Klicken Sie unter **Microsoft Dynamics CRM** auf **Einstellungen**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Klicken **unter „Einstellungen** auf **Anpassungen**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Klicken Sie auf **Lösungen**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Sie sollten Marketo bereits installiert und konfiguriert haben, bevor Sie fortfahren

1. Klicken Sie **Importieren**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicken Sie im neuen Fenster auf &quot;**&quot;**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Suchen Sie die Lösung, die Sie oben heruntergeladen haben, und wählen Sie sie aus.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Die Lösung wird hochgeladen. Sie können den Paketinhalt anzeigen, wenn Sie möchten. Klicken Sie auf **Weiter**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Lassen Sie das Kontrollkästchen aktiviert und klicken Sie auf **Importieren**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sie können die Protokolldatei gerne herunterladen. Klicken Sie auf **Schließen**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastisch! Sie sollten die Lösung jetzt sehen. Wenn er nicht da ist, aktualisieren Sie Ihren Bildschirm.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Marketo und Sales Insight verbinden {#connect-marketo-and-sales-insight}

Binden wir Ihre Marketo-Instanz an Sales Insights in Dynamics.

>[!NOTE]
>
>Administratorrechte erforderlich.

1. Melden Sie sich bei Marketo an und gehen Sie zum Abschnitt **Admin** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicken Sie im Abschnitt **Sales Insights** auf **API-Konfiguration bearbeiten**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopieren Sie den **Marketo** Host **, die API** und die **API-Benutzer-ID** zur Verwendung in einem späteren Schritt. Geben Sie einen **API-Geheimschlüssel** Ihrer Wahl ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie in Ihrem API-Geheimschlüssel kein kaufmännisches Und-Zeichen (&amp;).

   ![](assets/image2014-12-12-9-3a7-3a9.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Klicken **unter „Einstellungen** auf **Marketo API-Konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Geben Sie die Informationen ein, die Sie zuvor aus Marketo übernommen haben, und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Benutzerzugriff festlegen {#set-user-access}

Schließlich können Sie bestimmten Benutzenden Zugriff auf Marketo Sales Insight gewähren.

1. Navigieren Sie zu **Einstellungen**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Wählen Sie die Benutzer aus, denen Sie Zugriff auf Sales Insights gewähren möchten, und klicken Sie auf **Rollen verwalten**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Wählen Sie die Rolle **Marketo Sales Insight** aus und klicken Sie auf **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Und Sie sollten fertig sein! Um schließlich zu testen, melden Sie sich bei Dynamics als Benutzer an, der Zugriff auf Marketo Sales Insight hat, und sehen Sie sich einen Lead oder Kontakt an.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Sie haben jetzt die Leistungsfähigkeit von Marketo Sales Insight für Ihr Vertriebsteam freigeschaltet.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
