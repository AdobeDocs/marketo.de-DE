---
unique-page-id: 7513680
description: Automatisieren eines Warnhinweises für möglicherweise doppelte Personen - Marketo-Dokumente - Produktdokumentation
title: Automatisieren eines Warnhinweises für mögliche doppelte Personen
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 1%

---

# Automatisieren eines Warnhinweises für mögliche doppelte Personen {#automate-an-alert-for-possible-duplicate-people}

Möchten Sie jedes Mal, wenn eine mögliche doppelte Person erstellt wird, einen Warnhinweis erstellen? Gehen Sie wie folgt vor, um eine Smart Campaign einzurichten.

1. [Erstellen Sie eine neue intelligente Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Definieren Sie die folgende Smart-Liste:

* Trigger: **[!UICONTROL Person wird erstellt]**
* Filter: **[!UICONTROL Felder duplizieren]**. Feldname **[!UICONTROL is] [!UICONTROL Full Name]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Seien Sie kreativ! Experimentieren Sie mit verschiedenen Feldern, um bessere Filterergebnisse zu erhalten.

1. Wählen Sie im Flussschritt die Flussaktion [[!UICONTROL Warnhinweis senden]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} aus.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Verwenden Sie das Token [Warnhinweis-Info senden](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}, um einen Link zur Person in Ihr CRM aufzunehmen.

   >[!CAUTION]
   >
   >Wenn Sie eine große Liste importieren, erhalten Sie möglicherweise eine Reihe dieser Warnungen gleichzeitig!
   >
   >Zwei Personen mit demselben Namen bedeuten nicht automatisch, dass sie dieselbe Person sind.

1. Aktivieren Sie die Kampagne auf der Registerkarte **[!UICONTROL Zeitplan]** .

   ![](assets/automate-an-alert-3.png)

Das ist alles! Diese Smart-Kampagne wird jedes Mal Trigger, wenn in Marketo eine neue Person mit einem vorhandenen vollständigen Namen erstellt wird.

>[!MORELIKETHIS]
>
>[Doppelte Personen suchen und zusammenführen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
