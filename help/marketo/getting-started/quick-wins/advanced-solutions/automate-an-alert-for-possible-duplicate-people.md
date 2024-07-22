---
unique-page-id: 7513680
description: Warnhinweis für mögliche doppelte Personen automatisieren - Marketo-Dokumente - Produktdokumentation
title: Automatisieren eines Warnhinweises für mögliche doppelte Personen
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatisieren eines Warnhinweises für mögliche doppelte Personen {#automate-an-alert-for-possible-duplicate-people}

Möchten Sie jedes Mal, wenn eine doppelte Person erstellt wird, einen Warnhinweis erstellen? So richten Sie eine Smart-Kampagne ein.

1. [Erstellen Sie eine neue Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Definieren Sie die folgende Smart-Liste:

* Trigger: **[!UICONTROL Benutzer wird erstellt]**
* Filter: **[!UICONTROL Duplizieren Sie die Felder]**. Feldname **[!UICONTROL ist ] [!UICONTROL Vollständiger Name]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Seien Sie kreativ! Experimentieren Sie mit verschiedenen Feldern, um bessere Ergebnisse zu erzielen.

1. Wählen Sie im Flussschritt die Flussaktion [[!UICONTROL Warnung senden]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} aus.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Verwendung des Tokens [Warnhinweisinformationen senden](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} , um einen Link zur Person in Ihr CRM-System aufzunehmen.

   >[!CAUTION]
   >
   >Wenn Sie eine große Liste importieren, erhalten Sie möglicherweise alle Warnhinweise gleichzeitig!
   >
   >Außerdem bedeuten zwei Personen mit demselben Namen nicht automatisch, dass sie dieselbe Person sind.

1. Aktivieren Sie die Kampagne auf der Registerkarte **[!UICONTROL Plan]** .

   ![](assets/automate-an-alert-3.png)

Das ist es! Diese Smart-Kampagne wird jedes Mal Trigger, wenn in Marketo eine neue Person mit dem vollständigen Namen erstellt wird.

>[!MORELIKETHIS]
>
>[Duplizierte Personen suchen und zusammenführen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
