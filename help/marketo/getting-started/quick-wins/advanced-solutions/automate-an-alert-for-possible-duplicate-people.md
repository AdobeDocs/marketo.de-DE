---
unique-page-id: 7513680
description: Automatisieren eines Warnhinweises für potenzielle Duplikat-Personen - Marketing-Dokumente - Produktdokumentation
title: Automatisieren einer Warnung für mögliche Duplikat-Personen
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Automatisieren einer Warnung für mögliche Duplikat-Personen {#automate-an-alert-for-possible-duplicate-people}

Sie möchten bei jedem Erstellen eines Duplikats eine Warnung erhalten? So richten Sie eine intelligente Kampagne ein.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. [Erstellen Sie eine neue intelligente Kampagne](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md). Definieren Sie die folgende intelligente Liste:

   * Auslöser: **Person erstellt**
   * Filter: **Duplikat-Felder. **Feldname **ist** **Vollständiger Name**.

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Sei kreativ! Experimentieren Sie mit verschiedenen Feldern, um bessere Filterergebnisse zu erhalten.

1. Wählen Sie im Flussschritt die Option Aktion für den [Sendewarnfluss](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Verwenden des Tokens &quot; [Warnhinweisinformationen senden&quot;, um einen Link zu der Person in Ihrem CRM-System einzuschließen](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) .

   >[!CAUTION]
   >
   >Wenn Sie eine große Liste importieren, erhalten Sie möglicherweise einen Haufen dieser Warnungen auf einmal!
   >
   >
   >Zwei Personen mit demselben Namen bedeuten nicht automatisch, dass sie die gleiche Person sind.

1. Aktivieren Sie die Kampagne auf der Registerkarte &quot; **Plan** &quot;.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

Das ist&#39;s! Diese intelligente Kampagne wird jedes Mal ausgelöst, wenn in Marketo eine neue Person mit einem vorhandenen vollständigen Namen erstellt wird.

>[!MORELIKETHIS]
>
>* [Duplikat-Personen suchen und zusammenführen](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

