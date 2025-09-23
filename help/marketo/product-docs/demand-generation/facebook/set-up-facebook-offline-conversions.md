---
unique-page-id: 11383953
description: Facebook-Offline-Konversionen einrichten - Marketo-Dokumente - Produktdokumentation
title: Einrichten von Offline-Konversionen in Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 5%

---

# Einrichten [!DNL Facebook] Offline-Konvertierungen {#set-up-facebook-offline-conversions}

Durch das Zurücksenden von Offline-Konversionsdaten an [!DNL Facebook] für Personen, die über Lead-Anzeigen erstellt wurden, kann Ihr Werbe-Team die Werbeausgaben besser als je zuvor optimieren. So richten Sie es ein.

>[!PREREQUISITES]
>
>* Sie müssen [Facebook-Lead-Anzeigen einrichten](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Sie müssen über ein genehmigtes Modell in [Umsatzzyklus-Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md) verfügen.

## Admin-Konfiguration {#admin-configuration}

1. Wechseln Sie zu Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Gehen Sie **[!UICONTROL LaunchPoint]** und doppelklicken Sie auf den zuvor erstellten Facebook-Lead-Anzeigen-Service.

   >[!NOTE]
   >
   >Wenn Sie das noch nicht getan haben, rufen Sie &quot;[ einrichten [!UICONTROL Facebook-]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)&quot; auf und kehren Sie hierher zurück.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Bearbeiten Sie bei Bedarf den **[!UICONTROL Anzeigename]**, um Offline-Konversionen einzuschließen. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Markieren Sie **[!UICONTROL Offline-Konversionen aktivieren]** und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Süß! Die Aktivierung [!DNL Facebook] Offline-Konversionen ist zur Hälfte abgeschlossen. Gehen wir nun zum Umsatzzyklus Modeler , um die Stadien zu kartieren.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Konfiguration von Modeler für den Umsatzzyklus {#revenue-cycle-modeler-configuration}

1. Navigieren Sie zu **[!UICONTROL Analytics]**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Wählen Sie Ihr Modell aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Derzeit gibt es 10 [!DNL Facebook], denen Sie Umsatzzyklusphasen zuordnen können:
   >
   >* Hinzufügen von Zahlungsinformationen
   >* Zu Warenkorb hinzufügen
   >* Add to Wish List
   >* Registrierungen abgeschlossen
   >* Checkouts initiiert
   >* Person
   >* Andere
   >* Kauf
   >* Suchvorgänge
   >* Inhaltsanzeigen

1. Wählen Sie das Stadium aus, das Sie zuordnen möchten, und wählen Sie dann aus **[!UICONTROL Dropdown-Liste]** Facebook-Konversion“ das [!DNL Facebook] Ereignis aus, dem Sie es zuordnen möchten. Wiederholen Sie diesen Schritt, um alle Phasen in Ihrem RCM der Offline-Konvertierung in [!DNL Facebook] zuzuordnen.

   ![](assets/1-1.png)

1. Wenn Sie die Zuordnung abgeschlossen haben, schließen Sie das Modell.

   ![](assets/2.png)

1. Genehmigen Sie Ihr Modell und Sie sind fertig!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Wenn nun Lead-Anzeigen-Leads die Stadien erreichen, die Sie zugeordnet haben, werden die Konversionen zur Berichterstellung an [!DNL Facebook] gesendet.

   >[!CAUTION]
   >
   >Überprüfen Sie Ihr [!DNL Facebook] und stellen Sie sicher, dass alle [Anzeigen“ ](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&cmsid&creative=link&creative_detail=advertiser-help-center&create_type&destination_cms_id&orig_http_referrer) Ereignissatz Marketo Offline-Konversionen verknüpft sind. Ist dies nicht der Fall, funktioniert die Attribution möglicherweise nicht.

   >[!NOTE]
   >
   >Offline-Konversionsdaten werden mehrmals täglich von Marketo an [!DNL Facebook] gesendet.

>[!MORELIKETHIS]
>
>[Grundlagen [!DNL Facebook] Offline-Konversionen](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
