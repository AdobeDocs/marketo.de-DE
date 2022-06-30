---
unique-page-id: 7513680
description: Warnhinweis für mögliche doppelte Personen automatisieren - Marketo-Dokumente - Produktdokumentation
title: Warnhinweis für mögliche doppelte Personen automatisieren
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Warnhinweis für mögliche doppelte Personen automatisieren {#automate-an-alert-for-possible-duplicate-people}

Möchten Sie jedes Mal, wenn eine doppelte Person erstellt wird, einen Warnhinweis erstellen? So richten Sie eine Smart-Kampagne ein.

1. [Neue Smart-Kampagne erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}. Definieren Sie die folgende Smart-Liste:

* Trigger: **Person wird erstellt**
* Filter: **Duplizieren Sie Felder.** Feldname **ist vollständiger Name**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Sei kreativ! Experimentieren Sie mit verschiedenen Feldern, um bessere Ergebnisse zu erzielen.

1. Wählen Sie im Flussschritt [Warnhinweis senden](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)Fluss-Aktion {target=&quot;_blank&quot;}.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Verwenden der [Warnhinweisinformationen-Token senden](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}, um einen Link zur Person in Ihr CRM-System aufzunehmen.

   >[!CAUTION]
   >
   >Wenn Sie eine große Liste importieren, erhalten Sie möglicherweise alle Warnhinweise gleichzeitig!
   >
   >Außerdem bedeuten zwei Personen mit demselben Namen nicht automatisch, dass sie dieselbe Person sind.

1. Aktivieren Sie die Kampagne im **Zeitplan** Registerkarte.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

Das ist es! Diese Smart-Kampagne wird jedes Mal Trigger, wenn in Marketo eine neue Person mit dem vollständigen Namen erstellt wird.

>[!MORELIKETHIS]
>
>[Duplizierte Personen suchen und zusammenführen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
