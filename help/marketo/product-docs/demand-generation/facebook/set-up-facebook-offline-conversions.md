---
unique-page-id: 11383953
description: Einrichten von Facebook-Offline-Konversionen - Marketo-Dokumente - Produktdokumentation
title: Einrichten von Facebook-Offline-Konversionen
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 2%

---

# Einrichten von Facebook-Offline-Konversionen {#set-up-facebook-offline-conversions}

Durch das Zurücksenden von Offline-Konversionsdaten an Facebook für Personen, die über Lead Ads erstellt wurden, kann Ihr Werbeteam die Werbeausgaben optimieren. So richten Sie es ein.

>[!PREREQUISITES]
>
>* Sie müssen [Facebook Lead Ads einrichten](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Sie müssen über ein genehmigtes Modell in [Umsatzzyklus-Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md) verfügen.

## Administratorkonfiguration {#admin-configuration}

1. Navigieren Sie zu Marketo **Admin**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Wechseln Sie zu **LaunchPoint** und doppelklicken Sie auf den zuvor erstellten Facebook Lead Ads-Dienst.

   >[!NOTE]
   >
   >Wenn Sie dies nicht getan haben, fahren Sie mit [Einrichten von Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) fort und kehren Sie hierher zurück.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Bearbeiten Sie bei Bedarf den **Anzeigenamen**, um Offline-Konversionen einzuschließen. Klicken Sie auf **Weiter**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Aktivieren Sie die Option **Offline-Konversionen aktivieren** und klicken Sie auf **Weiter**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Süß! Sie haben die Aktivierung der Facebook-Offline-Konversionen auf halbem Wege abgeschlossen. Wechseln wir zum Modeler für den Umsatzzyklus, um die Bühnen zuzuordnen.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Modeler-Konfiguration für Umsatzzyklus {#revenue-cycle-modeler-configuration}

1. Wechseln Sie zu **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Wählen Sie Ihr Modell aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Derzeit gibt es 10 Facebook-Ereignisse, denen Sie Umsatzzyklusschritte zuordnen können:
   >
   >* Hinzufügung von Zahlungsinformationen
   >* Zum Warenkorb hinzugefügt
   >* Fügt der Wunschliste hinzu
   >* Abgeschlossene Registrierungen
   >* Checkouts initiiert
   >* Person
   >* Andere
   >* Kauf
   >* Suchvorgänge
   >* Inhaltsanzeigen

1. Wählen Sie die Bühne aus, die Sie zuordnen möchten, und wählen Sie dann aus der Dropdownliste **Facebook-Konversion** das Facebook-Ereignis aus, dem Sie es zuordnen möchten. Wiederholen Sie diesen Schritt, um alle Phasen in Ihrem RCM Offline-Konversionsphasen in Facebook zuzuordnen.

   ![](assets/1-1.png)

1. Wenn Sie die Zuordnung abgeschlossen haben, schließen Sie das Modell.

   ![](assets/2.png)

1. Genehmigen Sie Ihr Modell und Sie sind fertig!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Wenn Lead-Anzeigen-Leads jetzt die von Ihnen zugeordneten Bühnen erreichen, werden die Konversionen zur Berichterstellung an Facebook gesendet.

   >[!CAUTION]
   >
   >Überprüfen Sie Ihr Facebook-Konto und stellen Sie sicher, dass alle [Anzeigen](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) mit dem Marketo-Ereignis &quot;Offline-Konversionen&quot;verknüpft sind. Ist dies nicht der Fall, funktioniert die Anzeigenzuordnung möglicherweise nicht.

   >[!NOTE]
   >
   >Offline-Konversionsdaten werden mehrmals täglich von Marketo an Facebook gesendet.

>[!MORELIKETHIS]
>
>[Offline-Konversionen von Facebook verstehen](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
